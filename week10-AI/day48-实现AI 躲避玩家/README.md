# 实现 AI 躲避玩家

## 1 球型监测

![image-20200708104025213](./images/image-20200708104025213.png)

## 2 实现躲猫猫

### 2.1 新建一个Actor掩体

用箭头来标识瞄点(角色可以躲藏的点)

![image-20200708173948259](./images/image-20200708173948259.png)

初始化的一些操作：

![image-20200708174134677](./images/image-20200708174134677.png)

查找可以安全的节点：

![image-20200708174350295](./images/image-20200708174350295.png)

### 2.2 发现可以躲藏的柱子

![image-20200708180904726](./images/image-20200708180904726.png)

### 2.3 移动到安全的节点

![image-20200708181128432](./images/image-20200708181128432.png)

