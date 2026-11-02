# 无人机路径规划项目代码

这里保存了大一年度项目使用的 ROS/catkin 工作空间 `src`。它用于多无人机路径规划、协同避障和仿真环境的学习与复现，对应仓库首页介绍的[无人机集群自主导航避障及路径规划研究](../README.md#无人机集群自主导航避障及路径规划研究)。

## 代码来源

本地源码以浙江大学 FAST 实验室开源的 [EGO-Planner-v2 / Swarm Playground](https://github.com/ZJU-FAST-Lab/EGO-Planner-v2) 为基础，包含该项目的原有代码及本地使用的配置和代码变动。原项目采用 [GNU GPL v3](LICENSE) 许可证；仓库中的上游代码和第三方组件仍归各自作者所有。这里展示的是项目使用的代码快照，不应将整个源码目录视为个人独立编写的算法。

## 目录说明

- [`src/planner`](src/planner)：路径搜索、轨迹优化、规划管理及多机协同相关 ROS 包。
- [`src/uav_simulator`](src/uav_simulator)：无人机动力学、环境地图和传感器仿真相关 ROS 包。
- [`src/Utils`](src/Utils)：消息定义、可视化插件及其他工具。

上传时保留了源码、配置和仿真所需资源，省略了 Visual Studio 缓存、构建输出及 Python 字节码。提供的 `src` 中没有 Unity 或 Arma 3 的工程文件，因此本目录主要对应 ROS 仿真阶段；三维 Unity 阶段的内容见[结题报告](../documents/UAV-project-report-redacted.pdf)和[答辩 PPT](../documents/UAV-project-presentation.pptx)。

项目使用 ROS 1 的 catkin 工作空间。`src/CMakeLists.txt` 记录了原环境中的 ROS Melodic 路径；在其他机器上编译前，需要按本机 ROS 环境重新生成该文件，并参考[上游项目说明](https://github.com/ZJU-FAST-Lab/EGO-Planner-v2)安装依赖。本次上传仅整理公开源码，未在当前 Windows 环境重新编译。
