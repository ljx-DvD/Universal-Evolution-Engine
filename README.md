# Universal Evolution Engine (UEE) — V1.0 Demo

## 项目简介

本项目是一个基于**离散非平衡动力学**的通用网络演化引擎（演示版）。四条设计原则：

- **无随机**：不含任何随机数生成器（RNG），演化完全确定。
- **无常量**：物理参数由系统状态实时导出。实现中保留的 5 个固定无量纲系数已在论文 v2 中逐项列出与分类。
- **严格守恒**：离散记账下精确；演示版为单精度实现，控制台打印的守恒偏差约 1e-6。
- **纯局部**：**V1.0 演示版为平均场实现**（参数每拍由全图统计导出并共用）。局部化调节机制见后续工作。

## 使用说明

1. 前往 [Releases] 页面下载演示版压缩包（`UEE_V1.0_Demo.zip`）。
2. 解压后，双击 `engine.exe` 即可运行。
3. 两种运行模式（文本驱动 / 直接控制）与输入文件格式，见压缩包内 `README.txt`。

## 开源说明

出于知识产权保护，本项目**不公开 C 语言核心源码**。演示版限制最大节点数为 **200**；
如需复现论文中的完整实验，请依据论文给出的方程自行实现。

## 学术引用

> Lin, J. (2026). A Locally-Regulated Open Dynamics Framework with State-Derived Parameters:
> Energy Conservation and Topology-Induced Entropy Phase Transitions.
> Zenodo. https://doi.org/10.5281/zenodo.23062905

## 许可协议

**专有软件（Proprietary）。保留所有权利。**

- **允许**：个人学习、非商业学术研究、论文复现与引用。
- **禁止**：商业使用、再分发、逆向工程、以本项目为基础制作衍生产品。
- 商业授权与合作请联系作者。
