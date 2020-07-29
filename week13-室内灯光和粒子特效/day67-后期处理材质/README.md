# 后期处理材质

## 1 冰的效果

### 1.1 制作法线

![image-20200729094610560](./images/image-20200729094610560.png)



![image-20200729110040795](./images/image-20200729110040795.png)

效果：

![image-20200729111632273](./images/image-20200729111632273.png)

## 2 镜像模糊

![image-20200729105741151](./images/image-20200729105741151.png)

使用材质实现：

![image-20200729114753047](./images/image-20200729114753047.png)

预览效果：

![image-20200729114709154](./images/image-20200729114709154.png)



## 3 使用 HLSL 模拟镜像模糊

![image-20200729120833089](./images/image-20200729120833089.png)



HLSL 代码，可以看到它使用 for 循环实现上面的五次相加，而且可以自定义次数，由此看来，使用 HLSL  来实现材质说一种非常简单的做饭。

```glsl
static const int SceneTextureId = 14;
float2 UV = GetDefaultSceneTextureUV(Parameters, SceneTextureId);
float3 Sum = float3(0, 0, 0);


float2 Dir = float2(CenterX, CenterY) - GetViewportUV(Parameters);
for (int it = 0; it < SampleNum; it++)
{
float2 UVOffset = it * Offset * length(Dir) * Dir;
#if SHADING_PATH_MOBILE
Sum += MobileSceneTextureLookup(Parameters, SceneTextureId, UV + UVOffset).rgb;
#else
Sum += SceneTextureLookup(UV + UVOffset, SceneTextureId, false).rgb;
#endif
}


return Sum/SampleNum;
```

参数暴露：

![image-20200729143222507](./images/image-20200729143222507.png)





引擎自定义：Shader

![image-20200729122338366](./images/image-20200729122338366.png)

参考链接：

https://www.cnblogs.com/herenzhiming/articles/5276106.html
https://blog.csdn.net/Invokar/article/details/80277334
https://www.raywenderlich.com/57-unreal-engine-4-custom-shaders-tutorial



## 4 景深

![image-20200729154241003](./images/image-20200729154241003.png)



添加到自定义景深：

![image-20200729154428177](./images/image-20200729154428177.png)