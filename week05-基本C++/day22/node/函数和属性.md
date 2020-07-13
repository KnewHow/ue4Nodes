# Day22

## 1 注释

### 1.1 版权信息

在文件首行，写上版权信息：

![image-20200602092535871](../images/image-20200602092535871.png)

### 1.2 文档注释

![image-20200602100826171](../images/image-20200602100826171.png)

### 1.3 Blueprintable/NotBlueprintable

让一个C++的类在蓝图中可用/不可用:

![image-20200602101827486](../images/image-20200602101827486.png)

![image-20200602101306044](../images/image-20200602101306044.png)

### 1.4 BlueprintType 和 NotBlueprintType

![image-20200602102305972](../images/image-20200602102305972.png)

可以参考宏



### 1.5 编码格式

安装utf-8插件，这样会让c++代码中的中文文档注释在UE4蓝图中显示出正确的内容，而不是乱码。

![image-20200602104413516](../images/image-20200602104413516.png)

### 1.6 Meta

![image-20200602110909589](../images/image-20200602110909589.png)

![image-20200602134051909](../images/image-20200602134051909.png)

## 2 UFUNCTION

### 2.1 BlueprintCallable

让函数在蓝图中可调用。

### 2.2 BlueprintImplementableEvent

![image-20200602113406919](../images/image-20200602113406919.png)

但是使用此声明时，该函数无法进行默认实现，系统的代码生成会自动产生生成代码

### 2.3 BlueprintNativeEvent

![](../images/image-20200602115114622.png)

在.h 中声明：

![image-20200602133329772](../images/image-20200602133329772.png)

在.cpp 中 实现：

![image-20200602133413770](../images/image-20200602133413770.png)

点击名称可以直接查看：

![image-20200602115552945](../images/image-20200602115552945.png)



创建一个该对象的子类，他就可以重写此方法：

![image-20200602140841271](../images/image-20200602140841271.png)

### 2.4 BlueprintPure

让当前的 C++ 函数变为纯函数

![image-20200602134556838](../images/image-20200602134556838.png)

### 2.5 Category

 在蓝图上使用分类：

![image-20200602134904314](../images/image-20200602134904314.png)

在c++ 中使用分类：

![image-20200602134931154](../images/image-20200602134931154.png)

此功能也可以在类中进行分类：

### 2.6 Meta(元数据)

* DisplayName
* ToolTip
* Keywords: 可以通过该关键字搜索到该函数

在蓝图中的对应功能

![image-20200602135717678](../images/image-20200602135717678.png)



## 3 UPROPERTY

![image-20200602143901768](../images/image-20200602143901768.png)

### 3.1 BlueprintReadOnly/BlueprintReadWrite

设置属性读写性质

### 3.2 AdvanceDisplay

![image-20200602144409795](../images/image-20200602144409795.png)



### 3.3 EditAnyWhere, VisibleAnyWhere,EditDefaultsOnly, VisonleDefaultOnly

![image-20200602145046267](../images/image-20200602145046267.png)

![image-20200602145625134](../images/image-20200602145625134.png)

### 3.5 Getter 和 Setter

![image-20200602151612132](../images/image-20200602151612132.png)



## 4 反射

### 4.1 获取Class 和 所有的属性

![image-20200602155327904](../images/image-20200602155327904.png)

和 Java的反射差不多，有时间去看看。