# ue4 材质基础

## 1 显示材质的 Shard Language

![image-20200720094942581](./images/image-20200720094942581.png)

一个学习 Shard Language 的网站：https://www.shadertoy.com/

![image-20200720095416504](./images/image-20200720095416504.png)

https://www.shadertoy.com/view/Ms2SD1

![image-20200720095508703](./images/image-20200720095508703.png)

使用 VS Code 预览：

![image-20200720095607157](./images/image-20200720095607157.png)

## 2 材质理论

### 2 .1 PBR

![image-20200720100443612](./images/image-20200720100443612.png)

### 2.2 微表面

![image-20200720100807430](./images/image-20200720100807430.png)



![image-20200720100850017](./images/image-20200720100850017.png)



![image-20200720100921119](./images/image-20200720100921119.png)



![image-20200720100934581](./images/image-20200720100934581.png)



### 2.3 能量守恒

![image-20200720101003955](./images/image-20200720101003955.png)



![image-20200720101151912](./images/image-20200720101151912.png)

![image-20200720101314881](./images/image-20200720101314881.png)

### 2.4 BRDF

![image-20200720101335965](./images/image-20200720101335965.png)

![image-20200720101416014](./images/image-20200720101416014.png)



## 3 UE4 材质

### 3.1 创建材质

![image-20200720101613925](./images/image-20200720101613925.png)



### 3.2 Render Target

![image-20200720101947603](./images/image-20200720101947603.png)

 实现动态渲染效果，用来实现在水平跑步溅起的水花。

### 3.3 材质编辑器

预览设置

![image-20200720103613968](./images/image-20200720103613968.png)

### 3.4 Detail

![image-20200720104047355](./images/image-20200720104047355.png)

 做贴画，例如弹坑：

![image-20200720104247003](./images/image-20200720104247003.png)

做皮肤的材质：

![image-20200720105329734](./images/image-20200720105329734.png)

 use Material Attribute:

![image-20200720105653083](./images/image-20200720105653083.png)

#### 3.4.1 Material Domain

![image-20200720105714532](./images/image-20200720105714532.png)

#### 3.4.2 Blend Mode

![image-20200720105833936](./images/image-20200720105833936.png)

#### 3.4.3 Shading Model

![image-20200720105950710](./images/image-20200720105950710.png)

### 3.5 基本快捷菜单栏

![image-20200720111524110](./images/image-20200720111524110.png)



## 4 材质节点

![image-20200720111757684](./images/image-20200720111757684.png)

### 4.1 UVCoord

![image-20200720112229382](./images/image-20200720112229382.png)



### 4.2 基础材质演示

![image-20200720115926596](./images/image-20200720115926596.png)

### 4.3 基本材质节点

![image-20200720120741028](./images/image-20200720120741028.png)

### 4.4 向量节点

![image-20200720121156073](./images/image-20200720121156073.png)

![image-20200720121351606](./images/image-20200720121351606.png)

### 4.5 实现 UV 缩放和平移

![image-20200720143609939](./images/image-20200720143609939.png)

![image-20200720143624668](./images/image-20200720143624668.png)

### 4.6 Rotator 旋转

![image-20200720144409256](./images/image-20200720144409256.png)

### 4.7 Custom Rotator

![image-20200720144921114](./images/image-20200720144921114.png)

按住 Ctrl 来 实现多个线条改变：

![image-20200720145123482](./images/image-20200720145123482.png)



### 4.8 Switch，If  和 Bool

![image-20200720150713162](./images/image-20200720150713162.png)

![image-20200720150813583](./images/image-20200720150813583.png)

### 4.9 Material Function

![image-20200720151609260](./images/image-20200720151609260.png)

输入参数：

![image-20200720151849512](./images/image-20200720151849512.png)

参数的类型：

![image-20200720151920070](./images/image-20200720151920070.png)

输出参数：

![image-20200720152737411](./images/image-20200720152737411.png)