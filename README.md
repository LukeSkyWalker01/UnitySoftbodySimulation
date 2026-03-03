# SoftbodySimulation
这是一个unity软体模拟插件，此插件可以使用CPU和GPU两种方式进行模拟。GPU模块是使用[ILGPU](https://github.com/m4rs-mt/ILGPU)进行模拟计算的。目前实现了软体和软体碰撞检测以及软体的自碰撞（目前还有点问题没有解决，当模拟的物体太薄比如皮肤，碰撞会出现穿透现象，目前还没有很好的解决方案）。此插件提供经过特殊处理过的刚体（可以通过unity 移动旋转等）和软体进行交互。另外可以通过矩形对软体进行切割。

![image](showcase/demo1_720.gif)
![image](showcase/demo2_720.gif)
![image](showcase/demo3_720.gif)
![image](showcase/demo4_720.gif)
![image](showcase/demo5_720.gif)
![image](showcase/demo6_720.gif)

**特性:**
- XPBD (Extended Position Based Dynamics) method
- 软体之间的碰撞以及软体的自碰撞
- 和自定义刚体交互
- 自定义矩形切割
- CPU和GPU

## 支持的unity 版本
此插件在Unity2022.3.62f3c1完成测试，在同等版本下应该也可以。



## 教程

- [bilibili](https://github.com/LukeSkyWalker01/UnitySoftbodySimulation)
- [Youtube](https://github.com/LukeSkyWalker01/UnitySoftbodySimulation)
- [用户注册网址](https://e.lm.virbox.com/activity/register.html?region=CN&developerGuid=32EBA82667950DCB79F6065C04E5178EE7C12912B9E186F563710EF17A9F77F460DE17929C9E236000918AE8E3967AEA)
- 注册完成之后+QQ群1077509080，私聊群主获取授权






