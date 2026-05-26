# 3D Gaussian Splatting 论文分类索引 (2026-03)

> 基于 `3dgs_2026-03.md` 中收集的论文，按研究方向细分类。
> ★ 表示被顶会/顶刊录用。

## 目录

- [3D Gaussian Splatting 论文分类索引 (2026-03)](#3d-gaussian-splatting-论文分类索引-2026-03)
  - [目录](#目录)
  - [一、核心算法与优化](#cat-core-opt)
  - [二、前馈 3DGS 与可泛化方法](#cat-feed-forward)
  - [三、动态场景与 4D 重建](#cat-dynamic-4d)
  - [四、SLAM 与机器人导航](#cat-slam-robotics)
  - [五、自动驾驶与交通场景](#cat-autonomous-driving)
  - [六、语义分割与场景理解](#cat-semantics)
  - [七、几何与表面重建](#cat-geometry)
  - [八、渲染加速与压缩](#cat-accel-compress)
  - [九、新视角合成](#cat-nvs)
  - [十、数字人与头像](#cat-avatar)
  - [十一、生成式模型与编辑](#cat-generative)
  - [十二、逆向渲染与重光照](#cat-relighting)
  - [十三、医疗与工业应用](#cat-medical-industrial)
  - [十四、视觉定位与水印安全](#cat-loc-security)
  - [十五、流媒体与编码](#cat-streaming)
  - [十六、其他应用与交叉领域](#cat-other)
  - [统计概览](#统计概览)

---

## 一、核心算法与优化 {#cat-core-opt}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-27 | ★ [GaussFusion](../3dgs_2026-03.md#gaussfusion-improving-3d-reconstruction-in-the-wild-with-a-geometry-informed-video-generator) | [2603.25053](https://arxiv.org/abs/2603.25053) | 几何感知视频生成器，CVPR'26 |
| 2026-03-23 | [Drop-In Perceptual Optimization](../3dgs_2026-03.md#drop-in-perceptual-optimization-for-3d-gaussian-splatting) | [2603.23297](https://arxiv.org/abs/2603.23297) | 即插即用感知优化 |
| 2026-03-16 | [NanoGS](../3dgs_2026-03.md#nanogs-training-free-gaussian-splat-simplification) | [2603.16103](https://arxiv.org/abs/2603.16103) | 免训练高斯简化 |
| 2026-03-12 | [3DGEER](../3dgs_2026-03.md#3d-gaussian-rendering-made-exact-and-efficient-for-generic-cameras) | [2505.24053](https://arxiv.org/abs/2505.24053) | 通用相机精确渲染，ICLR'26 |
| 2026-03-09 | [SkipGS](../3dgs_2026-03.md#skipgs-post-densification-backward-skipping-for-efficient-3dgs-training) | [2603.08997](https://arxiv.org/abs/2603.08997) | 反向传播跳过，训练加速 |
| 2026-03-09 | [ImprovedGS+](../3dgs_2026-03.md#improvedgs-a-high-performance-ccuda-re-implementation-strategy-for-3d-gaussian-splatting) | [2603.08661](https://arxiv.org/abs/2603.08661) | C++/CUDA 高性能重实现 |
| 2026-03-09 | [Spherical-GOF](../3dgs_2026-03.md#spherical-gof-geometry-aware-panoramic-gaussian-opacity-fields-for-3d-scene-reconstruction) | [2603.08503](https://arxiv.org/abs/2603.08503) | 球面高斯不透明度场 |
| 2026-03-09 | [Improving Continual Learning](../3dgs_2026-03.md#improving-continual-learning-for-gaussian-splatting-based-environments-reconstruction-on-commercial-off-the-shelf-edge-devices) | [2603.08499](https://arxiv.org/abs/2603.08499) | 边缘设备持续学习 |
| 2026-03-07 | [MoE-GS](../3dgs_2026-03.md#moe-gs-mixture-of-experts-for-dynamic-gaussian-splatting) | [2510.19210](https://arxiv.org/abs/2510.19210) | Mixture of Experts，ICLR'26 |
| 2026-03-06 | [EntON](../3dgs_2026-03.md#enton-eigenentropy-optimized-neighborhood-densification-in-3d-gaussian-splatting) | [2603.06216](https://arxiv.org/abs/2603.06216) | 特征熵优化密度控制 |
| 2026-03-05 | [GloSplat](../3dgs_2026-03.md#glosplat-joint-pose-appearance-optimization-for-faster-and-more-accurate-3d-reconstruction) | [2603.04847](https://arxiv.org/abs/2603.04847) | 联合位姿-外观优化 |
| 2026-03-03 | [HeroGS](../3dgs_2026-03.md#herogs-hierarchical-guidance-for-robust-3d-gaussian-splatting-under-sparse-views) | [2603.01099](https://arxiv.org/abs/2603.01099) | 分层引导鲁棒 3DGS |
| 2026-03-03 | [Proxy-GS](../3dgs_2026-03.md#proxy-gs-unified-occlusion-priors-for-training-and-inference-in-structured-3d-gaussian-splatting) | [2509.24421](https://arxiv.org/abs/2509.24421) | 遮挡先验统一框架 |
| 2026-03-02 | [tttLRM](../3dgs_2026-03.md#tttlrm-test-time-training-for-long-context-and-autoregressive-3d-reconstruction) | [2602.20160](https://arxiv.org/abs/2602.20160) | 测试时训练，CVPR'26 |
| 2026-03-02 | [StreamSplat](../3dgs_2026-03.md#streamsplat-towards-online-dynamic-3d-reconstruction-from-uncalibrated-video-streams) | [2506.08862](https://arxiv.org/abs/2506.08862) | 全前馈动态重建，ICLR'26 |
| 2026-03-01 | ★ [FLICKER](../3dgs_2026-03.md#flicker-a-fine-grained-contribution-aware-accelerator-for-real-time-3d-gaussian-splatting) | [2603.01158](https://arxiv.org/abs/2603.01158) | 贡献感知硬件加速器，DATE'26 |

**概要**: 改进 3DGS 基础优化过程，包括优化器设计、密度控制、基元分裂/裁剪策略、训练加速、硬件加速等。MoE-GS 用 MoE 架构提升动态场景一致性，NanoGS 免训练简化模型，SkipGS 减少 23% 训练时间。

---

## 二、前馈 3DGS 与可泛化方法 {#cat-feed-forward}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-26 | [Less Gaussians, Texture More](../3dgs_2026-03.md#less-gaussians-texture-more-4k-feed-forward-textured-splatting) | [2603.25745](https://arxiv.org/abs/2603.25745) | 4K 前馈纹理溅射 |
| 2026-03-26 | [ViewSplat](../3dgs_2026-03.md#viewsplat-view-adaptive-dynamic-gaussian-splatting-for-feed-forward-synthesis) | [2603.25265](https://arxiv.org/abs/2603.25265) | 视图自适应前馈合成 |
| 2026-03-26 | [AirSplat](../3dgs_2026-03.md#airsplat-alignment-and-rating-for-robust-feed-forward-3d-gaussian-splatting) | [2603.25129](https://arxiv.org/abs/2603.25129) | 对齐+评分鲁棒前馈 |
| 2026-03-25 | [F4Splat](../3dgs_2026-03.md#f4splat-feed-forward-predictive-densification-for-feed-forward-3d-gaussian-splatting) | [2603.21304](https://arxiv.org/abs/2603.21304) | 前馈预测密度增强 |
| 2026-03-24 | [AdvSplat](../3dgs_2026-03.md#advsplat-adversarial-attacks-on-feed-forward-gaussian-splatting-models) | [2603.23686](https://arxiv.org/abs/2603.23686) | 前馈模型对抗攻击 |
| 2026-03-24 | [2Xplat](../3dgs_2026-03.md#2xplat-two-experts-are-better-than-one-generalist) | [2603.21064](https://arxiv.org/abs/2603.21064) | 双专家前馈架构 |
| 2026-03-24 | [Uni3R](../3dgs_2026-03.md#uni3r-unified-3d-reconstruction-and-semantic-understanding-via-generalizable-gaussian-splatting-from-unposed-multi-view-images) | [2508.03643](https://arxiv.org/abs/2508.03643) | 统一重建+语义理解 |
| 2026-03-23 | [Camera-Agnostic Pruning](../3dgs_2026-03.md#camera-agnostic-pruning-of-3d-gaussian-splats-via-descriptor-based-beta-evidence) | [2603.21933](https://arxiv.org/abs/2603.21933) | 相机无关剪枝 |
| 2026-03-20 | [Matryoshka GS](../3dgs_2026-03.md#matryoshka-gaussian-splatting) | [2603.19234](https://arxiv.org/abs/2603.19234) | 嵌套多分辨率表示 |
| 2026-03-17 | [Leveling3D](../3dgs_2026-03.md#leveling3d-leveling-up-3d-reconstruction-with-feed-forward-3d-gaussian-splatting-and-geometry-aware-generation) | [2603.16211](https://arxiv.org/abs/2603.16211) | 前馈+几何感知生成 |
| 2026-03-17 | [InstantHDR](../3dgs_2026-03.md#instanthdr-single-forward-gaussian-splatting-for-high-dynamic-range-3d-reconstruction) | [2603.11298](https://arxiv.org/abs/2603.11298) | 单次前向 HDR 重建 |
| 2026-03-12 | [VolSplat](../3dgs_2026-03.md#volsplat-rethinking-feed-forward-3d-gaussian-splatting-with-voxel-aligned-prediction) | [2509.19297](https://arxiv.org/abs/2509.19297) | 体素对齐前馈预测 |
| 2026-03-10 | [DenoiseSplat](../3dgs_2026-03.md#denoisesplat-feed-forward-gaussian-splatting-for-noisy-3d-scene-reconstruction) | [2603.09291](https://arxiv.org/abs/2603.09291) | 噪声场景前馈重建 |
| 2026-03-10 | ★ [Speeding Up 3D Gaussians](../3dgs_2026-03.md#speeding-up-the-learning-of-3d-gaussians-with-much-shorter-gaussian-lists) | [2603.09277](https://arxiv.org/abs/2603.09277) | 更短高斯列表加速，CVPR'26 |
| 2026-03-08 | [ReconDrive](../3dgs_2026-03.md#recondrive-fast-feed-forward-4d-gaussian-splatting-for-autonomous-driving-scene-reconstruction) | [2603.07552](https://arxiv.org/abs/2603.07552) | VGGT 驱动前馈 4D |
| 2026-03-03 | [Multimodal-Prior-Guided Sampling](../3dgs_2026-03.md#multimodal-prior-guided-importance-sampling-for-hierarchical-gaussian-splatting-in-sparse-view-novel-view-synthesis) | [2603.02866](https://arxiv.org/abs/2603.02866) | 多模态先验重要性采样 |
| 2026-03-02 | ★ [SemGS](../3dgs_2026-03.md#semgs-feed-forward-semantic-3d-gaussian-splatting-from-sparse-views-for-generalizable-scene-understanding) | [2603.02548](https://arxiv.org/abs/2603.02548) | 前馈语义 3DGS，ICRA'26 |
| 2026-03-02 | [Sparse View Distractor-Free GS](../3dgs_2026-03.md#sparse-view-distractor-free-gaussian-splatting) | [2603.01603](https://arxiv.org/abs/2603.01603) | 稀疏视图无干扰 GS |

**概要**: 无需逐场景优化即可合成新视角或重建场景的前馈/可泛化方法。3 月该方向论文数量众多，涵盖视图自适应、鲁棒对齐、预测密度增强、双专家架构、噪声鲁棒、HDR 等子方向。

---

## 三、动态场景与 4D 重建 {#cat-dynamic-4d}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-31 | ★ [MotionScale](../3dgs_2026-03.md#motionscale-reconstructing-appearance-geometry-and-motion-of-dynamic-scenes-with-scalable-4d-gaussian-splatting) | [2603.29296](https://arxiv.org/abs/2603.29296) | 可扩展 4D 重建，CVPR'26 |
| 2026-03-27 | [Relaxed Rigidity with Ray-based Grouping](../3dgs_2026-03.md#relaxed-rigidity-with-ray-based-grouping-for-dynamic-gaussian-splatting) | [2603.24994](https://arxiv.org/abs/2603.24994) | 放松刚性约束，射线分组 |
| 2026-03-27 | [SpeeDe3DGS](../3dgs_2026-03.md#speede3dgs-speedy-deformable-3d-gaussian-splatting-with-temporal-pruning-and-motion-grouping) | [2506.07917](https://arxiv.org/abs/2506.07917) | 时间剪枝+运动分组加速 |
| 2026-03-27 | [Gaussian Mapping for Evolving Scenes](../3dgs_2026-03.md#gaussian-mapping-for-evolving-scenes) | [2506.06909](https://arxiv.org/abs/2506.06909) | 演化场景增量建图 |
| 2026-03-26 | [MoRGS](../3dgs_2026-03.md#morgs-efficient-per-gaussian-motion-reasoning-for-streamable-dynamic-3d-scenes) | [2603.25042](https://arxiv.org/abs/2603.25042) | 逐高斯运动推理 |
| 2026-03-26 | ★ [MoRel](../3dgs_2026-03.md#morel-long-range-flicker-free-4d-motion-modeling-via-anchor-relay-based-bidirectional-blending-with-hierarchical-densification) | [2512.09270](https://arxiv.org/abs/2512.09270) | 长程无闪烁 4D 运动，CVPR'26 |
| 2026-03-25 | [SpectralSplats](../3dgs_2026-03.md#spectralsplats-robust-differentiable-tracking-via-spectral-moment-supervision) | [2603.24036](https://arxiv.org/abs/2603.24036) | 光谱矩监督可微跟踪 |
| 2026-03-23 | [RefacGS](../3dgs_2026-03.md#refracgs-novel-view-synthesis-through-refractive-water-surfaces-with-3d-gaussian-ray-tracing) | [2603.21695](https://arxiv.org/abs/2603.21695) | 折射水面新视角合成 |
| 2026-03-21 | [Fast and Robust Deformable 3DGS](../3dgs_2026-03.md#fast-and-robust-deformable-3d-gaussian-splatting) | [2603.20857](https://arxiv.org/abs/2603.20857) | 快速鲁棒形变 3DGS |
| 2026-03-15 | [UPGS](../3dgs_2026-03.md#upgs-unified-pose-aware-gaussian-splatting-for-dynamic-scene-deblurring) | [2509.00831](https://arxiv.org/abs/2509.00831) | 统一位姿感知去模糊 |
| 2026-03-12 | [Mango-GS](../3dgs_2026-03.md#mango-gs-enhancing-spatio-temporal-consistency-in-dynamic-scenes-reconstruction-using-multi-frame-node-guided-4d-gaussian-splatting) | [2603.11543](https://arxiv.org/abs/2603.11543) | 多帧节点引导 4D 重建 |
| 2026-03-11 | [Grow with the Flow](../3dgs_2026-03.md#grow-with-the-flow-4d-reconstruction-of-growing-plants-with-gaussian-flow-fields) | [2602.08958](https://arxiv.org/abs/2602.08958) | 植物生长 4D 重建 |
| 2026-03-11 | [PLANING](../3dgs_2026-03.md#planing-a-loosely-coupled-triangle-gaussian-framework-for-streaming-3d-reconstruction) | [2601.22046](https://arxiv.org/abs/2601.22046) | 三角-高斯流式重建 |
| 2026-03-09 | [DynamicVGGT](../3dgs_2026-03.md#dynamicvggt-learning-dynamic-point-maps-for-4d-scene-reconstruction-in-autonomous-driving) | [2603.08254](https://arxiv.org/abs/2603.08254) | VGGT 扩展到动态 4D |
| 2026-03-09 | [ReSplat](../3dgs_2026-03.md#resplat-learning-recurrent-gaussian-splatting) | [2510.08575](https://arxiv.org/abs/2510.08575) | 循环高斯溅射 |
| 2026-03-06 | [Advances in 4D Representation](../3dgs_2026-03.md#advances-in-4d-representation-geometry-motion-and-interaction) | [2510.19255](https://arxiv.org/abs/2510.19255) | 4D 表示综述 |
| 2026-03-05 | ★ [UFO-4D](../3dgs_2026-03.md#ufo-4d-unposed-feedforward-4d-reconstruction-from-two-images) | [2602.24290](https://arxiv.org/abs/2602.24290) | 无位姿前馈 4D 重建，ICLR'26 |
| 2026-03-02 | ★ [CloDS](../3dgs_2026-03.md#clods-visual-only-unsupervised-cloth-dynamics-learning-in-unknown-conditions) | [2602.01844](https://arxiv.org/abs/2602.01844) | 无监督布料动力学，ICLR'26 |
| 2026-03-02 | ★ [PhysGM](../3dgs_2026-03.md#physgm-large-physical-gaussian-model-for-feed-forward-4d-synthesis) | [2508.13911](https://arxiv.org/abs/2508.13911) | 大物理高斯模型，CVPR'26 |

**概要**: 处理随时间变化的动态场景，包括 4D 高斯表示、形变场建模、时序一致性、增量更新等。MotionScale 和 MoRel 两篇 CVPR'26 论文分别实现可扩展 4D 重建和长程无闪烁运动建模。

---

## 四、SLAM 与机器人导航 {#cat-slam-robotics}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-22 | ★ [SGAD-SLAM](../3dgs_2026-03.md#sgad-slam-splatting-gaussians-at-adjusted-depth-for-better-radiance-fields-in-rgbd-slam) | [2603.21055](https://arxiv.org/abs/2603.21055) | 深度调整 GS SLAM，CVPR'26 |
| 2026-03-22 | ★ [MipSLAM](../3dgs_2026-03.md#mipslam-alias-free-gaussian-splatting-slam) | [2603.06989](https://arxiv.org/abs/2603.06989) | 无混叠 GS SLAM，ICRA'26 |
| 2026-03-20 | [TRGS-SLAM](../3dgs_2026-03.md#trgs-slam-imu-aided-gaussian-splatting-slam-for-blurry-rolling-shutter-and-noisy-thermal-images) | [2603.20443](https://arxiv.org/abs/2603.20443) | 热图像 IMU 辅助 SLAM |
| 2026-03-19 | [FeatureSLAM](../3dgs_2026-03.md#featureslam-feature-enriched-3d-gaussian-splatting-slam-in-real-time) | [2601.05738](https://arxiv.org/abs/2601.05738) | 特征增强实时 SLAM |
| 2026-03-17 | [M³](../3dgs_2026-03.md#m3-dense-matching-meets-multi-view-foundation-models-for-monocular-gaussian-splatting-slam) | [2603.16844](https://arxiv.org/abs/2603.16844) | 密集匹配+多视图基础模型 |
| 2026-03-12 | [VIGS-SLAM](../3dgs_2026-03.md#vigs-slam-visual-inertial-gaussian-splatting-slam) | [2512.02293](https://arxiv.org/abs/2512.02293) | 视觉惯性 GS SLAM |
| 2026-03-10 | ★ [VarSplat](../3dgs_2026-03.md#varsplat-uncertainty-aware-3d-gaussian-splatting-for-robust-rgbd-slam) | [2603.09673](https://arxiv.org/abs/2603.09673) | 不确定性感知 RGB-D SLAM，CVPR'26 |
| 2026-03-09 | ★ [MCGS-SLAM](../3dgs_2026-03.md#mcgs-slam-a-multi-camera-slam-framework-using-gaussian-splatting-for-high-fidelity-mapping) | [2509.14191](https://arxiv.org/abs/2509.14191) | 多摄像头 RGB SLAM，ICRA'26 |
| 2026-03-09 | [LIVE-GS](../3dgs_2026-03.md#live-gs-online-lidar-inertial-visual-state-estimation-and-globally-consistent-mapping-with-3d-gaussian-splatting) | [2507.23273](https://arxiv.org/abs/2507.23273) | LiDAR-惯性-视觉紧耦合 |
| 2026-03-08 | [LagMemo](../3dgs_2026-03.md#lagmemo-language-3d-gaussian-splatting-memory-for-multi-modal-open-vocabulary-multi-goal-visual-navigation) | [2510.24118](https://arxiv.org/abs/2510.24118) | 语言 3DGS 导航记忆 |
| 2026-03-03 | ★ [OnlineX](../3dgs_2026-03.md#onlinex-unified-online-3d-reconstruction-and-understanding-with-active-to-stable-state-evolution) | [2603.02134](https://arxiv.org/abs/2603.02134) | 在线重建+理解，CVPR Finding'26 |
| 2026-03-02 | [VGGT Distractor-Free](../3dgs_2026-03.md#sparse-view-distractor-free-gaussian-splatting) | [2603.01603](https://arxiv.org/abs/2603.01603) | VGGT 先验无干扰 GS |
| 2026-03-01 | ★ [Openfly](../3dgs_2026-03.md#openfly-a-comprehensive-platform-for-aerial-vision-language-navigation) | [2502.18041](https://arxiv.org/abs/2502.18041) | 航空 VLN 平台，ICLR'26 |

**概要**: 基于 3DGS 的 SLAM 系统在 3 月表现活跃，涵盖 RGB-D、多摄像头、视觉惯性、LiDAR 融合等多种传感器组合。VarSplat、MipSLAM、SGAD-SLAM 三篇 CVPR/ICRA 录用论文分别聚焦不确定性感知、无混叠和深度调整。

---

## 五、自动驾驶与交通场景 {#cat-autonomous-driving}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-27 | [Drive-Through](../3dgs_2026-03.md#drive-through-3d-vehicle-exterior-reconstruction-via-dynamic-scene-sfm-and-distortion-aware-gaussian-splatting) | [2603.26638](https://arxiv.org/abs/2603.26638) | 车辆外部 3D 重建 |
| 2026-03-19 | [StreetForward](../3dgs_2026-03.md#streetforward-perceiving-dynamic-street-with-feedforward-causal-attention) | [2603.19552](https://arxiv.org/abs/2603.19552) | 动态街道前馈感知 |
| 2026-03-19 | [Splat2BEV](../3dgs_2026-03.md#reconstruction-matters-learning-geometry-aligned-bev-representation-through-3d-gaussian-splatting) | [2603.19193](https://arxiv.org/abs/2603.19193) | 3DGS 到 BEV 表示 |
| 2026-03-19 | [GSMem](../3dgs_2026-03.md#gsmem-3d-gaussian-splatting-as-persistent-spatial-memory-for-zero-shot-embodied-exploration-and-reasoning) | [2603.19137](https://arxiv.org/abs/2603.19137) | 持久空间记忆 |
| 2026-03-16 | [NavGSim](../3dgs_2026-03.md#navgsim-high-fidelity-gaussian-splatting-simulator-for-large-scale-navigation) | [2603.15186](https://arxiv.org/abs/2603.15186) | 大规模导航模拟器 |
| 2026-03-15 | [RadarGaussianDet3D](../3dgs_2026-03.md#radargaussiandet3d-gaussian-representation-based-real-time-3d-object-detection-with-4d-automotive-radars) | [2509.16119](https://arxiv.org/abs/2509.16119) | 4D 雷达 3D 目标检测，IEEE RAL |
| 2026-03-12 | [3DGS-DET](../3dgs_2026-03.md#3dgs-det-empower-3d-gaussian-splatting-with-boundary-guidance-and-box-focused-sampling-for-indoor-3d-object-detection) | [2410.01647](https://arxiv.org/abs/2410.01647) | 边界引导 3D 目标检测 |
| 2026-03-08 | [ReconDrive](../3dgs_2026-03.md#recondrive-fast-feed-forward-4d-gaussian-splatting-for-autonomous-driving-scene-reconstruction) | [2603.07552](https://arxiv.org/abs/2603.07552) | VGGT 前馈 4D 重建 |
| 2026-03-06 | ★ [Transforming Omnidirectional RGB-LiDAR](../3dgs_2026-03.md#transforming-omnidirectional-rgb-lidar-data-into-3d-gaussian-splatting) | [2603.06061](https://arxiv.org/abs/2603.06061) | 全景 RGB-LiDAR 管线，IROS'26 |

**概要**: 3DGS 在自动驾驶领域的应用持续扩展，涵盖动态街道感知、BEV 表示学习、4D 雷达目标检测、VGGT 前馈 4D 重建等方向。

---

## 六、语义分割与场景理解 {#cat-semantics}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-31 | ★ [TreeGaussian](../3dgs_2026-03.md#treegaussian-tree-guided-cascaded-contrastive-learning-for-hierarchical-consistent-3d-gaussian-scene-segmentation-and-understanding) | [2604.03309](https://arxiv.org/abs/2604.03309) | 树引导级联对比分割 |
| 2026-03-30 | ★ [Off The Grid](../3dgs_2026-03.md#off-the-grid-detection-of-primitives-for-feed-forward-3d-gaussian-splatting) | [2512.15508](https://arxiv.org/abs/2512.15508) | 基元结构检测，CVPR'26 |
| 2026-03-27 | ★ [ExtrinSplat](../3dgs_2026-03.md#extrinsplat-decoupling-geometry-and-semantics-for-open-vocabulary-understanding-in-3d-gaussian-splatting) | [2509.22225](https://arxiv.org/abs/2509.22225) | 几何语义解耦，CVPR'26 |
| 2026-03-27 | [VG-Mapping](../3dgs_2026-03.md#vg-mapping-variation-aware-density-control-for-online-3d-gaussian-mapping-in-semi-static-scenes) | [2510.09962](https://arxiv.org/abs/2510.09962) | 变化感知在线建图 |
| 2026-03-23 | [IDSplat](../3dgs_2026-03.md#idsplat-instance-decomposed-3d-gaussian-splatting-for-driving-scenes) | [2511.19235](https://arxiv.org/abs/2511.19235) | 实例分解驾驶场景 |
| 2026-03-19 | ★ [OnlinePG](../3dgs_2026-03.md#onlinepg-online-open-vocabulary-panoptic-mapping-with-3d-gaussian-splatting) | [2603.18510](https://arxiv.org/abs/2603.18510) | 在线开放词汇全景映射，CVPR'26 |
| 2026-03-19 | [Camera-Aware Cross-View Alignment](../3dgs_2026-03.md#camera-aware-cross-view-alignment-for-referring-3d-gaussian-splatting-segmentation) | [2511.03992](https://arxiv.org/abs/2511.03992) | 引用分割，ICME'26 |
| 2026-03-18 | [Semantic Segmentation for Lunar Surface](../3dgs_2026-03.md#semantic-segmentation-and-depth-estimation-for-real-time-lunar-surface-mapping-using-3d-gaussian-splatting) | [2603.18218](https://arxiv.org/abs/2603.18218) | 月球表面语义分割 |
| 2026-03-18 | [UniSem](../3dgs_2026-03.md#unisem-generalizable-semantic-3d-reconstruction-from-sparse-unposed-images) | [2603.17519](https://arxiv.org/abs/2603.17519) | 可泛化语义 3D 重建 |
| 2026-03-15 | [S2GS](../3dgs_2026-03.md#s2gs-streaming-semantic-gaussian-splatting-for-online-scene-understanding-and-reconstruction) | [2603.14232](https://arxiv.org/abs/2603.14232) | 流式语义 GS |
| 2026-03-10 | ★ [REALM](../3dgs_2026-03.md#realm-an-mllm-agent-framework-for-open-world-3d-reasoning-segmentation-and-editing-on-gaussian-splatting) | [2510.16410](https://arxiv.org/abs/2510.16410) | MLLM-Agent 推理分割编辑，CVPR'26 |
| 2026-03-10 | [CoRe-GS](../3dgs_2026-03.md#core-gs-coarse-to-refined-gaussian-splatting-with-semantic-object-focus) | [2509.04859](https://arxiv.org/abs/2509.04859) | 粗到精语义对象聚焦 |
| 2026-03-06 | [VG3S](../3dgs_2026-03.md#vg3s-visual-geometry-grounded-gaussian-splatting-for-semantic-occupancy-prediction) | [2603.06210](https://arxiv.org/abs/2603.06210) | 视觉几何接地语义占用 |
| 2026-03-06 | [PoI](../3dgs_2026-03.md#poi-a-filter-to-extract-pixel-of-interest-from-novel-views-for-scene-coordinate-regression) | [2502.04843](https://arxiv.org/abs/2502.04843) | 兴趣像素过滤 |
| 2026-03-04 | [Holi-Spatial](../3dgs_2026-03.md#holi-spatial-evolving-video-streams-into-holistic-3d-spatial-intelligence) | [2603.07660](https://arxiv.org/abs/2603.07660) | 大规模空间感知数据集 |
| 2026-03-04 | [3DGS-HPC](../3dgs_2026-03.md#3dgs-hpc-distractor-free-3d-gaussian-splatting-with-hybrid-patch-wise-classification) | [2603.07587](https://arxiv.org/abs/2603.07587) | 混合分块分类 |
| 2026-03-03 | [LangSurf](../3dgs_2026-03.md#langsurf-language-embedded-surface-gaussians-for-3d-scene-understanding) | [2412.17635](https://arxiv.org/abs/2412.17635) | 语言嵌入表面场 |
| 2026-03-02 | [X-GS](../3dgs_2026-03.md#x-gs-an-extensible-open-framework-for-perceiving-and-thinking-via-3d-gaussian-splatting) | [2603.09632](https://arxiv.org/abs/2603.09632) | 可扩展感知推理框架 |
| 2026-03-02 | [HUGE-Bench](../3dgs_2026-03.md#huge-bench-a-benchmark-for-high-level-uav-vision-language-action-tasks) | [2603.19822](https://arxiv.org/abs/2603.19822) | UAV VLA 基准 |

**概要**: 3DGS 上的语义分割、开放词汇场景理解、语言 grounding 和物体级提取。ExtrinSplat、OnlinePG 和 REALM 三篇 CVPR'26 论文分别聚焦几何语义解耦、在线全景映射和 MLLM 驱动的 3D 推理分割编辑。

---

## 七、几何与表面重建 {#cat-geometry}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-29 | [MeshSplats](../3dgs_2026-03.md#meshsplats-mesh-based-rendering-with-gaussian-splatting-initialization) | [2502.07754](https://arxiv.org/abs/2502.07754) | 网格+高斯混合渲染 |
| 2026-03-28 | [DiffSoup](../3dgs_2026-03.md#diffsoup-direct-differentiable-rasterization-of-triangle-soup-for-extreme-radiance-field-simplification) | [2603.27151](https://arxiv.org/abs/2603.27151) | 三角形汤可微光栅化 |
| 2026-03-27 | ★ [GLINT](../3dgs_2026-03.md#glint-modeling-scene-scale-transparency-via-gaussian-radiance-transport) | [2603.26181](https://arxiv.org/abs/2603.26181) | 场景级透明度建模，CVPR'26 |
| 2026-03-26 | ★ [Cross-Instance Registration](../3dgs_2026-03.md#cross-instance-gaussian-splatting-registration-via-geometry-aware-feature-guided-alignment) | [2603.21936](https://arxiv.org/abs/2603.21936) | 跨实例配准，CVPR'26 |
| 2026-03-26 | ★ [Self-Constrained Priors](../3dgs_2026-03.md#3d-gaussian-splatting-with-self-constrained-priors-for-high-fidelity-surface-reconstruction) | [2603.19682](https://arxiv.org/abs/2603.19682) | 自约束先验表面重建，CVPR'26 |
| 2026-03-25 | [Accurate Point Measurement](../3dgs_2026-03.md#accurate-point-measurement-in-3dgs-a-new-alternative-to-traditional-stereoscopic-view-based-measurements) | [2603.24716](https://arxiv.org/abs/2603.24716) | 精确点测量，ISPRS'26 |
| 2026-03-24 | [GTLR-GS](../3dgs_2026-03.md#gtlr-gs-geometry-texture-aware-lidar-regularized-3d-gaussian-splatting-for-realistic-scene-reconstruction) | [2603.23192](https://arxiv.org/abs/2603.23192) | LiDAR 几何正则化 |
| 2026-03-24 | [Predictive Photometric Uncertainty](../3dgs_2026-03.md#predictive-photometric-uncertainty-in-gaussian-splatting-for-novel-view-synthesis) | [2603.22786](https://arxiv.org/abs/2603.22786) | 预测光度不确定性 |
| 2026-03-16 | [Laplace-Beltrami Operator for GS](../3dgs_2026-03.md#laplace-beltrami-operator-for-gaussian-splatting) | [2502.17531](https://arxiv.org/abs/2502.17531) | 拉普拉斯-贝尔特拉米算子 |
| 2026-03-14 | ★ [PhyGaP](../3dgs_2026-03.md#phygap-physically-grounded-gaussians-with-polarization-cues) | [2603.14001](https://arxiv.org/abs/2603.14001) | 极化线索物理感知，CVPR'26 |
| 2026-03-11 | [PolGS++](../3dgs_2026-03.md#polgs-physically-guided-polarimetric-gaussian-splatting-for-fast-reflective-surface-reconstruction) | [2603.10801](https://arxiv.org/abs/2603.10801) | 偏振高斯反射表面重建 |
| 2026-03-07 | ★ [GS-2M](../3dgs_2026-03.md#gs-2m-material-aware-gaussian-splatting-for-high-fidelity-mesh-reconstruction) | [2509.22276](https://arxiv.org/abs/2509.22276) | 材质感知网格重建，Eurographics'26 |
| 2026-03-05 | [SSR-GS](../3dgs_2026-03.md#ssr-gs-separating-specular-reflection-in-gaussian-splatting-for-glossy-surface-reconstruction) | [2603.05152](https://arxiv.org/abs/2603.05152) | 镜面反射 glossy 表面重建 |
| 2026-03-04 | [Generalized non-exponential GS](../3dgs_2026-03.md#generalized-non-exponential-gaussian-splatting) | [2603.02887](https://arxiv.org/abs/2603.02887) | 非指数辐射传输泛化 |
| 2026-03-03 | [Intrinsic Geometry-Appearance Consistency](../3dgs_2026-03.md#intrinsic-geometry-appearance-consistency-optimization-for-sparse-view-gaussian-splatting) | [2603.02893](https://arxiv.org/abs/2603.02893) | 几何-外观一致性优化 |
| 2026-03-01 | [FastAvatar](../3dgs_2026-03.md#fastavatar-towards-unified-and-fast-3d-avatar-reconstruction-with-large-gaussian-reconstruction-transformers) | [2508.19754](https://arxiv.org/abs/2508.19754) | 大高斯重建 Transformer |

**概要**: 从图像重建几何准确的表面、网格或点云，包括表面光栅化、高频细节恢复、多传感器融合、透明度/反射建模等。GLINT 和 GS-2M 分别被 CVPR'26 和 Eurographics'26 录用。

---

## 八、渲染加速与压缩 {#cat-accel-compress}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-28 | [PocketGS](../3dgs_2026-03.md#pockets-on-device-training-of-3d-gaussian-splatting-for-high-perceptual-modeling) | [2601.17354](https://arxiv.org/abs/2601.17354) | 端侧训练，量化+稀疏化 |
| 2026-03-28 | [SplatSuRe](../3dgs_2026-03.md#splatsure-selective-super-resolution-for-multi-view-consistent-3d-gaussian-splatting) | [2512.02172](https://arxiv.org/abs/2512.02172) | 选择性超分辨率 |
| 2026-03-27 | [Smol-GS](../3dgs_2026-03.md#smol-gs-compact-representations-for-abstract-3d-gaussian-splatting) | [2512.00850](https://arxiv.org/abs/2512.00850) | 紧凑抽象表示 |
| 2026-03-24 | [FilterGS](../3dgs_2026-03.md#filtergs-traversal-free-parallel-filtering-and-adaptive-shrinking-for-large-scale-lod-3d-gaussian-splatting) | [2603.23891](https://arxiv.org/abs/2603.23891) | 免遍历并行滤波 |
| 2026-03-20 | [SRGS](../3dgs_2026-03.md#srgs-super-resolution-3d-gaussian-splatting) | [2404.10318](https://arxiv.org/abs/2404.10318) | 超分辨率 3DGS |
| 2026-03-19 | [GoDe](../3dgs_2026-03.md#gode-gaussians-on-demand-for-progressive-level-of-detail-and-scalable-compression) | [2501.13558](https://arxiv.org/abs/2501.13558) | 按需高斯，渐进 LOD |
| 2026-03-12 | [Mobile-GS](../3dgs_2026-03.md#mobile-gs-real-time-gaussian-splatting-for-mobile-devices) | [2603.11531](https://arxiv.org/abs/2603.11531) | 移动端实时渲染 |
| 2026-03-09 | [ExGS](../3dgs_2026-03.md#exgs-extreme-3d-gaussian-compression-with-diffusion-priors) | [2509.24758](https://arxiv.org/abs/2509.24758) | 扩散先验压缩，100x+ |

**概要**: 提升 3DGS 渲染性能或降低存储开销，包括硬件加速、端侧训练、移动端优化、压缩与编码等。ExGS 用扩散先验实现超过 100x 压缩。

---

## 九、新视角合成 {#cat-nvs}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-31 | ★ [SGS-Intrinsic](../3dgs_2026-03.md#sgs-intrinsic-semantic-invariant-gaussian-splatting-for-sparse-view-indoor-inverse-rendering) | [2603.27516](https://arxiv.org/abs/2603.27516) | 语义不变稀疏视角，CVPR'26 |
| 2026-03-30 | ★ [Hierarchical Visual Relocalization](../3dgs_2026-03.md#hierarchical-visual-relocalization-with-nearest-view-synthesis-from-feature-gaussian-splatting) | [2603.29185](https://arxiv.org/abs/2603.29185) | 分层视觉重定位，CVPR'26 |
| 2026-03-26 | [IDESplat](../3dgs_2026-03.md#idesplat-iterative-depth-probability-estimation-for-generalizable-3d-gaussian-splatting) | [2601.03824](https://arxiv.org/abs/2601.03824) | 迭代深度概率估计 |
| 2026-03-16 | [GeoNVS](../3dgs_2026-03.md#geonvs-geometry-grounded-video-diffusion-for-novel-view-synthesis) | [2603.14965](https://arxiv.org/abs/2603.14965) | 几何接地视频扩散 |
| 2026-03-13 | [Enhancing NVS via Set Diffusion](../3dgs_2026-03.md#enhancing-novel-view-synthesis-via-geometry-grounded-set-diffusion) | [2601.07540](https://arxiv.org/abs/2601.07540) | 几何接地集扩散 |
| 2026-03-11 | [Splat2Real](../3dgs_2026-03.md#splat2real-novel-view-scaling-for-physical-ai-with-3d-gaussian-splatting) | [2603.10638](https://arxiv.org/abs/2603.10638) | 物理 AI 新视角扩展 |
| 2026-03-10 | [ARSGaussian](../3dgs_2026-03.md#arsgaussian-3d-gaussian-splatting-with-lidar-for-aerial-remote-sensing-novel-view-synthesis) | [2412.18380](https://arxiv.org/abs/2412.18380) | 航拍遥感新视角，ISPRS |
| 2026-03-05 | [CylinderSplat](../3dgs_2026-03.md#cylindersplat-3d-gaussian-splatting-with-cylindrical-triplanes-for-panoramic-novel-view-synthesis) | [2603.05882](https://arxiv.org/abs/2603.05882) | 圆柱 Triplane 全景合成 |

**概要**: 从有限输入视角合成新视角，涵盖稀疏视角重建、全景渲染、扩散先验、几何接地等方向。

---

## 十、数字人与头像 {#cat-avatar}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-30 | [Relightable Holoported Characters](../3dgs_2026-03.md#relightable-holoported-characters-capturing-and-relighting-dynamic-human-performance-from-sparse-views) | [2512.00255](https://arxiv.org/abs/2512.00255) | 可重光照全息角色 |
| 2026-03-25 | ★ [HyperGaussians](../3dgs_2026-03.md#hypergaussians-high-dimensional-gaussian-splatting-for-high-fidelity-animatable-face-avatars) | [2507.02803](https://arxiv.org/abs/2507.02803) | 高维人脸头像，CVPR'26 |
| 2026-03-24 | [AGORA](../3dgs_2026-03.md#agora-adversarial-generation-of-real-time-animatable-3d-gaussian-head-avatars) | [2512.06438](https://arxiv.org/abs/2512.06438) | 对抗生成可动画头像 |
| 2026-03-23 | ★ [CrowdGaussian](../3dgs_2026-03.md#crowdgaussian-reconstructing-high-fidelity-3d-gaussians-for-human-crowd-from-a-single-image) | [2603.17779](https://arxiv.org/abs/2603.17779) | 单图人群重建，CVPR'26 |
| 2026-03-18 | [AHOY!](../3dgs_2026-03.md#ahoy-animatable-humans-under-occlusion-from-youtube-videos-with-gaussian-splatting-and-video-diffusion-priors) | [2603.17975](https://arxiv.org/abs/2603.17975) | 遮挡下可动画人体 |
| 2026-03-17 | [SMAL-pets](../3dgs_2026-03.md#smal-pets-smal-based-avatars-of-pets-from-single-image) | [2603.17131](https://arxiv.org/abs/2603.17131) | 单图宠物头像 |
| 2026-03-16 | [LHM++](../3dgs_2026-03.md#lhm-an-efficient-large-human-reconstruction-model-for-pose-free-images-to-3d) | [2506.13766](https://arxiv.org/abs/2506.13766) | 大人体重建模型 |
| 2026-03-11 | [SEGA](../3dgs_2026-03.md#sega-drivable-3d-gaussian-head-avatar-from-a-single-image) | [2504.14373](https://arxiv.org/abs/2504.14373) | 单图可驱动头像 |
| 2026-03-08 | [EmbedTalk](../3dgs_2026-03.md#embedtalk-triplane-free-talking-head-synthesis-using-embedding-driven-gaussian-deformation) | [2603.07604](https://arxiv.org/abs/2603.07604) | 无 Triplane 数字人 |
| 2026-03-05 | ★ [STAvatar](../3dgs_2026-03.md#stavatar-soft-binding-and-temporal-density-control-for-monocular-3d-head-avatars-reconstruction) | [2511.19854](https://arxiv.org/abs/2511.19854) | 软绑定头像，CVPR'26 |
| 2026-03-03 | [EmoTaG](../3dgs_2026-03.md#emotag-emotion-aware-talking-head-synthesis-on-gaussian-splatting-with-few-shot-personalization) | [2603.21332](https://arxiv.org/abs/2603.21332) | 情感感知数字人，CVPR'26 |
| 2026-03-02 | [LiftAvatar](../3dgs_2026-03.md#liftavatar-kinematic-space-completion-for-expression-controlled-3d-gaussian-avatar-animation) | [2603.02129](https://arxiv.org/abs/2603.02129) | 运动空间头像动画 |
| 2026-03-24 | [FaceParts](../3dgs_2026-03.md#faceparts-segmentation-and-editing-of-gaussian-splatting) | [2605.13853](https://arxiv.org/abs/2605.13853) | 人脸分割与编辑 |

**概要**: 基于 3DGS 的人脸/人体/数字人头像建模与动画，涵盖单图重建、表情/情感驱动、少样本个性化等方向。HyperGaussians 和 STAvatar 两篇 CVPR'26 论文分别实现高维高保真头像和软绑定重建。

---

## 十一、生成式模型与编辑 {#cat-generative}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-30 | [ObjectMorpher](../3dgs_2026-03.md#objectmopher-3d-aware-image-editing-via-deformable-3dgs-models) | [2603.28152](https://arxiv.org/abs/2603.28152) | 3D 感知图像编辑 |
| 2026-03-30 | [SVGS](../3dgs_2026-03.md#svgs-single-view-to-3d-object-editing-via-gaussian-splatting) | [2603.28126](https://arxiv.org/abs/2603.28126) | 单图到 3D 物体编辑 |
| 2026-03-27 | [Detailed Geometry from Opportunistic Motion](../3dgs_2026-03.md#detailed-geometry-and-appearance-from-opportunistic-motion) | [2603.26665](https://arxiv.org/abs/2603.26665) | 偶发运动 3D 重建 |
| 2026-03-20 | [3D-Consistent Multi-View Editing](../3dgs_2026-03.md#3d-consistent-multi-view-editing-by-correspondence-guidance) | [2511.22228](https://arxiv.org/abs/2511.22228) | 对应引导多视图编辑 |
| 2026-03-20 | [Pseudo-Simulation](../3dgs_2026-03.md#pseudo-simulation-for-autonomous-driving) | [2506.04218](https://arxiv.org/abs/2506.04218) | 自动驾驶伪仿真，CoRL'25 |
| 2026-03-23 | [3DSceneEditor](../3dgs_2026-03.md#3dsceneeditor-controllable-3d-scene-editing-with-gaussian-splatting) | [2412.01583](https://arxiv.org/abs/2412.01583) | 可控 3D 场景编辑，WACV'26 |
| 2026-03-16 | [IRIS](../3dgs_2026-03.md#iris-intersection-aware-ray-based-implicit-editable-scenes) | [2603.15368](https://arxiv.org/abs/2603.15368) | 可编辑隐式场景 |
| 2026-03-15 | [Direct Object-Level Reconstruction](../3dgs_2026-03.md#direct-object-level-reconstruction-via-probabilistic-gaussian-splatting) | [2603.14316](https://arxiv.org/abs/2603.14316) | 概率对象级重建 |
| 2026-03-14 | [Scene Generation at Absolute Scale](../3dgs_2026-03.md#scene-generation-at-absolute-scale-utilizing-semantic-and-geometric-guidance-from-text-for-accurate-and-interpretable-3d-indoor-scene-generation) | [2603.13910](https://arxiv.org/abs/2603.13910) | 文本引导绝对尺度场景生成 |
| 2026-03-14 | [GT2-GS](../3dgs_2026-03.md#gt2-gs-geometry-aware-texture-transfer-for-gaussian-splatting) | [2505.15208](https://arxiv.org/abs/2505.15208) | 几何感知纹理迁移，AAAI'26 |
| 2026-03-14 | [ABC-GS](../3dgs_2026-03.md#abc-gs-alignment-based-controllable-style-transfer-for-3d-gaussian-splatting) | [2503.22218](https://arxiv.org/abs/2503.22218) | 可控风格迁移，ICME'25 Oral |
| 2026-03-13 | [Variation-aware Flexible 3D Gaussian Editing](../3dgs_2026-03.md#variation-aware-flexible-3d-gaussian-editing) | [2602.11638](https://arxiv.org/abs/2602.11638) | 变化感知灵活编辑 |
| 2026-03-13 | [ExCellGen](../3dgs_2026-03.md#excellgen-fast-controllable-photorealistic-3d-scene-generation-from-a-single-real-world-exemplar) | [2412.16253](https://arxiv.org/abs/2412.16253) | 单图 3D 场景生成 |
| 2026-03-05 | [DiffusionHarmonizer](../3dgs_2026-03.md#diffusionharmonizer-bridging-neural-reconstruction-and-photorealistic-simulation-with-online-diffusion-enhancer) | [2602.24096](https://arxiv.org/abs/2602.24096) | 在线扩散增强 |
| 2026-03-05 | ★ [Text-to-3D by Stitching](../3dgs_2026-03.md#text-to-3d-by-stitching-a-multi-view-reconstruction-network-to-a-video-generator) | [2510.13454](https://arxiv.org/abs/2510.13454) | VIST3A 文本到 3D，ICLR'26 Oral |

**概要**: 使用扩散模型、自回归模型等生成式方法生成或编辑 3DGS 场景。VIST3A (ICLR'26 Oral) 将文本到视频模型与前馈 3D 重建系统结合，实现文本到 3D 场景生成。

---

## 十二、逆向渲染与重光照 {#cat-relighting}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-30 | ★ [SGS-Intrinsic](../3dgs_2026-03.md#sgs-intrinsic-semantic-invariant-gaussian-splatting-for-sparse-view-indoor-inverse-rendering) | [2603.27516](https://arxiv.org/abs/2603.27516) | 语义不变逆向渲染，CVPR'26 |
| 2026-03-27 | [R-PGA](../3dgs_2026-03.md#r-pga-robust-physical-adversarial-camouflage-generation-via-relightable-3d-gaussian-splatting) | [2603.26067](https://arxiv.org/abs/2603.26067) | 可重光照对抗伪装 |
| 2026-03-16 | ★ [MetaGS](../3dgs_2026-03.md#metags-a-meta-learned-gaussian-phong-model-for-out-of-distribution-3d-scene-relighting) | [2405.20791](https://arxiv.org/abs/2405.20791) | 元学习重光照，NeurIPS'25 Spotlight |
| 2026-03-03 | ★ [R3GW](../3dgs_2026-03.md#r3gw-relightable-3d-gaussians-for-outdoor-scenes-in-the-wild) | [2603.02801](https://arxiv.org/abs/2603.02801) | 户外场景重光照，VISAPP'26 |
| 2026-03-03 | ★ [VIRGi](../3dgs_2026-03.md#virgi-view-dependent-instant-recoloring-of-3d-gaussians-splats) | [2603.02986](https://arxiv.org/abs/2603.02986) | 视角依赖重着色，TPAMI'26 |

**概要**: 3DGS 上的逆向渲染和重光照，包括材质分解、光照估计、重光照、材质迁移等。

---

## 十三、医疗与工业应用 {#cat-medical-industrial}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-31 | [TUGS](../3dgs_2026-03.md#tugs-physics-based-compact-representation-of-underwater-scenes-by-tensorized-gaussian) | [2505.08811](https://arxiv.org/abs/2505.08811) | 张量高斯水下场景 |
| 2026-03-31 | [Moving Light Colonoscopy](../3dgs_2026-03.md#moving-light-adaptive-colonoscopy-reconstruction-via-illumination-attenuation-aware-3d-gaussian-splatting) | [2510.18739](https://arxiv.org/abs/2510.18739) | 结肠镜重建，ICME'26 |
| 2026-03-27 | [EOGS++](../3dgs_2026-03.md#eogs-earth-observation-gaussian-splatting-with-internal-camera-refinement-and-direct-panchromatic-rendering) | [2511.16542](https://arxiv.org/abs/2511.16542) | 地球观测 GS，ISPRS'26 |
| 2026-03-26 | [ArtPro](../3dgs_2026-03.md#artpro-self-supervised-articulated-object-reconstruction-with-adaptive-integration-of-mobility-proposals) | [2602.22666](https://arxiv.org/abs/2602.22666) | 自监督关节物体重建 |
| 2026-03-25 | [Instrument-Splatting++](../3dgs_2026-03.md#instrument-splatting-towards-controllable-surgical-instrument-digital-twin-using-gaussian-splatting) | [2603.22792](https://arxiv.org/abs/2603.22792) | 手术器械数字孪生 |
| 2026-03-20 | [Nevis Digital Twin](../3dgs_2026-03.md#nevis-digital-twin-photogrammetry-and-immersive-visualization-of-historical-sites) | [2603.20560](https://arxiv.org/abs/2603.20560) | 历史遗址数字孪生 |
| 2026-03-17 | [FreeGaussian](../3dgs_2026-03.md#freegaussian-annotation-free-control-of-articulated-objects-via-3d-gaussian-splats-with-flow-derivatives) | [2410.22070](https://arxiv.org/abs/2410.22070) | 免标注关节物体控制 |
| 2026-03-16 | [Three-Dimensional MRI Reconstruction](../3dgs_2026-03.md#three-dimensional-mri-reconstruction-with-gaussian-representations-tackling-the-undersampling-problem) | [2502.06510](https://arxiv.org/abs/2502.06510) | 3D MRI 重建 |
| 2026-03-13 | [TreeDGS](../3dgs_2026-03.md#treedgs-aerial-gaussian-splatting-for-distant-dbh-measurement) | [2601.12823](https://arxiv.org/abs/2601.12823) | 航拍树木测量 |
| 2026-03-12 | [4D Radar-Inertial Odometry](../3dgs_2026-03.md#4d-radar-inertial-odometry-based-on-gaussian-modeling-and-multi-hypothesis-scan-matching) | [2412.13639](https://arxiv.org/abs/2412.13639) | 4D 雷达惯性里程计 |
| 2026-03-09 | [SurgCalib](../3dgs_2026-03.md#surgcalib-gaussian-splatting-based-hand-eye-calibration-for-robot-assisted-minimally-invasive-surgery) | [2603.08983](https://arxiv.org/abs/2603.08983) | 手术机器人手眼标定 |
| 2026-03-06 | [ColonSplat](../3dgs_2026-03.md#colonsplat-reconstruction-of-peristaltic-motion-in-colonoscopy-with-dynamic-gaussian-splatting) | [2603.06860](https://arxiv.org/abs/2603.06860) | 结肠蠕动运动重建 |
| 2026-03-06 | [Active View Selection for CT](../3dgs_2026-03.md#active-view-selection-with-perturbed-gaussian-ensemble-for-tomographic-reconstruction) | [2603.06852](https://arxiv.org/abs/2603.06852) | CT 主动视角选择 |
| 2026-03-03 | [DSA-SRGS](../3dgs_2026-03.md#dsa-srgs-super-resolution-gaussian-splatting-for-dynamic-sparse-view-dsa-reconstruction) | [2603.04770](https://arxiv.org/abs/2603.04770) | 动态 DSA 超分重建 |
| 2026-03-02 | [Zero-shot CT SR](../3dgs_2026-03.md#zero-shot-ct-super-resolution-using-diffusion-based-2d-projection-priors-and-signed-3d-gaussians) | [2508.15151](https://arxiv.org/abs/2508.15151) | 零样本 CT 超分 |

**概要**: 3DGS 在医疗（内窥镜、CT/MRI、手术机器人）、工业（水下、遥感、历史遗址数字孪生、农业测量）等垂直领域的应用。

---

## 十四、视觉定位与水印安全 {#cat-loc-security}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-30 | ★ [Hierarchical Visual Relocalization](../3dgs_2026-03.md#hierarchical-visual-relocalization-with-nearest-view-synthesis-from-feature-gaussian-splatting) | [2603.29185](https://arxiv.org/abs/2603.29185) | 分层视觉重定位，CVPR'26 |
| 2026-03-19 | [Remove360](../3dgs_2026-03.md#remove360-benchmarking-residuals-after-object-removal-in-3d-gaussian-splatting) | [2508.11431](https://arxiv.org/abs/2508.11431) | 物体移除残差基准 |
| 2026-03-18 | ★ [ReLaGS](../3dgs_2026-03.md#relags-relational-language-gaussian-splatting) | [2603.17605](https://arxiv.org/abs/2603.17605) | 关系语言 GS，CVPR'26 |
| 2026-03-17 | ★ [Rethinking Pose Refinement](../3dgs_2026-03.md#rethinking-pose-refinement-in-3d-gaussian-splatting-under-pose-prior-and-geometric-uncertainty) | [2603.16538](https://arxiv.org/abs/2603.16538) | 位姿精炼，CVPR'26 |
| 2026-03-12 | [InstantSfM](../3dgs_2026-03.md#instantsfm-towards-gpu-native-sfm-for-the-deep-learning-era) | [2510.13310](https://arxiv.org/abs/2510.13310) | GPU 原生 SfM |
| 2026-03-09 | [S2D](../3dgs_2026-03.md#s2d-sparse-to-dense-lifting-for-3d-reconstruction-with-minimal-inputs) | [2603.10893](https://arxiv.org/abs/2603.10893) | 稀疏到密集提升 |
| 2026-03-07 | ★ [3DGS with Fisheye Images](../3dgs_2026-03.md#3d-gaussian-splatting-with-fisheye-images-field-of-view-analysis-and-depth-based-initialization) | [2508.06968](https://arxiv.org/abs/2508.06968) | 鱼眼图像 3DGS，VISAPP'26 |
| 2026-03-06 | [Gaussian Set Surface Reconstruction](../3dgs_2026-03.md#gaussian-set-surface-reconstruction-through-per-gaussian-optimization) | [2507.18923](https://arxiv.org/abs/2507.18923) | 高斯集表面重建 |
| 2026-03-04 | ★ [Where, What, Why: Explainable 3D-GS Watermarking](../3dgs_2026-03.md#where-what-why-toward-explainable-3d-gs-watermarking) | [2603.08809](https://arxiv.org/abs/2603.08809) | 可解释水印，CVPR'26 |
| 2026-03-03 | [Spectral Defense](../3dgs_2026-03.md#spectral-defense-against-resource-targeting-attack-in-3d-gaussian-splatting) | [2603.12796](https://arxiv.org/abs/2603.12796) | 频谱防御资源攻击 |

**概要**: 基于 3DGS 的视觉定位、位姿估计和 SfM，以及 3DGS 安全（水印、对抗攻击防御）相关研究。

---

## 十五、流媒体与编码 {#cat-streaming}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-15 | [LiDAR-EVS](../3dgs_2026-03.md#lidar-evs-enhance-extrapolated-view-synthesis-for-3d-gaussian-splatting-with-pseudo-lidar-supervision) | [2603.14763](https://arxiv.org/abs/2603.14763) | 伪 LiDAR 监督增强 |
| 2026-03-10 | [GSStream](../3dgs_2026-03.md#gsstream-3d-gaussian-splatting-based-volumetric-scene-streaming-system) | [2603.09718](https://arxiv.org/abs/2603.09718) | 体视频流式传输 |
| 2026-03-10 | [ProGS](../3dgs_2026-03.md#progs-towards-progressive-coding-for-3d-gaussian-splatting) | [2603.09703](https://arxiv.org/abs/2603.09703) | 渐进式编码 |
| 2026-03-09 | [HDR-NSFF](../3dgs_2026-03.md#hdr-nsff-high-dynamic-range-neural-scene-flow-fields) | [2603.08313](https://arxiv.org/abs/2603.08313) | HDR 神经场景流场，ICLR'26 |

**概要**: 3DGS 场景或动态 3DGS 的视频编码、流式传输和带宽优化。

---

## 十六、其他应用与交叉领域 {#cat-other}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-03-31 | [AA-Splat](../3dgs_2026-03.md#aasplat-anti-aliased-feed-forward-gaussian-splatting) | [2603.29394](https://arxiv.org/abs/2603.29394) | 抗锯齿前馈 GS |
| 2026-03-30 | [Efficient Camera Pose Augmentation](../3dgs_2026-03.md#efficient-camera-pose-augmentation-for-view-generalization-in-robotic-policy-learning) | [2603.29192](https://arxiv.org/abs/2603.29192) | 机器人策略视角增强 |
| 2026-03-29 | [GS3LAM](../3dgs_2026-03.md#gs3lam-gaussian-semantic-splatting-slam) | [2603.27781](https://arxiv.org/abs/2603.27781) | 语义 GS SLAM，ACM MM'24 |
| 2026-03-29 | ★ [NeAR](../3dgs_2026-03.md#near-coupled-neural-asset-renderer-stack) | [2511.18600](https://arxiv.org/abs/2511.18600) | 神经资产-渲染栈，CVPR'26 |
| 2026-03-27 | [GHOST](../3dgs_2026-03.md#ghost-fast-category-agnostic-hand-object-interaction-reconstruction-from-rgb-videos-using-gaussian-splatting) | [2603.18912](https://arxiv.org/abs/2603.18912) | 手物交互重建 |
| 2026-03-26 | [arg-VU](../3dgs_2026-03.md#arg-vu-affordance-reasoning-with-physics-aware-3d-geometry-for-visual-understanding-in-robotic-surgery) | [2603.26814](https://arxiv.org/abs/2603.26814) | 手术机器人可用性推理 |
| 2026-03-25 | [Let it Snow!](../3dgs_2026-03.md#let-it-snow-animating-3d-gaussian-scenes-with-dynamic-weather-effects-via-physics-guided-score-distillation) | [2504.05296](https://arxiv.org/abs/2504.05296) | 动态天气效果，CVPR'26 |
| 2026-03-24 | [PhotoAgent](../3dgs_2026-03.md#photoagent-a-robotic-photographer-with-spatial-and-aesthetic-understanding) | [2603.22796](https://arxiv.org/abs/2603.22796) | 机器人摄影师，ICRA'26 |
| 2026-03-22 | [SignSparK](../3dgs_2026-03.md#signspark-efficient-multilingual-sign-language-production-via-sparse-keyframe-learning) | [2603.10446](https://arxiv.org/abs/2603.10446) | 多语种手语生成 |
| 2026-03-20 | [GaussianPile](../3dgs_2026-03.md#gaussianpile-a-unified-sparse-gaussian-splatting-framework-for-slice-based-volumetric-reconstruction) | [2603.20611](https://arxiv.org/abs/2603.20611) | 切片体素重建，CVPR'26 |
| 2026-03-15 | [In-Field 3D Wheat Head Segmentation](../3dgs_2026-03.md#in-field-3d-wheat-head-instance-segmentation-from-tls-point-clouds-using-deep-learning-without-manual-labels) | [2603.14309](https://arxiv.org/abs/2603.14309) | 小麦头 3D 分割，ISPRS'26 |
| 2026-03-12 | [EMGauss](../3dgs_2026-03.md#emgauss-continuous-slice-to-3d-reconstruction-via-dynamic-gaussian-modeling-in-volume-electron-microscopy) | [2512.06684](https://arxiv.org/abs/2512.06684) | 电子显微镜 3D 重建，CVPR'26 |
| 2026-03-08 | ★ [MUGSQA](../3dgs_2026-03.md#mugsqa-novel-multi-uncertainty-based-gaussian-splatting-quality-assessment-method-dataset-and-benchmarks) | [2511.06830](https://arxiv.org/abs/2511.06830) | 质量评估，ICASSP'26 |
| 2026-03-08 | [Observer-Actor](../3dgs_2026-03.md#observer-actor-active-vision-imitation-learning-with-sparse-view-gaussian-splatting) | [2511.18140](https://arxiv.org/abs/2511.18140) | 主动视觉模仿学习，ICRA'26 |
| 2026-03-07 | ★ [Phys2Real](../3dgs_2026-03.md#phys2real-fusing-vlm-priors-with-interactive-online-adaptation-for-uncertainty-aware-sim-to-real-manipulation) | [2510.11689](https://arxiv.org/abs/2510.11689) | 仿到真 RL，ICRA'26 |
| 2026-03-05 | [FTSplat](../3dgs_2026-03.md#ftsplat-feed-forward-triangle-splatting-network) | [2603.05932](https://arxiv.org/abs/2603.05932) | 前馈三角形溅射 |
| 2026-03-02 | [Learning Convex Decomposition](../3dgs_2026-03.md#learning-convex-decomposition-via-feature-fields) | [2603.09285](https://arxiv.org/abs/2603.09285) | 凸分解特征场 |

**概要**: 上述类别未涵盖的交叉领域应用，包括机器人策略学习、手语生成、天气效果模拟、质量评估、仿到真迁移、凸分解等。

---

## 统计概览

| 类别 | 论文数 |
|------|--------|
| 核心算法与优化 | 16 |
| 前馈 3DGS 与可泛化方法 | 18 |
| 动态场景与 4D 重建 | 19 |
| SLAM 与机器人导航 | 13 |
| 自动驾驶与交通场景 | 9 |
| 语义分割与场景理解 | 19 |
| 几何与表面重建 | 16 |
| 渲染加速与压缩 | 8 |
| 新视角合成 | 8 |
| 数字人与头像 | 13 |
| 生成式模型与编辑 | 15 |
| 逆向渲染与重光照 | 5 |
| 医疗与工业应用 | 16 |
| 视觉定位与水印安全 | 10 |
| 流媒体与编码 | 4 |
| 其他应用与交叉领域 | 16 |
| **合计** | **185** |

> 注：月度文件中共 180 篇论文，部分论文因跨领域被归入两个类别，故合计略高。
