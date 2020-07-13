# Day21-Cpp 基础

## 1 新建 C++ 类

![image-20200601092956122](../images/image-20200601092956122.png)



### 1.1 分模块

![image-20200601100018017](../images/image-20200601100018017.png)



![image-20200601100104570](../images/image-20200601100104570.png)

### 1.2 GENERATED_BODY() 和 GENERAATED_UCLASS_BODY()

![image-20200601100631730](../images/image-20200601100631730.png)



### 1.3 BlueprintType 

![image-20200601101317837](../images/image-20200601101317837.png)



### 1.4 UPROPERTY(BlueprintReadWrite)——属性设置

BlueprintReadWrite: 蓝图可以读写

BlueprintReadOnly: 蓝图只读

设置变量的读写性质。

![image-20200601105359953](../images/image-20200601105359953.png)

### 1.5 Unreal Header Tool 扫描规则

这些规则的处理只是针对蓝图做处理，真正的c++代码是不管这些的规则的。

![image-20200601111110756](../images/image-20200601111110756.png)

### 1.6 数据类型

![image-20200601104717386](../images/image-20200601104717386.png)

![image-20200601104957354](../images/image-20200601104957354.png)

![image-20200601112014249](../images/image-20200601112014249.png)

因此 对于 Name,String 以及 Text,Vector 等类型，都是结构体变量

### 1.7 函数声明和实现

1. 函数声明

![image-20200601105717278](../images/image-20200601105717278.png)

函数实现：

![image-20200601110827224](../images/image-20200601110827224.png)

当然，我们可以快捷方式实现：

![image-20200601110927637](../images/image-20200601110927637.png)



### 1.8 创建一个类

![image-20200601111505013](../images/image-20200601111505013.png)

### 1.9 遍历数组

![image-20200601114841388](../images/image-20200601114841388.png)

### 1.10 蓝图使用引用实现多返回

![image-20200601115057285](../images/image-20200601115057285.png)

在蓝图中使用，你会发现传递引用的参数变成了返回值。

![image-20200601115116952](../images/image-20200601115116952.png)

### 1.11 定义结构体

结构体在 UE4 中相对于类来说，是一种较为轻量的数据结构。

![image-20200601135529807](../images/image-20200601135529807.png)

### 1.12 枚举定义

枚举需要以E开头

![image-20200601135702498](../images/image-20200601135702498.png)



### 1.13 创建Actor

1. 定义Actor

   ![image-20200601143109804](../images/image-20200601143109804.png)

2. 在.cpp 的文件中，实现构造函数

   ![image-20200601143238163](../images/image-20200601143238163.png)

   ![image-20200601143211769](../images/image-20200601143211769.png)

### 1.14 DEPRECATED

![image-20200601144944214](../images/image-20200601144944214.png)

### 1.15 Root Component

![image-20200601145412369](../images/image-20200601145412369.png)

### 1.16 在 Acotor 中添加静态物体

1. 在.h 文件中定义一个静态类型变量

   ![image-20200601152814996](../images/image-20200601152814996.png)

2. 在构造函数中绑定具体的模型

   ![image-20200601152733412](../images/image-20200601152733412.png)

   其中静态的模型`Path` 做如下获取：

   ![image-20200601153535383](../images/image-20200601153535383.png)

### 1.17 Class、Object、SoftClass、SoftObject

在资源浏览器中，所有的`Actor`、贴图、材质都是资源，他们都是类（Class），而当他们拖入场景就实例化为对象(Object)。

但是有些资源依赖其他的资源，如果在游戏开始的时候，就加载对于的资源，会很耗性能，但是我们可以使用软引用(SoftObject 或者 SoftObject)，这样