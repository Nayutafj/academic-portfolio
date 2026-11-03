# 无人机集群自主导航避障及路径规划研究

本仓库保存大一年度项目《无人机集群自主导航避障及路径规划研究》的代码快照与结题材料。项目从二维多无人机协同避障和路径规划仿真出发，进一步探索基于深度信息的三维导航与避障。

## 项目内容

- **二维仿真：**基于浙江大学 [ZJU-FAST-Lab](https://github.com/ZJU-FAST-Lab) 的开源工作，学习并复现多无人机路径规划与协同避障实验，在 Ubuntu 和 Windows 环境中进行部署与测试。
- **三维探索：**尝试从场景图像构建环境信息，随后在 Unity 仿真环境中使用虚拟深度摄像头获取深度图，通过坐标变换生成三维点云。
- **阶段性成果：**完成二维环境中的多无人机协同避障实验，并在 Unity 中完成单架无人机基于深度信息的初步三维导航与避障验证。三维集群协同仍是后续可扩展的方向。

## 代码与结题材料

- [ROS/catkin 项目代码及来源说明](uav-project-code/README.md)
- [结题报告（公开版）](documents/UAV-project-report-redacted.pdf)
- [结题答辩 PPT](documents/UAV-project-presentation.pptx)

代码目录主要对应 ROS 仿真阶段；提供的源码中没有 Unity 或 Arma 3 工程文件，三维阶段的过程与结果见结题报告和答辩 PPT。代码以 [EGO-Planner-v2 / Swarm Playground](https://github.com/ZJU-FAST-Lab/EGO-Planner-v2) 为基础，包含上游代码及项目期间使用的配置和变动；详细来源、许可和环境说明见[代码说明](uav-project-code/README.md)。
