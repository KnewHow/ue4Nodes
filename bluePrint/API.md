# 蓝图节点

## GetWorldLocation

获取当前对象在世界坐标中的位置，返回一个三维向量

![image-20200511185140936](./images/image-20200511185140936.png)



## GetWorldRotation

获取一个物体的旋转，返回一个`Rotator` 对象。

![image-20200511185425270](./images/image-20200511185425270.png)

## GetRotationXVector

将一个旋转值转换为X方向的向量。

![image-20200511185608277](./images/image-20200511185608277.png)

## LineTraceForObjects

碰撞线性追踪：

![image-20200511190100083](./images/image-20200511190100083.png)

碰撞的结果信息：

![image-20200511190225210](./images/image-20200511190225210.png)



## Branch

相当于`if...else`，输入是一个`bool`类型，`true`和`false`代表不同的分支

![image-20200511190411588](./images/image-20200511190411588.png)



## Make Transform

根据需要的值，新建一个`Transform`对象

![image-20200511190532069](./images/image-20200511190532069.png)



## SpawnActorFromClass

根据一个`Actor`模板创建一个`Actor`的实例，用于新建一个对象

![image-20200511190721464](./images/image-20200511190721464.png)

## Sequence

串行的执行多个操作，首先执行`then0`,完成后执行`then1`,以此类推

![image-20200511191009311](./images/image-20200511191009311.png)



## Is Valid

校验一个对象是否非法

![image-20200511191213490](./images/image-20200511191213490.png)



## GetActorLocation

获取Actor的位置

![image-20200511194703470](./images/image-20200511194703470.png)

## Lerp(插值)

![image-20200511194749181](./images/image-20200511194749181.png)



## VectorLength

向量的长度

![image-20200511194813805](./images/image-20200511194813805.png)



## Draw Debug Line

画一条调试线

![image-20200511194910134](./images/image-20200511194910134.png)

## Draw Debug String

画一条调试字符串

![image-20200511195001895](./images/image-20200511195001895.png)