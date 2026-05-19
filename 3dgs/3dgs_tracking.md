# 3D Gaussian Splatting 论文跟踪

## 目录

| 日期 | 论文 | arXiv | 类别 | 简述 |
|------|------|-------|------|------|
| 2026-05-18 | [PanoWorld](#1-panoworld-a-generative-spatial-world-model-for-consistent-whole-house-panorama-synthesis) | [2605.17916](https://arxiv.org/abs/2605.17916) | cs.CV | 自回归全屋全景生成，3DGS 作为空间记忆缓存 |
| 2026-05-18 | [TensorGS](#2-accelerating-3d-gaussian-splatting-using-tensor-cores-tensorgs) | [2605.17855](https://arxiv.org/abs/2605.17855) | cs.GR | Tensor Core 加速 3DGS 光栅化，渲染提速 1.65x |
| 2026-05-18 | [LiteLoc](#3-efficient-sparse-to-dense-visual-localization-via-compact-gaussian-scene-representation-and-accelerated-dense-pose-estimation-liteloc) | [2605.17777](https://arxiv.org/abs/2605.17777) | cs.CV | 去除颜色场减 94% 存储，PnP 蒸馏提速 19x |
| 2026-05-17 | [GEM](#1-gem-gaussian-evolution-model-for-occupancy-forecasting-and-motion-planning) | [2605.17682](https://arxiv.org/abs/2605.17682) | cs.CV | 非自回归 4D Gaussian 世界模型，自动驾驶占用预测与规划 |
| 2026-05-16 | [Topo-GS](#1-topo-gs-continuous-volumetric-embedding-of-high-dimensional-data-via-topological-gaussian-splatting) | [2605.17011](https://arxiv.org/abs/2605.17011) | cs.GR | 将 3DGS 用于降维可视化，离散散点图→连续体表示 |
| 2026-05-16 | [DSGS](#2-a-single-atlas-is-all-you-need-decoder-side-gaussian-splatting-for-immersive-video) | [2605.17002](https://arxiv.org/abs/2605.17002) | cs.GR | 解码端前向 3DGS 替代深度估计，沉浸式视频带宽大幅降低 |
| 2026-05-16 | [P2GS](#3-p2gs-physical-prior-guided-gaussian-splatting-for-photometrically-consistent-urban-reconstruction) | [2605.16925](https://arxiv.org/abs/2605.16925) | cs.CV | 物理先引导光度一致重建，解决跨视角曝光不一致（CVPR'26） |

## 2026-05-18

### 1. PanoWorld: A Generative Spatial World Model for Consistent Whole-House Panorama Synthesis

- **arXiv**: [2605.17916](https://arxiv.org/abs/2605.17916)
- **作者**: Jinrang Jia, Zhenjia Li, Yijiang Hu, Yifeng Shi
- **类别**: cs.CV

**摘要**: 从平面图和风格参考生成一致的全屋 VR 漫游，需要照片级真实感和跨视角空间一致性。纯 2D 生成器在视角变化时会重新想象几何和材质，而整体式 3D 生成在 multi-room 尺度下又昂贵且丢失细节纹理。PanoWorld 将全屋合成视为自回归的节点式 360 度全景图生成，利用 floorplan 派生的 3D shell 作为全局几何代理，动态 3DGS cache 作为可渲染的空间记忆。通过 Room-aware Group Attention 抑制跨房间特征干扰，拓扑感知渐进式缓存策略融合局部更新。

---

### 2. Accelerating 3D Gaussian Splatting using Tensor Cores (TensorGS)

- **arXiv**: [2605.17855](https://arxiv.org/abs/2605.17855)
- **作者**: Sheng Li, Yang Sui, Yue Wu, Zhuoran Song, Bo Yuan, Xulong Tang, Yue Dai
- **类别**: cs.GR

**摘要**: 3DGS 已成为实时神经渲染和 3D 场景重建的主流技术，但渲染成本在延迟敏感场景下仍然过高。Rasterization 阶段占据了渲染时间的主体，而现有 3DGS 系统完全在 CUDA cores 上运行，Tensor Cores 处于闲置状态。作者发现 3DGS 在 FP16 下运行几乎无损画质。TensorGS 将 rasterization 计算张量化为 Tensor Core 兼容的矩阵运算，并引入跨 tile 分组提高 Gaussian 复用率。实验显示端到端渲染性能提升 1.65 倍且保持图像质量。

---

### 3. Efficient Sparse-to-Dense Visual Localization via Compact Gaussian Scene Representation and Accelerated Dense Pose Estimation (LiteLoc)

- **arXiv**: [2605.17777](https://arxiv.org/abs/2605.17777)
- **作者**: Zizhuo Li, Songchu Deng, Linfeng Tang, Jiayi Ma
- **类别**: cs.CV

**摘要**: 基于 3DGS 的高效稀疏到密集视觉定位器。前序 SOTA 方法 STDLoc 定位能力强但存在严重存储冗余和计算延迟。LiteLoc 提出两项改进：（1）去除 3DGS 中对定位无用的颜色场，构建紧凑的高斯场景表示，消除约 94% 冗余存储；（2）将密集 PnP 求解中的匹配点蒸馏为 5% 代表性子集，实现近 19 倍速度提升。在多个场景中超越 STDLoc，同时大幅降低存储和计算开销。

---

## 2026-05-17

### 1. GEM: Gaussian Evolution Model for Occupancy Forecasting and Motion Planning

- **arXiv**: [2605.17682](https://arxiv.org/abs/2605.17682)
- **作者**: Cheng Chen, Hao Huang, Saurabh Bagchi
- **类别**: cs.CV

**摘要**: 面向自动驾驶的占用预测与运动规划。GEM 为非自回归的 4D Gaussian 世界模型，场景表示为连续时间的高斯基元并学习其动力学。相比固定步长自回归生成，GEM 可在任意时间戳直接查询并 splat 为语义占用体，支持灵活的时间查询和运动规划，在多项任务上达到 SOTA。

---

## 2026-05-16

### 1. Topo-GS: Continuous Volumetric Embedding of High-Dimensional Data via Topological Gaussian Splatting

- **arXiv**: [2605.17011](https://arxiv.org/abs/2605.17011)
- **作者**: João Paulo Gois, Luis Gustavo Nonato
- **类别**: cs.GR, cs.CV, cs.LG

**摘要**: 将 3DGS 复用于降维可视化，把高维数据投影转化为无网格的体素重建过程。通过正交 Procrustes 优化和拓扑感知策略，将离散散点图转换为连续体表示，同时保持局部拓扑保真度。

---

### 2. A Single Atlas is All You Need: Decoder-Side Gaussian Splatting for Immersive Video

- **arXiv**: [2605.17002](https://arxiv.org/abs/2605.17002)
- **作者**: Dawid Mieloch, Stuart Perry
- **类别**: cs.GR, cs.MM, eess.IV

**摘要**: 提出 DSGS，在解码端用前向 3DGS 推断替代传统深度估计来生成沉浸式视频。发现有损压缩能作为隐式低通滤波器稳定 splat 预测，仅用 4 个输入视图即可比 DSDE 基线提升 +5.79 dB BD-PSNR。

---

### 3. P2GS: Physical Prior-guided Gaussian Splatting for Photometrically Consistent Urban Reconstruction

- **arXiv**: [2605.16925](https://arxiv.org/abs/2605.16925)
- **作者**: Kota Shimomura, Hidehisa Arai, Tsubasa Takahashi, Takayoshi Yamashita, Hironobu Fujiyoshi
- **类别**: cs.CV
- **备注**: CVPR 2026 main 录用

**摘要**: 面向自动驾驶的城市场景重建，解决 3DGS 在异构相机管线和动态光照下的光度不一致问题。从 LDR 图像联合分解视图不变 HDR 辐射场、每视角曝光增益和色调映射函数，在多种场景中显著提升跨视角光度一致性。

