[Uploading README.md…]()
# Universal Evolution Engine (UEE) - V1.0 Demo

## 项目简介
本项目是一个基于**离散非平衡动力学**的通用网络演化引擎（演示版）。
系统的核心设计遵循四大铁律：
- **无随机**：没有任何随机数生成器（RNG），演化完全确定。
- **无常量**：所有物理参数均由系统状态实时导出，无硬编码常量。
- **纯局部**：节点只与局部邻居交互，无全局矩阵运算。
- **严格守恒**：全局能量守恒误差严格限制在单精度浮点极限（1e-6）以内。

## 使用说明
1. 前往 [Releases] 页面下载最新的演示版压缩包（`UEE_V1.0_Demo.zip`）。
2. 解压后，双击 `engine.exe` 即可运行。
3. 详细使用说明及两种运行模式（文本驱动/直接控制），请参阅压缩包内的 `README.txt`。

## 开源与安全说明
出于**知识产权保护**与**防止系统被滥用于大规模网络攻击**的考量，本项目**不公开C语言核心源码**。
演示版严格限制了最大节点数为**200**。如果学者需要复现论文中的完整实验数据，请依据论文中的数学方程自行实现。

## 学术引用
如果您在学术研究中使用了本引擎，请引用以下预印本：
> *Lin, J. (2026). A Locally-Regulated Open Dynamics Framework with State-Derived Parameters: Energy Conservation and Topology-Induced Entropy Phase Transitions. Zenodo. https://doi.org/10.5281/zenodo.23062905*

## 许可协议
本项目采用 **AGPLv3** 协议（或自定义限制性协议）。允许个人学习与学术研究，**严禁任何形式的商业闭源使用、武器化系统及未经授权的网络攻击**。
