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
| 2026-05-15 | [Prior-Guided 3DGS Segmentation](#1-robust-prior-guided-segmentation-for-editable-3d-gaussian-splatting) | [2605.16065](https://arxiv.org/abs/2605.16065) | cs.CV | SAM-HQ 生成 2D 掩码，先验引导的多视角一致 3D 分割 |
| 2026-05-15 | [ArtMesh](#2-artmesh-part-aware-articulated-mesh-fields-with-motion-consistent-dynamics) | [2605.16582](https://arxiv.org/abs/2605.16582) | cs.CV | 网格原生关节物体重建，超越 3DGS 散点基线 |
| 2026-05-15 | [Learn2Splat](#3-learn2splat-extending-the-horizon-of-learned-3dgs-optimization) | [2605.15760](https://arxiv.org/abs/2605.15760) | cs.CV | 元学习扩展 3DGS 学习型优化器到更长优化周期 |
| 2026-05-14 | [Eff-WRFGS](#1-eff-wrfgs-efficient-wireless-radiance-field-using-3d-gaussian-splatting) | [2605.15324](https://arxiv.org/abs/2605.15324) | eess.SP | 可学习掩码裁剪高斯基元，无线信道建模存储减 44x |
| 2026-05-14 | [AV1 Motion Vector for 3DGS](#2-efficient-dense-matching-for-enhanced-gaussian-splatting-using-av1-motion-vectors) | [2605.14629](https://arxiv.org/abs/2605.14629) | eess.IV | AV1 运动向量替代穷举匹配，SfM 特征点增 8 倍 |
| 2026-05-14 | [Denoising-GS](#3-denoising-gs-gaussian-splatting-with-spatial-aware-denoising) | [2605.14880](https://arxiv.org/abs/2605.14880) | cs.CV | 将 3DGS 优化建模为空间感知去噪过程，SOTA |
| 2026-05-14 | [3DEditSafe](#4-3d-editsafe-defending-3d-editing-pipelines-from-unsafe-generation) | [2605.15398](https://arxiv.org/abs/2605.15398) | cs.GR | 3DGS 文本驱动编辑中的不安全生成防御 |
| 2026-05-14 | [Skew-Normal Splatting](#5-3d-skew-normal-splatting) | [2605.15010](https://arxiv.org/abs/2605.15010) | cs.CV | Azzalini 偏态正态分布替代高斯核，灵活建模不对称边界 |
| 2026-05-13 | [PanoPlane](#1-panoplane-plane-aware-panoramic-completion-for-sparse-view-indoor-3d-gaussian-splatting) | [2605.14135](https://arxiv.org/abs/2605.14135) | cs.CV | 平面感知全景补全，3 视图即可 SOTA 新视角合成 |
| 2026-05-13 | [HarmoGS](#2-harmogs-robust-3d-gaussian-splatting-in-the-wild-via-conflict-aware-gradient-harmonization) | [2605.13073](https://arxiv.org/abs/2605.13073) | cs.CV | 冲突感知梯度调和，解决野生场景跨视角不一致 |
| 2026-05-13 | [GuardMarkGS](#3-guardmarkgs-unified-ownership-tracing-and-edit-deterrence-for-3d-gaussian-splatting) | [2605.12919](https://arxiv.org/abs/2605.12919) | cs.CV | 统一水印追踪与编辑威慑，3DGS 版权保护 |
| 2026-05-13 | [RoSplat](#4-rosplat-robust-feed-forward-pixel-wise-gaussian-splatting-for-varying-input-views-and-high-resolution-rendering) | [2605.13093](https://arxiv.org/abs/2605.13093) | cs.CV | 前向像素级 3DGS，alpha 归一化修复变亮问题 |
| 2026-05-13 | [Z-Order Transformer for 3DGS](#5-z-order-transformer-for-feed-forward-gaussian-splatting) | [2605.13465](https://arxiv.org/abs/2605.13465) | cs.CV | Z 序稀疏注意力，单次前向预测属性（CVPR'26 Oral） |
| 2026-05-13 | [SCOUP](#6-sparse-code-uplifting-for-efficient-3d-language-gaussian-splatting) | [2605.13600](https://arxiv.org/abs/2605.13600) | cs.CV | 稀疏码本提升，3D 语言高斯训练提速 400x |
| 2026-05-12 | [XFreq-GS](#1-xfreq-gs-cross-frequency-wireless-radiation-field-reconstruction-with-3d-gaussian-splatting) | [2605.11432](https://arxiv.org/abs/2605.11432) | eess.SP | 共享几何+频率自适应属性，跨频率无线信道建模 |
| 2026-05-12 | [PointGS](#2-pointgs-semantic-consistent-unsupervised-3d-point-cloud-segmentation-with-3d-gaussian-splatting) | [2605.11520](https://arxiv.org/abs/2605.11520) | cs.CV | 3DGS 桥接 2D-3D 语义迁移，无监督点云分割（CVPR'26） |
| 2026-05-12 | [Retrospective Dynamic NVS](#3-3d-gaussian-splatting-for-efficient-retrospective-dynamic-scene-novel-view-synthesis-with-a-standardized-benchmark) | [2605.12437](https://arxiv.org/abs/2605.12437) | cs.CV | 同步多视图下无需时间耦合约束的动态场景重建（CVPR'26） |
| 2026-05-12 | [3DGS³](#4-3dgs-cubed-joint-super-sampling-and-frame-interpolation-for-real-time-large-scale-3dgs-rendering) | [2605.11489](https://arxiv.org/abs/2605.11489) | cs.GR | 后处理超采样+帧插值，统一高效渲染 |
| 2026-05-12 | [PoseCompass](#5-posecompass-intelligent-synthetic-pose-selection-for-visual-localization) | [2605.12144](https://arxiv.org/abs/2605.12144) | cs.CV | 3DGS 合成位姿智能筛选，APR 微调提速 3x |
| 2026-05-12 | [PointForward](#6-pointforward-feedforward-driving-reconstruction-through-point-aligned-representations) | [2605.11594](https://arxiv.org/abs/2605.11594) | cs.CV | 空间稀疏查询替代像素对齐，前向驾驶场景重建 |
| 2026-05-12 | [PairDropGS](#7-pairdropgs-paired-dropout-induced-consistency-regularization-for-sparse-view-gaussian-splatting) | [2605.12072](https://arxiv.org/abs/2605.12072) | cs.CV | 成对 Dropout 一致性正则化，稀疏视角重建 |
| 2026-05-12 | [GeoQuery](#8-geoquery-geometry-query-diffusion-for-sparse-view-reconstruction) | [2605.12399](https://arxiv.org/abs/2605.12399) | cs.CV | 几何引导扩散模型修复严重伪像（SIGGRAPH'26） |
| 2026-05-11 | [PG-3DGS](#1-pg-3dgs-optimizing-3d-gaussian-splatting-to-satisfy-physics-objectives) | [2605.11266](https://arxiv.org/abs/2605.11266) | cs.CV | 可微物理模拟引导形状优化，3D 结构兼具物理功能 |
| 2026-05-11 | [AdaptSplat](#2-adaptsplat-adapting-vision-foundation-models-for-feed-forward-3d-gaussian-splatting) | [2605.10239](https://arxiv.org/abs/2605.10239) | cs.CV | 仅 1.5M 参数的频率保持适配器，前向 3DGS SOTA |
| 2026-05-11 | [SDTalk](#3-sdtalk-structured-facial-priors-and-dual-branch-motion-fields-for-generalizable-gaussian-talking-head-synthesis) | [2605.09956](https://arxiv.org/abs/2605.09956) | cs.CV | 单帧可泛化 3DGS 说话人头合成 |
| 2026-05-11 | [DySurface](#4-dysurface-consistent-4d-surface-reconstruction-via-bridging-explicit-gaussians-and-implicit-functions) | [2605.10360](https://arxiv.org/abs/2605.10360) | cs.CV | 显式高斯+隐式 SDF 桥接，动态场景连续表面重建 |
| 2026-05-11 | [MAGS-SLAM](#5-mags-slam-monocular-multi-agent-gaussian-splatting-slam-for-geometrically-and-photometrically-consistent-reconstruction) | [2605.10760](https://arxiv.org/abs/2605.10760) | cs.RO | 仅 RGB 的多智能体 3DGS SLAM 协同重建 |
| 2026-05-11 | [VEGA](#6-vega-visual-encoder-grounding-alignment-for-spatially-aware-vision-language-action-models) | [2605.10485](https://arxiv.org/abs/2605.10485) | cs.RO | 3DGS 监督的 DINOv2-FiT3D 对齐 VLA 空间感知 |

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

---

## 2026-05-15

### 1. Robust Prior-Guided Segmentation for Editable 3D Gaussian Splatting

- **arXiv**: [2605.16065](https://arxiv.org/abs/2605.16065)
- **作者**: Raushan Joshi, Jean-Yves Guillemaut
- **类别**: cs.CV, cs.AI
- **备注**: IEEE ICIP 2026 录用

**摘要**: 3DGS 支持实时重建但缺乏鲁棒分割以支持编辑操作。现有从 2D 提升的方法存在视角不一致问题。本文利用 SAM-HQ 生成高精度 2D 掩码，提出先验引导的标签重分配方法，通过多视角一致性将标签分配给 3D Gaussians，实现实时交互式物体编辑，边界保持效果优于现有方法。

---

### 2. ArtMesh: Part-Aware Articulated Mesh Fields with Motion-Consistent Dynamics

- **arXiv**: [2605.16582](https://arxiv.org/abs/2605.16582)
- **作者**: Sylvia Yuan, Dan Wang, Ravi Ramamoorthi, Xinrui Cui
- **类别**: cs.CV

**摘要**: 面向关节物体的网格原生重建方法。3DGS 的散点几何缺乏表面拓扑，不利于关节运动推理。ArtMesh 基于网格可微渲染，引入感知部件的 Delaunay 重网格化，生成不跨越语义边界的子网格。通过双向顶点级和像素级运动一致性优化关节参数。在自建 Articulate-100 基准上，关节参数估计和几何重建均超越 3DGS 基线。

---

### 3. Learn2Splat: Extending the Horizon of Learned 3DGS Optimization

- **arXiv**: [2605.15760](https://arxiv.org/abs/2605.15760)
- **作者**: Naama Pearl, Stefano Esposito, Haofei Xu, Amit Peleg et al.
- **类别**: cs.CV

**摘要**: 3DGS 优化通常使用 Adam 等通用优化器，无法捕捉参数间结构和空间关系，导致收敛缓慢。学习型优化器虽有改进，但仅在固定迭代次数内有效。Learn2Splat 通过元学习、检查点缓冲区和优化器 rollout 策略，将优化器扩展到更长优化周期而不退化。同时在零样本泛化到未见设置上取得良好效果。

---

## 2026-05-14

### 1. Eff-WRFGS: Efficient Wireless Radiance Field Using 3D Gaussian Splatting

- **arXiv**: [2605.15324](https://arxiv.org/abs/2605.15324)
- **作者**: Chenghong Bian, Meng Hua, Deniz Gunduz
- **类别**: eess.SP

**摘要**: 将 3DGS 应用于无线信道辐射场建模。为每个高斯基元引入可学习掩码以指示其重要性，指导裁剪不重要的基元。训练时使用渲染损失和正则化损失的加权和，在 NeRF² 数据集上实现 44 倍存储降低和 7 倍渲染加速，质量仅有轻微下降。

---

### 2. Efficient Dense Matching for Enhanced Gaussian Splatting Using AV1 Motion Vectors

- **arXiv**: [2605.14629](https://arxiv.org/abs/2605.14629)
- **作者**: Julien Zouein, Vibhoothi Vibhoothi, François Pitié, Anil Kokaram
- **类别**: eess.IV, cs.CV

**摘要**: 3DGS 重建质量高度依赖初始点云。SfM 管线成本高且在无纹理区域稀疏。本文利用 AV1 视频编解码器内置的运动向量替代 COLMAP 的穷举匹配，产生密集 8 倍的点云，VMAF 提升 9 点，训练时间平均减少 63%。

---

### 3. Denoising-GS: Gaussian Splatting with Spatial-aware Denoising

- **arXiv**: [2605.14880](https://arxiv.org/abs/2605.14880)
- **作者**: Qingyuan Zhou, Xinyi Liu, Weidong Yang, Ning Wang et al.
- **类别**: cs.CV, cs.GR, cs.LG

**摘要**: 3DGS 优化不可避免地引入噪声基元。现有方法仅调整位置而忽略空间结构。Denoising-GS 将优化建模为去噪过程，提出空间感知去噪框架：保持空间优化流的优化器、空间梯度去噪策略、不确定性去噪模块裁剪冗余基元、空间连贯性细化策略在稀疏区域选择性分裂基元。在三项基准数据集上达到 SOTA。

---

### 4. 3DEditSafe: Defending 3D Editing Pipelines from Unsafe Generation

- **arXiv**: [2605.15398](https://arxiv.org/abs/2605.15398)
- **作者**: Nicole Meng, Zheyuan Liu, Meng Jiang, Yingjie Lao
- **类别**: cs.GR, cs.CV

**摘要**: 3DGS 文本驱动编辑管线在遇到不安全提示时会产生跨视角一致的 NSFW 内容。3DEditSafe 首次研究该安全问题，结合生成阶段安全引导、渲染视图 3D 安全正则化、安全语义投影、残差抑制和掩码感知保护，有效降低不安全语义传播。同时揭示了安全与质量之间的权衡。

---

### 5. 3D Skew-Normal Splatting

- **arXiv**: [2605.15010](https://arxiv.org/abs/2605.15010)
- **作者**: Xiangru Wu, Ke Fan, Yanwei Fu
- **类别**: cs.CV

**摘要**: 3DGS 的高斯基元是对称的，在有限基元预算下难以表现不对称结构（如物体边界）。本文提出偏态正态光栅化（SNS），采用 Azzalini 偏态正态分布作为基本基元，引入可学习偏态参数，在对称高斯和半高斯之间连续插值。保持仿射变换和分析可导性，无缝集成现有管线。在新视角合成基准上优于高斯及近年非高斯核。

---

## 2026-05-13

### 1. PanoPlane: Plane-Aware Panoramic Completion for Sparse-View Indoor 3D Gaussian Splatting

- **arXiv**: [2605.14135](https://arxiv.org/abs/2605.14135)
- **作者**: Adil Qureshi, Dongki Jung, Jaehoon Choi, Dinesh Manocha
- **类别**: cs.CV

**摘要**: 稀疏视角室内新视角合成。不同于基于透视视角的生成方法，PanoPlane 利用 360° 全景补全，提出 Layout Anchored Attention Steering——推理时将扩散模型注意力引导至检测到的平面表面，用有根据的表面外推替代无约束幻觉。仅需 3 个输入视图即在 Replica、ScanNet++、Matterport3D 上达到 SOTA，PSNR 提升达 17.8%。

---

### 2. HarmoGS: Robust 3D Gaussian Splatting in the Wild via Conflict-Aware Gradient Harmonization

- **arXiv**: [2605.13073](https://arxiv.org/abs/2605.13073)
- **作者**: Yulei Kang, Tianze Zhu, Jian-Fang Hu, Jianhuang Lai, Wei-Shi Zheng
- **类别**: cs.CV

**摘要**: 野生场景 3DGS 面临瞬态干扰物和跨视角外观不一致问题。现有掩码方法无法消除残存遮挡和光照不一致导致的跨视角梯度冲突。HarmoGS 提出双重策略：语义一致性引导掩码自适应精炼先验掩码，双视角冲突感知梯度调和将视图梯度旋转至正交配置以减少负向干扰，配合冲突感知稠密化和裁剪。在野生基准上达到 SOTA。

---

### 3. GuardMarkGS: Unified Ownership Tracing and Edit Deterrence for 3D Gaussian Splatting

- **arXiv**: [2605.12919](https://arxiv.org/abs/2605.12919)
- **作者**: Utae Jeong, Jaewan Choi, Junseok Lee, Jongheon Jeong et al.
- **类别**: cs.CV

**摘要**: 3DGS 资产面临双重版权风险：未经授权使用和恶意编辑。现有方法只能解决其中一面。GuardMarkGS 是首个统一框架，联合优化所有权水印追踪和编辑威慑。对抗分支结合潜空间锚点分离、去噪轨迹偏转和交叉注意力偏转，更新显著性驱动的高斯选择策略分配更强对抗更新。在水印恢复、编辑威慑和渲染质量之间实现良好平衡。

---

### 4. RoSplat: Robust Feed-Forward Pixel-wise Gaussian Splatting for Varying Input Views and High-Resolution Rendering

- **arXiv**: [2605.13093](https://arxiv.org/abs/2605.13093)
- **作者**: Hoang Chuong Nguyen, Renjie Wu, Jose M. Alvarez, Miaomiao Liu
- **类别**: cs.CV

**摘要**: 前向像素级 3DGS 在输入视图数量变化时出现过亮问题，且高斯尺度估计不足导致高分辨率渲染出现孔洞。RoSplat 提出简单的 alpha 归一化策略维持亮度一致性，并引入基于 3D 采样的辅助正则化器改善高斯尺度估计，显著修复两种问题。

---

### 5. Z-Order Transformer for Feed-Forward Gaussian Splatting

- **arXiv**: [2605.13465](https://arxiv.org/abs/2605.13465)
- **作者**: Can Wang, Lei Liu, Wei Jiang, Dong Xu
- **类别**: cs.CV
- **备注**: CVPR 2026 Oral 录用

**摘要**: 传统 3DGS 优化缓慢，前向方法虽快但基元冗余且质量不足。本文设计基于 Transformer 的架构，利用 Z 序曲线将无序高斯集组织为空间连贯序列，通过稀疏注意力捕捉高斯间关系并自适应抑制冗余。单次前向即可用更少基元预测高质量属性。

---

### 6. Sparse Code Uplifting for Efficient 3D Language Gaussian Splatting

- **arXiv**: [2605.13600](https://arxiv.org/abs/2605.13600)
- **作者**: Lovre Antonio Budimir, Yushi Guan, Steve Ryhner, Sven Lončarić, Nandita Vijaykumar
- **类别**: cs.CV

**摘要**: 3D 语言高斯将语言对齐特征附加到高斯上，但存储和渲染成本高昂。SCOUP 将语言表示学习从 3D 优化中解耦：先在 2D 图像区域学习稀疏码本表示，再通过高斯到像素关联加权聚合提升为 3D，Top-K 筛选提取主导系数。训练提速 400 倍，内存节省 3 倍，开放词汇查询精度超越现有方法。

---

## 2026-05-12

### 1. XFreq-GS: Cross-Frequency Wireless Radiation Field Reconstruction with 3D Gaussian Splatting

- **arXiv**: [2605.11432](https://arxiv.org/abs/2605.11432)
- **作者**: Sheng Wang, Hengtao He, Chaozheng Wen, Jingwen Tong et al.
- **类别**: eess.SP

**摘要**: 将 3DGS 应用于跨频率无线辐射场重建。使用共享几何和频率自适应射频属性的高斯基元重建跨频率 WRF 并合成功率角谱图。相比现有单频方法，实现优异的跨频率泛化能力。

---

### 2. PointGS: Semantic-Consistent Unsupervised 3D Point Cloud Segmentation with 3D Gaussian Splatting

- **arXiv**: [2605.11520](https://arxiv.org/abs/2605.11520)
- **作者**: Yixiao Song, Qingyong Li, Wen Wang, Zhicheng Yan
- **类别**: cs.CV, cs.AI
- **备注**: CVPR 2026 录用

**摘要**: 无监督点云分割面临 2D-3D 语义迁移中的离散连续域不匹配问题。PointGS 利用 3DGS 作为统一中间表示桥接域差：稀疏点云经多视角重建为密集 3D 高斯空间，消除投影重叠；多视角渲染图经 SAM 提取语义掩码，对比学习将语义蒸馏到高斯基元上；最后通过最近邻搜索分配点语义。ScanNet-V2 mIoU 提升 +0.9%，S3DIS 提升 +2.8%。

---

### 3. 3D Gaussian Splatting for Efficient Retrospective Dynamic Scene Novel View Synthesis with a Standardized Benchmark

- **arXiv**: [2605.12437](https://arxiv.org/abs/2605.12437)
- **作者**: Yunxiao Zhang, Suryansh Kumar
- **类别**: cs.CV
- **备注**: CVPR 2026 录用

**摘要**: 同步多视图动态场景重建中，显式时间耦合并非必需。文章论证校准同步视图已提供充分空间一致性，通过 SfM 点云初始化并随时间传播优化高斯即可实现高效回溯新视角合成。同时介绍了基于 Blender 的动态多视图数据集框架和基准套件。

---

### 4. 3DGS³: Joint Super Sampling and Frame Interpolation for Real-Time Large-Scale 3DGS Rendering

- **arXiv**: [2605.11489](https://arxiv.org/abs/2605.11489)
- **作者**: Yibo Zhao, Fan Gao, Youcheng Cai, Ligang Liu
- **类别**: cs.GR, cs.CV

**摘要**: 3DGS 在超密集场景和高分辨率下存在计算瓶颈。3DGS³ 是统一后处理框架，利用 3DGS 的连续可微性：梯度感知超采样模块提取图像梯度引导 GRU 精炼网络实现高保真超采样；轻量级时序帧插值模块融合连续帧时序和空间线索合成中间帧。兼顾高分辨率和高帧率渲染。

---

### 5. PoseCompass: Intelligent Synthetic Pose Selection for Visual Localization

- **arXiv**: [2605.12144](https://arxiv.org/abs/2605.12144)
- **作者**: Yanan Zhou, Zhaoyan Qian, Yanli Li, Nan Yang et al.
- **类别**: cs.CV

**摘要**: APR 位姿回归依赖微调数据质量。基于 3DGS 的新视角合成数据增强中，随机采样产生冗余和噪声。PoseCompass 提出基于价值的位姿筛选机制，综合三个维度：定位难度（偏好挑战区域）、覆盖新颖性（探索欠采样区域）、渲染可观测性（过滤伪像）。在 7-Scenes 上适配时间从 15.2 分降至 5.1 分，中位位姿误差降低 53.8%。

---

### 6. PointForward: Feedforward Driving Reconstruction through Point-Aligned Representations

- **arXiv**: [2605.11594](https://arxiv.org/abs/2605.11594)
- **作者**: Cheng Chi, Xianqi Wang, Hongcheng Luo, Mingfei Tu et al.
- **类别**: cs.CV

**摘要**: 前向 3DGS 驾驶重建中像素对齐范式存在多视角不一致和分层伪像。PointForward 在世界空间初始化稀疏 3D 查询，通过时空融合聚合多视图信息，单次前向即可显式确保跨视角一致性。引入场景图组织运动实例，利用 3D 包围盒实现实例级运动传播。在大规模驾驶基准上达到 SOTA。

---

### 7. PairDropGS: Paired Dropout-Induced Consistency Regularization for Sparse-View Gaussian Splatting

- **arXiv**: [2605.12072](https://arxiv.org/abs/2605.12072)
- **作者**: Hantang Li, Qiang Zhu, Xiandong Meng, Xingtao Wang et al.
- **类别**: cs.CV

**摘要**: Dropout 稀疏视角 3DGS 忽略了不同 Dropout 子集间的不一致性。PairDropGS 从共享高斯场构建 Dropout 子对，设计低频一致性正则化约束渲染结构，鼓励共享场在不同随机 dropout 下保持稳定场景布局。渐进一致性调度策略逐步加强正则化。简洁即插即用，显著优于现有 dropout 方法。

---

### 8. GeoQuery: Geometry-Query Diffusion for Sparse-View Reconstruction

- **arXiv**: [2605.12399](https://arxiv.org/abs/2605.12399)
- **作者**: Xiao Cao, Yuze Li, Youmin Zhang, Jiayu Song et al.
- **类别**: cs.CV
- **备注**: SIGGRAPH 2026 录用

**摘要**: 稀疏视角下 3DGS 渲染伪像严重，图像扩散修复中的多视图自注意力在严重损坏查询特征下失效。GeoQuery 提出几何引导交叉注意力机制：利用预测深度和相机位姿构建几何诱导对应场，采样参考特征形成几何对齐代理查询，在局部窗口内限制交叉注意力以抑制虚假匹配。即使在极端视角稀疏下也能稳健重建。

---

## 2026-05-11

### 1. PG-3DGS: Optimizing 3D Gaussian Splatting to Satisfy Physics Objectives

- **arXiv**: [2605.11266](https://arxiv.org/abs/2605.11266)
- **作者**: Zachary Lee, Maxwell Jacobson, Yexiang Xue
- **类别**: cs.CV, cs.GR, cs.LG

**摘要**: 3DGS 仅视觉优化缺乏物理理解。PG-3DGS 将可微物理模拟与 3D 高斯表示耦合，让物理目标引导形状优化。生成的结构不仅外观准确且物理功能可用（如茶壶可倒水、飞机可产生升力）。桌面风洞实验验证 3D 打印飞机在所有测试中升力均高于基线。

---

### 2. AdaptSplat: Adapting Vision Foundation Models for Feed-Forward 3D Gaussian Splatting

- **arXiv**: [2605.10239](https://arxiv.org/abs/2605.10239)
- **作者**: Mingwei Xing, Xinliang Wang, Yifeng Shi
- **类别**: cs.CV

**摘要**: 前向 3DGS 中跨域泛化和高频几何保真度不足。AdaptSplat 证明无需复杂组件，仅引入 1.5M 参数的频率保持适配器（FPA）即可：从强大视觉基础模型浅层特征中提取方向感知高频结构先验，通过高频位置编码和自适应残差调制集成到通用管线。多个基准上达到前向重建 SOTA。

---

### 3. SDTalk: Structured Facial Priors and Dual-Branch Motion Fields for Generalizable Gaussian Talking Head Synthesis

- **arXiv**: [2605.09956](https://arxiv.org/abs/2605.09956)
- **作者**: Peng Jia, Zhen Xiao, Jia Li, Xueliang Liu et al.
- **类别**: cs.CV, cs.AI

**摘要**: 高质量说话人头合成通常依赖特定身份模型。SDTalk 为单帧 3DGS 框架，可泛化到未见身份无需个性化训练。结构面部先验引导重建模块分别预测可见和遮挡区域 3DGS 参数，实现单图完整头部重建；双分支运动场建模粗细粒度面部动态，提升细节保真度和唇形同步。

---

### 4. DySurface: Consistent 4D Surface Reconstruction via Bridging Explicit Gaussians and Implicit Functions

- **arXiv**: [2605.10360](https://arxiv.org/abs/2605.10360)
- **作者**: Minje Kim, Younghyun Noh, Jaesoon Kim, Tae-Kyun Kim
- **类别**: cs.CV

**摘要**: 动态场景几何表面重建中仅光度优化导致几何歧义和表面不连续。DySurface 桥接显式高斯和隐式 SDF：解决 3DGS 前向形变和 SDF 体渲染后向形变之间的结构差异，提出 VoxGS-DSDF 分支利用形变高斯构建动态稀疏体素网格，为隐式 SDF 场提供显式几何引导，实现 watertight 表面重建。

---

### 5. MAGS-SLAM: Monocular Multi-Agent Gaussian Splatting SLAM for Geometrically and Photometrically Consistent Reconstruction

- **arXiv**: [2605.10760](https://arxiv.org/abs/2605.10760)
- **作者**: Zhihao Cao, Qi Shao, Shuhao Zhai, Jing Zhang et al.
- **类别**: cs.RO

**摘要**: 首个仅 RGB 的多智能体 3DGS SLAM 协同重建框架。每个智能体独立构建单目高斯子图并传输紧凑摘要，通过几何和外观感知回环验证、occupancy 感知高斯融合实现一致全局重建，解决单目尺度模糊问题。在合成和真实数据集上达到与 RGB-D 方法相当的渲染质量，同时引入 ReplicaMultiagent Plus 基准。

---

### 6. VEGA: Visual Encoder Grounding Alignment for Spatially-Aware Vision-Language-Action Models

- **arXiv**: [2605.10485](https://arxiv.org/abs/2605.10485)
- **作者**: Hao Wang, Xiaobao Wei, Jingyang He, Chengyu Bai et al.
- **类别**: cs.RO

**摘要**: VLA 模型的视觉骨干缺乏精确空间感知。VEGA 将 VLA 视觉编码器输出直接与具有空间感知特征对齐，后者来自 DINOv2-FiT3D（经多视角一致 3DGS 监督微调）。在视觉编码器层级对齐避免了语言语义纠缠。轻量投影器在推理时可丢弃，零额外开销。在仿真和真实操作任务上达到隐式空间定位 SOTA。
