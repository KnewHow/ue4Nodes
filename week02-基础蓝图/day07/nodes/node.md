# day07

## 1 函数

### 1.1 函数创建

![image-20200512092146892](../images/image-20200512092146892.png)

### 1.2 函数细节

![image-20200512092232215](../images/image-20200512092232215.png)

#### 1.2.1 keywords

![image-20200512092437280](../images/image-20200512092437280.png)



#### 1.2.2 Access Specifier

![image-20200512092918398](../images/image-20200512092918398.png)



#### 1.2.3 参数设置

![image-20200512092828245](../images/image-20200512092828245.png)



#### 1.2.4 输出(返回值)

可以有多个

![image-20200512093120642](../images/image-20200512093120642.png)

#### 1.2.5 纯函数

纯函数打开的时候，函数的颜色发生了变化，此时的函数应该没有副作用。

纯函数用于计算量较小的逻辑

![image-20200512093427776](../images/image-20200512093427776.png)



非纯函数时候的状态：

![image-20200512093550945](../images/image-20200512093550945.png)

在下面的例子中：



纯函数会被调用两次：



非纯函数只会被调用一次：

![image-20200512093858303](../images/image-20200512093858303.png)



#### 1.2.6 蓝图函数库

![image-20200512094048918](../images/image-20200512094048918.png)

![image-20200512094127806](../images/image-20200512094127806.png)



![image-20200512094310404](../images/image-20200512094310404.png)



其实可以这么区分，目标函数在一个类(Actor)里面,必须依靠类存在，而蓝图库函数，不依赖任何类(对象)，他是一个独立的函数。



## 2 项目实战

### 2.1 获取摄像机位置

![image-20200512101113038](../images/image-20200512101113038.png)



### 2.2 让一个物体始终面对玩家的方法

![image-20200512104314359](../images/image-20200512104314359.png)



## 3 事件

![image-20200512105535388](../images/image-20200512105535388.png)

### 3.1 函数和事件的区别

函数有返回值，但是事件不行。

![image-20200512105634097](../images/image-20200512105634097.png)

### 3.2 批量创建Actor

![image-20200512110153282](../images/image-20200512110153282.png)

### 3.3 定义事件调度器

![image-20200512110359845](../images/image-20200512110359845.png)

![image-20200512110406436](../images/image-20200512110406436.png)

### 3.4 分发事件

![image-20200512112436786](../images/image-20200512112436786.png)



### 3.5 监听事件

上面的是定义一个监听事件的行为，下面的为当事件被送达的时候，需要执行的操作。

![image-20200513174618745](../images/image-20200513174618745.png)



### 3.6 解除事件

![image-20200512113136540](../images/image-20200512113136540.png)



### 3.7 添加 事件参数

![image-20200512141837627](../images/image-20200512141837627.png)



## 4 流程控制

![image-20200512134811954](../images/image-20200512134811954.png)

### 4.1 Branch

![image-20200512134424248](../images/image-20200512134424248.png)

### 4.2 Sequence

![image-20200512134413075](../images/image-20200512134413075.png)

### 4.3 Do Once 和 Do N

![image-20200512134346711](../images/image-20200512134346711.png)

### 4.4 DoOnce MultiInput

![image-20200512135023107](../images/image-20200512135023107.png)

### 4.5 Flip-Flop

![image-20200512135104408](../images/image-20200512135104408.png)

###  4.6 ForLoop

![image-20200512135003137](../images/image-20200512135003137.png)

### 4.7 ForLoopWithBreak

![image-20200512135247810](../images/image-20200512135247810.png)

### 4.8 ForEachLoop(高级For)和ForEachLoopWithBreak

![image-20200512135709783](../images/image-20200512135709783.png)

![image-20200512135753064](../images/image-20200512135753064.png)



### 4.9 Gate

![image-20200512140044006](../images/image-20200512140044006.png)

### 4.10 Switch 

![image-20200512163147537](../images/image-20200512163147537.png)

### 4.11 Delay

延迟执行

![image-20200512163224772](../images/image-20200512163224772.png)



### 4.12 FormatText

![image-20200512135912295](../images/image-20200512135912295.png)



## 5 宏(macro)

用于自定义某些函数、流程等，和C++里面的宏差不多。

### 5.1 创建宏蓝图

![image-20200512140702370](../images/image-20200512140702370.png)

### 5.2 定义宏

![image-20200512141518258](../images/image-20200512141518258.png)



### 5.3 使用宏

![image-20200512141604991](../images/image-20200512141604991.png)





## 6 实现破坏

### 6.1 添加插件

![image-20200512144422950](../images/image-20200512144422950.png)



### 6.2 创建对应的爆炸体

不能用ue4里面的Cube,可以使用新手包里面的Shapes

![image-20200512145234905](../images/image-20200512145234905.png)

 ### 6.3 破坏预览和调整参数

![image-20200512144231808](../images/image-20200512144231808.png)



### 6.4 参数的含义

![image-20200512145000615](../images/image-20200512145000615.png)

和这个值相对应：

![image-20200512151608618](../images/image-20200512151608618.png)



![image-20200512151654125](../images/image-20200512151654125.png)

![image-20200512151848409](../images/image-20200512151848409.png)

### 6.5 在蓝图中实现

添加可以爆炸物体：

![image-20200512152622428](../images/image-20200512152622428.png)

使用蓝图的流程控制：

![image-20200512152450649](../images/image-20200512152450649.png)



## 7 构造脚本和Select

### 7.1 构造脚本

构造函数在Actor创建或者是Actor的Detail的属性发生变化时会调用。尤其是第二个，我们可以利用第二个来简化我们的场景构造，我们将一大堆物体拖进场景，然后分别设置他的某个值，然后让构造函数执行某些操作

![image-20200512154842172](../images/image-20200512154842172.png)



### 7.2 Select

![image-20200512162833699](../images/image-20200512162833699.png)

