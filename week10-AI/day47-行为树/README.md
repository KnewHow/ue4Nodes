# 行为树

![image-20200707103757904](./images/image-20200707103757904.png)

选择黑板资源：

![image-20200707104007680](./images/image-20200707104007680.png)

实例同步：

![image-20200707104200167](./images/image-20200707104200167.png)

在AI控制器中执行行为树：

![image-20200707110216322](./images/image-20200707110216322.png)

## 1 Composite

实现多种组合

![image-20200707105510486](./images/image-20200707105510486.png)

### 1.1 Selector

选择执行，只要有一个执行成功， Selector 就成功了

![image-20200707104819988](./images/image-20200707104819988.png)

### 1.2 Sequence

依次执行，全部成功Sequence 才成功，自动闭环。

![image-20200707104857755](./images/image-20200707104857755.png)

### 1.3 Parallel

![image-20200707105128375](./images/image-20200707105128375.png)

## 2 Task

https://docs.unrealengine.com/zh-CN/Engine/ArtificialIntelligence/BehaviorTrees/BehaviorTreeNodeReference/BehaviorTreeNodeReferenceTasks/index.html

具体的执行操作

![image-20200707105551506](./images/image-20200707105551506.png)

### 2.1 创建自定义的Task

![image-20200707111114416](./images/image-20200707111114416.png)

![image-20200707111132610](./images/image-20200707111132610.png)

可重载的函数：

![image-20200707111222102](./images/image-20200707111222102.png)



### 2.2 指定使用黑板中的变量

![image-20200707112334931](./images/image-20200707112334931.png)

### 2.3 向黑板中更新数据

首先实现一个获取玩家位置的任务：

![image-20200707112427115](./images/image-20200707112427115.png)

在执行的把`playerLocationKey`绑定到`PlayerLocation`

![image-20200707112515646](./images/image-20200707112515646.png)

## 3 BlackBoard

黑板，用于传递各个任务之间的状态。

![image-20200707112227092](./images/image-20200707112227092.png)

### 3.1 Intanced Synced

![image-20200707112626207](./images/image-20200707112626207.png)



### 3.2 在 AI_Controller 中修改 BlackBoard 中的变量

![image-20200707141245615](./images/image-20200707141245615.png)

## 4 Decorator

https://docs.unrealengine.com/zh-CN/Engine/ArtificialIntelligence/BehaviorTrees/BehaviorTreeNodeReference/BehaviorTreeNodeReferenceDecorators/index.html

### 4.1 装饰器类型

![image-20200707141350685](./images/image-20200707141350685.png)

### 4.2 Blackboard

![image-20200707140625416](./images/image-20200707140625416.png)

#### 4.2.1 Self

![image-20200707120627506](./images/image-20200707120627506.png)

条件为 false时，立刻结束当前任务，执行下个任务。

#### 4.2.2 Lower Priority

![image-20200707120901337](./images/image-20200707120901337.png)

#### 4.2.3 Both

![image-20200707121036802](./images/image-20200707121036802.png)

#### 4.3 自定义装饰器

![image-20200707153158956](./images/image-20200707153158956.png)



## 5 服务

https://docs.unrealengine.com/zh-CN/Engine/ArtificialIntelligence/BehaviorTrees/BehaviorTreeNodeReference/BehaviorTreeNodeReferenceServices/index.html

### 5.1 创建服务

![image-20200707160840015](./images/image-20200707160840015.png)

### 5.2 添加服务器

![image-20200707160927808](./images/image-20200707160927808.png)

### 5.3 设置执行间隔

![image-20200707161044015](./images/image-20200707161044015.png)

然后服务里面的逻辑就会按照固定的时间间隔执行，前提是可以执行到对应的`装饰器`