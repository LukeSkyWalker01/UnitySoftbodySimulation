# SoftbodySimulation
This is a Unity softbody simulation plugin that can use both CPU and GPU for simulation. The GPU module uses [ILGPU](https://github.com/m4rs-mt/ILGPU) for simulation calculations. Currently, it implements softbody-to-softbody collision detection and softbody self-collision (there are still some issues to be resolved, such as penetration when simulating very thin objects like skin, and there is no good solution yet). This plugin provides specially processed rigid bodies (which can be moved, rotated, etc. through Unity) to interact with softbodies. In addition, softbodies can be cut using rectangles.

![image](showcase/demo1_720.gif)
![image](showcase/demo2_720.gif)
![image](showcase/demo3_720.gif)
![image](showcase/demo4_720.gif)
![image](showcase/demo5_720.gif)
![image](showcase/demo6_720.gif)

**Features:**
- XPBD (Extended Position Based Dynamics) method
- Softbody-to-softbody collision and softbody self-collision
- Interaction with custom rigid bodies
- Custom rectangle cutting
- CPU and GPU support

## Supported Unity Versions
This plugin was tested on Unity 2022.3.62f3c1 and should work on similar versions.

## Tutorials

- [bilibili](https://www.bilibili.com/video/BV1dVAzzoEjT/?vd_source=5bccc61294ff6dede8114d4ec98da810)
- [Youtube](https://www.youtube.com/watch?v=Nm7qr-_KJTg&t=20s)
- [User Registration URL](https://e.lm.virbox.com/activity/register.html?region=CN&developerGuid=32EBA82667950DCB79F6065C04E5178EE7C12912B9E186F563710EF17A9F77F460DE17929C9E236000918AE8E3967AEA)
- After registration, join QQ group 1077509080
- Or you can contact us via email (3922946025@qq.com).  

## Other Language Versions
- [Chinese README](README_zh.md)
