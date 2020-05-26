# Day 14

## 1 实现射击不同的子弹

### 1.1 创建子弹类型枚举

![image-20200521094351869](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521094351869.png)

![image-20200521094620332](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521094620332.png)

### 1.2 局部变量和默认值

![image-20200521102419724](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521102419724.png)

### 1.3 停止时钟句柄

![image-20200521112601190](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521112601190.png)



## 2 动画蒙太奇

将原来的动画进行处理，如之前的跑步

## 3 战场播报

### 3.1 创建文字飘动的动画

给文字的透明度添加动画：

0s-> 0

1s->1

2s-> 0

![image-20200521135715277](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521135715277.png)

给文字的transform Y 添加动画

0s-> -30

1s-> 30

![image-20200521135503418](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521135503418.png)

### 3.1 监听动画播放结束事件

![image-20200521133912684](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521133912684.png)



## 4 摄像机

![image-20200521143616134](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521143616134.png)



![image-20200521143646137](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521143646137.png)

### 4.1 狙击镜

![image-20200521144157234](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521144157234.png)

### 4.2 屏幕尺寸

由于屏幕不是正方形，但是狙击镜是正方形，因此会被缩放，所以不能直接用，得使用材质。

![image-20200521153006045](C:\Users\JHxuhuan2\AppData\Roaming\Typora\typora-user-images\image-20200521153006045.png)