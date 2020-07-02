# 过场动画

![image-20200702103417330](./images/image-20200702103417330.png)

## 1 第一幕过场动画

选定一个模型：

![image-20200702111801039](./images/image-20200702111801039.png)

添加到动画轨道中：

![image-20200702111830407](./images/image-20200702111830407.png)

添加一个模型的动画：

![image-20200702111900348](./images/image-20200702111900348.png)

设置模型的位置：

![image-20200702111947056](./images/image-20200702111947056.png)

在场景中添加影视摄像机，并添加到动画轨迹中：

![image-20200702112103211](./images/image-20200702112103211.png)

给摄像机添加位移：

![image-20200702112239308](./images/image-20200702112239308.png)

按下S键打上关键帧：

![image-20200702112302387](./images/image-20200702112302387.png)

可以调整摄像机的参数配置：

![image-20200702112742460](./images/image-20200702112742460.png)

动画混合：

![image-20200702113514656](./images/image-20200702113514656.png)

![image-20200702113529517](./images/image-20200702113529517.png)

帧速率调整：

![image-20200702113748497](./images/image-20200702113748497.png)

播放玩保持动作：

![image-20200702114139535](./images/image-20200702114139535.png)

## 2 Master Sequence

一个可以包含多个子镜头的过程动画，在创建的时候可以选择`Number of Shots`

![image-20200702115704979](./images/image-20200702115704979.png)

![image-20200702122545343](./images/image-20200702122545343.png)

![image-20200702115941777](./images/image-20200702115941777.png)

在子Sequencer中需要选定摄像机，添加快照：

![image-20200702122725656](./images/image-20200702122725656.png)

## 3 Squence

合并两个子动画

![image-20200702142918209](./images/image-20200702142918209.png)

驾驶摄像机：

![image-20200702143043077](./images/image-20200702143043077.png)

## 4 Take

![image-20200702143226090](./images/image-20200702143226090.png)

一个Sequence的多个版本，用于切换。

## 5 相机轨道

![image-20200702151522384](./images/image-20200702151522384.png)

相机追踪对象：

![image-20200702151754239](./images/image-20200702151754239.png)

## 6 摄像机摇臂

![image-20200702152841470](./images/image-20200702152841470.png)

https://docs.unrealengine.com/zh-CN/Engine/Sequencer/HowTo/CameraRigCrane/index.html

## 7 事件轨

可以用来调用蓝图事件一种轨道。

将 Actor 添加到sequence中

![image-20200702155202641](./images/image-20200702155202641.png)

给 Actor 添加事件轨：

![image-20200702155236139](./images/image-20200702155236139.png)

绑定蓝图中对应的事件：

![image-20200702155109450](./images/image-20200702155109450.png)

添加关键帧：

![image-20200702155341710](./images/image-20200702155341710.png)

添加后的样子：

![image-20200702155430148](./images/image-20200702155430148.png)

将 Sequence 拖到场景中，让他自动播放：

![image-20200702155519766](./images/image-20200702155519766.png)

## 8 播放动画

![image-20200702160616074](./images/image-20200702160616074.png)

### 8.1 动画导出

![image-20200702160714001](./images/image-20200702160714001.png)



### 8.2 添加水印

![image-20200702160825605](./images/image-20200702160825605.png)

### 8.2 Sequencer 动态绑定

![image-20200702163333476](./images/image-20200702163333476.png)



### 8.3 Sequencer Record

一个录制过场动画的方式

![image-20200702163909014](./images/image-20200702163909014.png)

![image-20200702163513272](./images/image-20200702163513272.png)

### 8.4 播放设置

![image-20200702165749760](./images/image-20200702165749760.png)

### 8.5 摄像机聚焦

![image-20200702165908621](./images/image-20200702165908621.png)