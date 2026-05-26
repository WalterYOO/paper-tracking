# 3D Gaussian Splatting 论文跟踪

> 2026年5月

> 注：★ 表示被顶会录用。

## 目录

| 日期 | 论文 | arXiv | 类别 | 概述 |
|------|------|-------|------|------|
| 2026-05-18 | [PanoWorld](#1-panoworld-a-generative-spatial-world-model-for-consistent-whole-house-panorama-synthesis) | [2605.17916](https://arxiv.org/abs/2605.17916) | cs.CV | 自回归全屋全景生成，3DGS 作为空间记忆缓存 |
| 2026-05-17 | [GEM](#1-gem-gaussian-evolution-model-for-occupancy-forecasting-and-motion-planning) | [2605.17682](https://arxiv.org/abs/2605.17682) | cs.CV | 非自回归 4D Gaussian 世界模型，自动驾驶占用预测与规划 |
| 2026-05-16 | ★ **[P2GS](#3-p2gs-physical-prior-guided-gaussian-splatting-for-photometrically-consistent-urban-reconstruction)** | [2605.16925](https://arxiv.org/abs/2605.16925) | cs.CV | 物理先引导光度一致重建，解决跨视角曝光不一致（CVPR'26） |
| 2026-05-13 | ★ **[Z-Order Transformer](#5-z-order-transformer-for-feed-forward-gaussian-splatting)** | [2605.13465](https://arxiv.org/abs/2605.13465) | cs.CV | Z 序稀疏注意力，单次前向预测属性（CVPR'26 Oral） |
| 2026-05-02 | ★ **[SplAttN](#1-splatttn-bridging-2d-and-3d-with-gaussian-soft-splatting-and-attention-for-point-cloud-completion)** | [2605.01466](https://arxiv.org/abs/2605.01466) | cs.CV | 高斯软光栅化替代硬投影，点云补全（ICML'26 Spotlight） |

## 2026-05-18

### 1. PanoWorld: A Generative Spatial World Model for Consistent Whole-House Panorama Synthesis

- **arXiv**: [2605.17916](https://arxiv.org/abs/2605.17916)
- **作者**: Jinrang Jia, Zhenjia Li, Yijiang Hu, Yifeng Shi
- **类别**: cs.CV

**摘要**: 从平面图和风格参考生成一致的全屋 VR 漫游，需要照片级真实感和跨视角空间一致性。纯 2D 生成器在视角变化时会重新想象几何和材质，而整体式 3D 生成在 multi-room 尺度下又昂贵且丢失细节纹理。PanoWorld 将全屋合成视为自回归的节点式 360 度全景图生成，利用 floorplan 派生的 3D shell 作为全局几何代理，动态 3DGS cache 作为可渲染的空间记忆。通过 Room-aware Group Attention 抑制跨房间特征干扰，拓扑感知渐进式缓存策略融合局部更新。

---

## 2026-05-17

### 1. GEM: Gaussian Evolution Model for Occupancy Forecasting and Motion Planning

- **arXiv**: [2605.17682](https://arxiv.org/abs/2605.17682)
- **作者**: Cheng Chen, Hao Huang, Saurabh Bagchi
- **类别**: cs.CV

**摘要**: 面向自动驾驶的占用预测与运动规划。GEM 为非自回归的 4D Gaussian 世界模型，场景表示为连续时间的高斯基元并学习其动力学。相比固定步长自回归生成，GEM 可在任意时间戳直接查询并 splat 为语义占用体，支持灵活的时间查询和运动规划，在多项任务上达到 SOTA。

---

## 2026-05-16

### 3. P2GS: Physical Prior-guided Gaussian Splatting for Photometrically Consistent Urban Reconstruction

- **arXiv**: [2605.16925](https://arxiv.org/abs/2605.16925)
- **作者**: Kota Shimomura, Hidehisa Arai, Tsubasa Takahashi, Takayoshi Yamashita, Hironobu Fujiyoshi
- **类别**: cs.CV
- **备注**: CVPR 2026 main 录用

**摘要**: 面向自动驾驶的城市场景重建，解决 3DGS 在异构相机管线和动态光照下的光度不一致问题。从 LDR 图像联合分解视图不变 HDR 辐射场、每视角曝光增益和色调映射函数，在多种场景中显著提升跨视角光度一致性。

---

## 2026-05-13

### 5. Z-Order Transformer for Feed-Forward Gaussian Splatting

- **arXiv**: [2605.13465](https://arxiv.org/abs/2605.13465)
- **作者**: Can Wang, Lei Liu, Wei Jiang, Dong Xu
- **类别**: cs.CV
- **备注**: CVPR 2026 Oral 录用

**摘要**: 传统 3DGS 优化缓慢，前向方法虽快但基元冗余且质量不足。本文设计基于 Transformer 的架构，利用 Z 序曲线将无序高斯集组织为空间连贯序列，通过稀疏注意力捕捉高斯间关系并自适应抑制冗余。单次前向即可用更少基元预测高质量属性。

---

## 2026-05-02

### 1. SplAttN: Bridging 2D and 3D with Gaussian Soft Splatting and Attention for Point Cloud Completion

- **arXiv**: [2605.01466](https://arxiv.org/abs/2605.01466)
- **作者**: Zhaoyang Li, Zhichao You, Tianrui Li
- **类别**: cs.CV, cs.LG
- **备注**: ICML 2026 Spotlight 录用

**摘要**: 多模态点云补全中，标准硬投影将稀疏点云投影到图像平面产生极稀疏支撑，导致跨模态熵崩溃。SplAttN 用可微高斯光栅化替代硬投影，产生密集连续的图像平面表示，将投影 reformulate 为连续密度估计，避免崩溃的稀疏支撑并改善跨模态连接可学习性。在 PCN 和 ShapeNet-55/34 上达到 SOTA，KITTI 基准上保持对视觉线索的稳健依赖。

---
