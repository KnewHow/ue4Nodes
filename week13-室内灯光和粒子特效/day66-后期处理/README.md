# 后期处理（POST PROCESS）

## 1 后期处理体积



### 1.1 全局生效

![image-20200728095355689](./images/image-20200728095355689.png)



### 1.2 混合权重(Blend Widget)

当多个后期处理框交叠的时候，每个部分站得比重

![image-20200728095531432](./images/image-20200728095531432.png)

## 2 Lens(镜头)

![image-20200728100051344](./images/image-20200728100051344.png)

### 2.1 Mobile Depth of Field (手机端场景景深)

![image-20200728100118838](./images/image-20200728100118838.png)

### 2.2 影视级摄像机

![image-20200728100446756](./images/image-20200728100446756.png)

摄像机类型：

![image-20200728100609329](./images/image-20200728100609329.png)

光圈：

![image-20200728102231231](./images/image-20200728102231231.png)

光圈和清晰度:

![image-20200728102317873](./images/image-20200728102317873.png)



### 2. 3 Bloom 灯光增益

![image-20200728104004882](./images/image-20200728104004882.png)



### 2.4 Exposure 自动曝光

由明到暗时，模拟人眼产生的明暗变化。让场景变亮变暗。

![image-20200728104341705](./images/image-20200728104341705.png)



![image-20200728104612933](./images/image-20200728104612933.png)



![image-20200728104640857](./images/image-20200728104640857.png)



![image-20200728104656607](./images/image-20200728104656607.png)



![image-20200728104720905](./images/image-20200728104720905.png)



![image-20200728104748259](./images/image-20200728104748259.png)



![image-20200728104811927](./images/image-20200728104811927.png)



![image-20200728104837219](./images/image-20200728104837219.png)



![image-20200728104829053](./images/image-20200728104829053.png)



![image-20200728104936221](./images/image-20200728104936221.png)



### 2.5 Chromatic Aberration(迷幻效果)

模拟人喝醉酒之后的场景

![image-20200728110515059](./images/image-20200728110515059.png)



### 2.6 Dirt Mask（污渍遮蔽）

![image-20200728111324474](./images/image-20200728111324474.png)



### 2.7 Lens Flares(镜头炫光)

![image-20200728111646366](./images/image-20200728111646366.png)



参数：

![image-20200728111827431](./images/image-20200728111827431.png)



颜色效果：

![image-20200728112123796](./images/image-20200728112123796.png)



### 2.8 Image Effect——摄像头效果

![image-20200728112712533](./images/image-20200728112712533.png)



监视摄像头：

![image-20200728112753236](./images/image-20200728112753236.png)



这些东西在影视摄像机里面都是可以单独设置的：

![image-20200728112858741](./images/image-20200728112858741.png)



## 3 Color Grading 调色——重点

![image-20200728115652216](./images/image-20200728115652216.png)

### 3.1 WhiteBlance(白平衡)

![image-20200728115738671](./images/image-20200728115738671.png)

染色：

![image-20200728120003740](./images/image-20200728120003740.png)

### 3.2 Global 全局颜色

![image-20200728120739081](./images/image-20200728120739081.png)

Saturation:饱和度

Contrast:对比度

![image-20200728120901982](./images/image-20200728120901982.png)

Gamma: 

Gain:增益

Offset 颜色偏移：

![image-20200728121134498](./images/image-20200728121134498.png)

### 3.3 Height Lighness(高光)

只针对高光的地方做处理

![image-20200728121335595](./images/image-20200728121335595.png)

### 3.4 Shadows(影子)

针对暗的地方调整

![image-20200728121802817](./images/image-20200728121802817.png)



### 3.5 Misc(杂项，自定义色卡)

标准色卡：

![image-20200728142229913](./images/image-20200728142229913.png)

获取修改色卡：

![image-20200728141924945](./images/image-20200728141924945.png)

将修改丢入Misc:

![image-20200728141628210](./images/image-20200728141628210.png)

此时需要将图片变成无压缩：

![image-20200728142518185](./images/image-20200728142518185.png)



## 4 Rendering Features

![image-20200728151654376](./images/image-20200728151654376.png)

### 4.1 Ambient Occlusion

![image-20200728151926016](./images/image-20200728151926016.png)

### 4.2 全局光照

![image-20200728152332460](./images/image-20200728152332460.png)



### 4.3 （Motion Blur） 动态模糊 

对于会动的东西产生一些模糊

![image-20200728152532567](./images/image-20200728152532567.png)

### 4.4 反射和屏幕空间反射

![image-20200728153008442](./images/image-20200728153008442.png)

### 4.5 折射

![image-20200728153215127](./images/image-20200728153215127.png)

### 4.6 后期处理材质

![image-20200728153352123](./images/image-20200728153352123.png)

材质的固定格式：

![image-20200728153453664](./images/image-20200728153453664.png)

让场景变成粉色：

![image-20200728153652476](./images/image-20200728153652476.png)



![image-20200728160651220](./images/image-20200728160651220.png)

### 4.7 制作血色闪动

![image-20200728165336866](C:\Users\JHxuhuan2\Desktop\image-20200728165336866.png)