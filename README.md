# SoftbodySimulation
这是一个unity软体模拟插件，此插件可以使用CPU和GPU两种方式进行模拟。GPU模块是使用[ILGPU](https://github.com/m4rs-mt/ILGPU)进行模拟计算的。目前实现了软体和软体碰撞检测以及软体的自碰撞（目前还有点问题没有解决，当模拟的物体太薄比如皮肤，碰撞会出现穿透现象，目前还没有很好的解决方案）。此插件提供经过特殊处理过的刚体（可以通过unity 移动旋转等）和软体进行交互。另外可以通过矩形对软体进行切割。

![obstacle_course](/showcase/obstacle_course.gif)
![skinning_vs_particles](/showcase/skinning_vs_particles.gif)

**Features:**
- PBD (Position Based Dynamics) method
- Soft-bodies from mesh and point data
- Box constraints (boundary or obstacle)
- Plane constraints
- Shape matching constraints (rigid, soft linear, soft quadratic)
- Cluster shape matching
- Mesh skinning according to particle positions
- Particle collisions
- Friction
- Different scenarios
- Particle dragging

## Build Instructions
For Visual Studio 2019:
```
git clone https://github.com/GitDaroth/SoftbodySimulation
cd SoftbodySimulation
cmake_generate_VS2019.bat
```
Open the generated Visual Studio solution in the "build" folder and build the "SoftbodySimulation" target.

Don't forget to copy the needed dll files from your Qt5 installation next to your executable:
```
QT5_INSTALLATION_PATH/bin/Qt5Core.dll
QT5_INSTALLATION_PATH/bin/Qt5Gui.dll
QT5_INSTALLATION_PATH/bin/Qt5Widgets.dll
QT5_INSTALLATION_PATH/plugins/platforms/qwindows.dll
QT5_INSTALLATION_PATH/plugins/styles/qwindowsvistastyle.dll
QT5_INSTALLATION_PATH/plugins/imageformats/qjpeg.dll
```

## Dependencies
**SoftbodyPhysics:**
- [Qt5 (Modules: Core, Gui)](https://www.qt.io)
- [CUDA](https://developer.nvidia.com/cuda-downloads)
- [Eigen](https://github.com/libigl/eigen)
- [unsupported/Eigen](https://github.com/libigl/eigen/tree/master/unsupported)
- [tinyobjectloader](https://github.com/tinyobjloader/tinyobjloader)

**SoftbodySimulation:**
- SoftbodyPhysics
- [Qt5 (Modules: Widgets)](https://www.qt.io)
