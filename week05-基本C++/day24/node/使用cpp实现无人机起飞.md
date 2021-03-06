# Day24-Cpp实现无人机

## 1 按键设置

无人机操作：

![image-20200604092621317](../images/image-20200604092621317.png)

参照美国手的设置，做如下按键输入：

![image-20200604092542195](../images/image-20200604092542195.png)

云台：

![image-20200604092937540](../images/image-20200604092937540.png)

紧急停浆：

![image-20200604093029662](../images/image-20200604093029662.png)

## 2 在 C++ 一些操作

### 2.1 绑定轴输入事件

![image-20200604171244813](../images/image-20200604171244813.png)

### 2.2 获取轴输入

![image-20200604171353890](../images/image-20200604171353890.png)

### 2.3 C++  预声明

![image-20200604101148815](../images/image-20200604101148815.png)

### 2.4 修改GameMode

修改GameMode为`雪地景观`的GameMode

### 2.5 修改 Pawn 为自己 C++ 新建的 Pawn

![image-20200604104317712](../images/image-20200604104317712.png)

### 2.6 在 C++ 中使用射线追踪

![image-20200604133105098](../images/image-20200604133105098.png)



### 2.7 WorldContextObject

事件上下文对象，可以用来创建 Actor,搜索 Actor.

### 2.8 获取向量长度

![image-20200604141151817](../images/image-20200604141151817.png)

和蓝图中的`VectorLength`一样

### 2.9 位置偏移

获取和设置位置偏移

![image-20200604165207123](../images/image-20200604165207123.png)

### 2.10 设置旋转

![image-20200604170411904](../images/image-20200604170411904.png)

### 2.11 建立结构体

![image-20200604170909552](../images/image-20200604170909552.png)

### 2.12 静态变量的声明和初始化

在头文件中声明：

![image-20200604171018754](../images/image-20200604171018754.png)

在cpp文件中初始化：

![image-20200604171052489](../images/image-20200604171052489.png)