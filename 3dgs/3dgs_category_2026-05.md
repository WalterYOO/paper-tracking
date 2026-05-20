# 3D Gaussian Splatting 论文分类索引 (2026-05)

> 基于 `3dgs_2026-05.md` 中收集的论文，按研究方向细分类。
> ★ 表示被顶会/顶刊录用。

## 目录

- [一、核心算法与优化](#cat-core-opt)
- [二、渲染加速与压缩](#cat-render-accel)
- [三、新视角合成](#cat-nvs)
  - [3.1 可泛化 / 前向](#cat-nvs-generalizable)
  - [3.2 稀疏视角](#cat-nvs-sparse)
- [四、动态场景与 4D](#cat-dynamic-4d)
- [五、语义分割与场景理解](#cat-seg-understand)
- [六、视觉定位](#cat-visloc)
- [七、几何与表面重建](#cat-geo-recon)
- [八、逆渲染与光照](#cat-invrender)
- [九、生成式模型](#cat-generative)
- [十、流媒体与编码](#cat-streaming)
- [十一、无线与射频传播](#cat-wireless)
- [十二、安全与版权](#cat-security)
- [十三、自动驾驶应用](#cat-ads)
- [十四、机器人、SLAM 与具身智能](#cat-robotics)
- [十五、其他应用](#cat-other)

---

## 一、核心算法与优化 {#cat-core-opt}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-15 | [Learn2Splat](#3-learn2splat-extending-the-horizon-of-learned-3dgs-optimization) | 2605.15760 | 学习型优化器，元学习 |
| 2026-05-14 | [Denoising-GS](#3-denoising-gs-gaussian-splatting-with-spatial-aware-denoising) | 2605.14880 | 空间感知去噪，冗余基元裁剪 |
| 2026-05-14 | [Skew-Normal Splatting](#5-3d-skew-normal-splatting) | 2605.15010 | 偏态正态核，非对称基元 |
| 2026-05-11 | [PG-3DGS](#1-pg-3dgs-optimizing-3d-gaussian-splatting-to-satisfy-physics-objectives) | 2605.11266 | 可微物理模拟引导优化 |
| 2026-05-09 | [ReorgGS](#2-reorggs-equivalent-distribution-reorganization-for-3d-gaussian-splatting) | 2605.08739 | 分布重组，抑制浮动伪影 |
| 2026-05-08 | [AV1 Motion Vector for 3DGS](#2-efficient-dense-matching-for-enhanced-gaussian-splatting-using-av1-motion-vectors) | 2605.14629 | AV1 运动向量替代穷举匹配 |
| 2026-05-07 | [AdpSplit](#1-adpsplit-error-driven-adaptive-splitting-for-faster-geometry-discovery-in-3d-gaussian-splatting) | 2605.06876 | 误差驱动自适应分裂 |
| 2026-05-01 | [LeGS](#2-beyond-heuristics-learnable-density-control-for-3d-gaussian-splatting) | 2605.00408 | 强化学习密度控制 |

**概要**: 改进 3DGS 基础优化过程，包括优化器设计、密度控制、基元分裂/裁剪策略、基元分布模型等。

---

## 二、渲染加速与压缩 {#cat-render-accel}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-18 | [TensorGS](#2-accelerating-3d-gaussian-splatting-using-tensor-cores-tensorgs) | 2605.17855 | Tensor Core 张量化，1.65x 加速 |
| 2026-05-12 | [3DGS³](#4-3dgs-cubed-joint-super-sampling-and-frame-interpolation-for-real-time-large-scale-3dgs-rendering) | 2605.11489 | 超采样+帧插值，后处理框架 |
| 2026-05-06 | [QuadBox](#3-quadbox-accelerating-3d-gaussian-splatting-with-geometry-aware-boxes) | 2605.04844 | 几何感知包围盒，1.85x 加速 |
| 2026-05-03 | [GETA-3DGS](#2-geta-3dgs-automatic-joint-structured-pruning-and-quantization-for-3d-gaussian-splatting) | 2605.02086 | 联合剪枝+量化，~5x 压缩 |

**概要**: 提升 3DGS 渲染性能或降低存储开销，包括硬件加速、包围盒裁剪、剪枝量化、后处理超采样等。

---

## 三、新视角合成 {#cat-nvs}

### 3.1 可泛化 / 前向 {#cat-nvs-generalizable}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-13 | [RoSplat](#4-rosplat-robust-feed-forward-pixel-wise-gaussian-splatting-for-varying-input-views-and-high-resolution-rendering) | 2605.13093 | alpha 归一化，多视角鲁棒 |
| 2026-05-13 | ★ **[Z-Order Transformer for 3DGS](#5-z-order-transformer-for-feed-forward-gaussian-splatting)** | 2605.13465 | Z 序稀疏注意力，单次前向 (CVPR'26 Oral) |
| 2026-05-11 | [AdaptSplat](#2-adaptsplat-adapting-vision-foundation-models-for-feed-forward-3d-gaussian-splatting) | 2605.10239 | 频率保持适配器，1.5M 参数 |
| 2026-05-10 | [ConFixGS](#1-confixgs-learning-to-fix-feedforward-3d-gaussian-splatting-with-confidence-aware-diffusion-priors-in-driving-scenes) | 2605.09688 | 置信感知扩散修复 |
| 2026-05-08 | [SplatWeaver](#8-splatweaver-learning-to-allocate-gaussian-primitives-for-generalizable-novel-view-synthesis) | 2605.07287 | 动态基元分配，像素级路由 |
| 2026-05-06 | [Ground4D](#6-ground4d-spatially-grounded-feedforward-4d-reconstruction-for-unstructured-off-road-scenes) | 2605.04435 | 空间锚定前向 4D，越野场景 |

### 3.2 稀疏视角 {#cat-nvs-sparse}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-13 | [PanoPlane](#1-panoplane-plane-aware-panoramic-completion-for-sparse-view-indoor-3d-gaussian-splatting) | 2605.14135 | 平面感知全景补全，3 视图 SOTA |
| 2026-05-12 | [PairDropGS](#7-pairdropgs-paired-dropout-induced-consistency-regularization-for-sparse-view-gaussian-splatting) | 2605.12072 | 成对 Dropout 一致性正则化 |
| 2026-05-12 | ★ **[GeoQuery](#8-geoquery-geometry-query-diffusion-for-sparse-view-reconstruction)** | 2605.12399 | 几何引导扩散修复伪像 (SIGGRAPH'26) |
| 2026-05-08 | [SatSurfGS](#2-satsurfgs-generalizable-2d-gaussian-splatting-for-sparse-view-satellite-surface-reconstruction) | 2605.07181 | 2DGS 可泛化卫星表面重建 |

**概要**: 无需逐场景优化即可合成新视角（可泛化/前向方法），或从极少输入视角重建场景（稀疏视角方法）。

---

## 四、动态场景与 4D {#cat-dynamic-4d}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-17 | [GEM](#1-gem-gaussian-evolution-model-for-occupancy-forecasting-and-motion-planning) | 2605.17682 | 非自回归 4D 世界模型，占用预测 |
| 2026-05-12 | ★ **[Retrospective Dynamic NVS](#3-3d-gaussian-splatting-for-efficient-retrospective-dynamic-scene-novel-view-synthesis-with-a-standardized-benchmark)** | 2605.12437 | 同步多视图回溯重建 (CVPR'26) |
| 2026-05-11 | [DySurface](#4-dysurface-consistent-4d-surface-reconstruction-via-bridging-explicit-gaussians-and-implicit-functions) | 2605.10360 | 显式高斯+隐式 SDF 桥接 |
| 2026-05-05 | [FreeTimeGS++](#1-freetimesgs-secrets-of-dynamic-gaussian-splatting-and-their-principles) | 2605.03337 | 4DGS 关键因子分析，门控边缘化 |

**概要**: 处理随时间变化的动态场景，包括 4D 高斯表示、动态表面重建、时序一致性等。

---

## 五、语义分割与场景理解 {#cat-seg-understand}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-15 | [Prior-Guided 3DGS Segmentation](#1-robust-prior-guided-segmentation-for-editable-3d-gaussian-splatting) | 2605.16065 | SAM-HQ 先验引导，多视角一致分割 |
| 2026-05-13 | [SCOUP](#6-sparse-code-uplifting-for-efficient-3d-language-gaussian-splatting) | 2605.13600 | 稀疏码本提升，训练提速 400x |
| 2026-05-12 | ★ **[PointGS](#2-pointgs-semantic-consistent-unsupervised-3d-point-cloud-segmentation-with-3d-gaussian-splatting)** | 2605.11520 | 3DGS 桥接 2D-3D 语义迁移 (CVPR'26) |
| 2026-05-10 | ★ **[BEA-GS](#4-bea-gs-beyond-radiance-supervision-in-3dgs-for-precise-object-extraction)** | 2605.09662 | 超越辐射监督的精确物体提取 (CVPR'26 Highlight) |
| 2026-05-07 | [OpenGaFF](#2-opengaff-open-vocabulary-gaussian-feature-field-with-codebook-attention) | 2605.06088 | 码本注意力，开放词汇特征场 |
| 2026-05-06 | [Ilov3Splat](#2-ilov3splat-instance-level-open-vocabulary-3d-scene-understanding-in-gaussian-splatting) | 2605.04506 | 实例级开放词汇场景理解 |
| 2026-05-03 | ★ **[GLMap](#3-multi-scale-gaussian-language-map-for-zero-shot-embodied-navigation-and-reasoning)** | 2605.01736 | 多尺度高斯-语言地图 (CVPR'26) |

**概要**: 3DGS 上的语义分割、开放词汇场景理解、语言 grounding 和物体级提取。

---

## 六、视觉定位 {#cat-visloc}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-18 | [LiteLoc](#3-efficient-sparse-to-dense-visual-localization-via-compact-gaussian-scene-representation-and-accelerated-dense-pose-estimation-liteloc) | 2605.17777 | 去除颜色场减 94% 存储，PnP 蒸馏 19x |
| 2026-05-12 | [PoseCompass](#5-posecompass-intelligent-synthetic-pose-selection-for-visual-localization) | 2605.12144 | 3DGS 合成位姿智能筛选 |
| 2026-05-08 | [SplitGS-Loc](#4-disambiguating-2d-3d-correspondences-in-gaussian-splatting-based-feature-fields-for-visual-localization) | 2605.07351 | 高斯分裂消歧 2D-3D 对应 |
| 2026-05-06 | ★ **[ULF-Loc](#5-ulf-loc-unbiased-landmark-feature-for-robust-visual-localization-with-3d-gaussian-splatting)** | 2605.04730 | 无偏地标特征 (CVPR'26 Highlight) |

**概要**: 基于 3DGS 场景表示的视觉定位，包括紧凑场景表示、特征场、2D-3D 匹配消歧等。

---

## 七、几何与表面重建 {#cat-geo-recon}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-16 | ★ **[P2GS](#3-p2gs-physical-prior-guided-gaussian-splatting-for-photometrically-consistent-urban-reconstruction)** | 2605.16925 | 物理先引导光度一致重建 (CVPR'26) |
| 2026-05-13 | [HarmoGS](#2-harmogs-robust-3d-gaussian-splatting-in-the-wild-via-conflict-aware-gradient-harmonization) | 2605.13073 | 冲突感知梯度调和，野生场景 |
| 2026-05-08 | [High-Fidelity Surface Splatting](#6-high-fidelity-surface-splatting-based-3d-reconstruction-from-multi-view-images) | 2605.07254 | 多项式核 IMLS，高频几何保真 |
| 2026-05-08 | [AsyncEvGS](#3-asyncevs-asynchronous-event-assisted-gaussian-splatting-for-handheld-motion-blurred-scenes) | 2605.07192 | 异步事件辅助，运动模糊场景 |
| 2026-05-02 | ★ **[SplAttN](#1-splatttn-bridging-2d-and-3d-with-gaussian-soft-splatting-and-attention-for-point-cloud-completion)** | 2605.01466 | 高斯软光栅化，点云补全 (ICML'26 Spotlight) |
| 2026-05-01 | [2D-SuGaR](#1-2d-sugar-surface-aware-gaussian-splatting-for-geometrically-accurate-mesh-reconstruction) | 2605.00569 | 单目深度法线先验增强 2DGS |

**概要**: 从图像重建几何准确的表面、网格或点云，包括表面光栅化、高频细节恢复、多传感器融合等。

---

## 八、逆渲染与光照 {#cat-invrender}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-09 | [Relightable GS for VP](#1-relightable-gaussian-splatting-for-virtual-production-using-image-based-illumination) | 2605.09024 | 基于图像照明的重光照 |
| 2026-05-07 | [3DSS](#3-3dss-3d-surface-splatting-for-inverse-rendering) | 2605.05876 | 首个表面光栅化可微逆渲染器 |
| 2026-05-01 | [GOR-IS](#3-gor-is-3d-gaussian-object-removal-in-the-intrinsic-space) | 2605.00498 | 内秉空间物体移除，全局光照一致 |

**概要**: 从渲染结果反推材质、光照、形状等内秉属性，或实现物理一致的重光照。

---

## 九、生成式模型 {#cat-generative}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-18 | [PanoWorld](#1-panoworld-a-generative-spatial-world-model-for-consistent-whole-house-panorama-synthesis) | 2605.17916 | 自回归全屋全景生成，3DGS 空间记忆 |
| 2026-05-08 | ★ **[DeG](#7-generative-3d-gaussians-with-learned-density-control)** | 2605.16355 | Octree+扩散模型，学习密度控制 (SIGGRAPH'26) |
| 2026-05-14 | [3DEditSafe](#4-3d-editsafe-defending-3d-editing-pipelines-from-unsafe-generation) | 2605.15398 | 3DGS 文本驱动编辑安全防御 |

**概要**: 使用扩散模型、自回归模型等生成式方法生成或编辑 3DGS 场景。

---

## 十、流媒体与编码 {#cat-streaming}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-16 | [DSGS](#2-a-single-atlas-is-all-you-need-decoder-side-gaussian-splatting-for-immersive-video) | 2605.17002 | 解码端前向 3DGS，沉浸式视频 |
| 2026-05-10 | ★ **[CAGS](#2-cags-color-adaptive-volumetric-video-streaming-with-dynamic-3d-gaussian-splatting)** | 2605.09279 | 矢量量化+颜色自适应，体视频流 (SIGGRAPH'26) |
| 2026-05-09 | [TIGAS](#4-thin-client-interactive-gaussian-adaptive-streaming-over-http3) | 2605.08699 | HTTP/3 轻量端自适应流式传输 |

**概要**: 3DGS 场景或动态 3DGS 的视频编码、流式传输和带宽优化。

---

## 十一、无线与射频传播 {#cat-wireless}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-14 | [Eff-WRFGS](#1-eff-wrfgs-efficient-wireless-radiance-field-using-3d-gaussian-splatting) | 2605.15324 | 可学习掩码裁剪，存储减 44x |
| 2026-05-12 | [XFreq-GS](#1-xfreq-gs-cross-frequency-wireless-radiation-field-reconstruction-with-3d-gaussian-splatting) | 2605.11432 | 共享几何+频率自适应，跨频率泛化 |
| 2026-05-08 | [Differentiable Ray Tracing](#5-differentiable-ray-tracing-with-gaussians-for-unified-radio-propagation-simulation-and-view-synthesis) | 2605.07781 | 高斯可微光线追踪，统一射频+视图 |

**概要**: 将 3DGS 用于无线信道辐射场建模和射频传播仿真。

---

## 十二、安全与版权 {#cat-security}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-13 | [GuardMarkGS](#3-guardmarkgs-unified-ownership-tracing-and-edit-deterrence-for-3d-gaussian-splatting) | 2605.12919 | 统一水印追踪与编辑威慑 |

**概要**: 3DGS 资产的版权保护、水印和编辑安全。

---

## 十三、自动驾驶应用 {#cat-ads}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-12 | [PointForward](#6-pointforward-feedforward-driving-reconstruction-through-point-aligned-representations) | 2605.11594 | 空间稀疏查询，前向驾驶重建 |
| 2026-05-09 | [REAP](#3-reap-reinforcement-learning-end-to-end-autonomous-parking-with-gaussian-splatting-simulator-for-real2sim2real-transfer) | 2605.08713 | 3DGS 模拟器，RL 端到端泊车 |
| 2026-05-03 | [3DGS for ADS Editing](#1-from-concept-to-capability-evaluating-3d-gaussian-splatting-for-synthetic-scene-editing-in-autonomous-driving) | 2605.01995 | 合成场景编辑 fidelity 评估 |

**概要**: 3DGS 在自动驾驶场景重建、合成数据生成、场景编辑和仿真中的应用。

---

## 十四、机器人、SLAM 与具身智能 {#cat-robotics}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-11 | [MAGS-SLAM](#5-mags-slam-monocular-multi-agent-gaussian-splatting-slam-for-geometrically-and-photometrically-consistent-reconstruction) | 2605.10760 | 仅 RGB 多智能体 3DGS SLAM |
| 2026-05-11 | [VEGA](#6-vega-visual-encoder-grounding-alignment-for-spatially-aware-vision-language-action-models) | 2605.10485 | 3DGS 监督 VLA 空间感知对齐 |
| 2026-05-02 | [DMP for IL](#2-a-principled-approach-for-creating-high-fidelity-synthetic-demonstrations-for-imitation-learning) | 2605.01232 | 3DGS 场景+DMP 模仿学习演示 |
| 2026-05-02 | [TAIL-Safe](#3-tail-safe-task-agnostic-safety-monitoring-for-imitation-learning-policies) | 2605.01195 | 3DGS 数字孪生，安全监控 IL |

**概要**: 3DGS 在机器人 SLAM、模仿学习、具身导航和操作任务中的应用。

---

## 十五、其他应用 {#cat-other}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-17 | [GEM](#1-gem-gaussian-evolution-model-for-occupancy-forecasting-and-motion-planning) * | 2605.17682 | 4D 世界模型，占用预测+规划 |
| 2026-05-16 | [Topo-GS](#1-topo-gs-continuous-volumetric-embedding-of-high-dimensional-data-via-topological-gaussian-splatting) | 2605.17011 | 3DGS 复用于降维可视化 |
| 2026-05-11 | [SDTalk](#3-sdtalk-structured-facial-priors-and-dual-branch-motion-fields-for-generalizable-gaussian-talking-head-synthesis) | 2605.09956 | 单帧可泛化说话人头合成 |
| 2026-05-10 | [LagrangianSplats](#3-lagrangiansplats-divergence-free-transport-of-gaussian-primitives-for-fluid-reconstruction) | 2605.09299 | 无散度核，流体场重建 |
| 2026-05-10 | [FrameTwin](#5-frametwin-curve-anchored-gaussian-alignment-from-sparse-views-for-adaptive-wireframe-3d-printing) | 2605.09362 | 曲线锚定高斯，自适应线框 3D 打印 |
| 2026-05-08 | [GD-DIFF](#1-from-pixels-to-primitives-scene-change-detection-in-3d-gaussian-splatting) | 2605.07203 | 基元属性级场景变化检测 |
| 2026-05-06 | [CoherentRaster](#1-coherentraster-efficient-3d-gaussian-splatting-for-light-field-displays) | 2605.04509 | 子像素光栅化，光场显示 |
| 2026-05-06 | [Aes3D](#4-aes3d-aesthetic-assessment-in-3d-gaussian-splatting) | 2605.05155 | 3DGS 场景美学评估框架 |
| 2026-05-04 | [HumanSplatHMR](#1-humansplathmr-closing-the-loop-between-human-mesh-recovery-and-gaussian-splatting-avatar) | 2605.02784 | 姿态估计+数字人渲染闭环 |

* GEM 同时在"动态场景与 4D"中列出。

**概要**: 3DGS 在其他领域的应用扩展，包括数字人、流体模拟、3D 打印、变化检测、光场显示、美学评估和数据可视化等。

---

## 统计概览

| 类别 | 论文数 |
|------|--------|
| 核心算法与优化 | 8 |
| 新视角合成 | 10 |
| 几何与表面重建 | 6 |
| 语义分割与场景理解 | 7 |
| 动态场景与 4D | 4 |
| 视觉定位 | 4 |
| 渲染加速与压缩 | 4 |
| 自动驾驶应用 | 3 |
| 机器人、SLAM 与具身智能 | 4 |
| 生成式模型 | 3 |
| 流媒体与编码 | 3 |
| 无线与射频传播 | 3 |
| 逆渲染与光照 | 3 |
| 安全与版权 | 1 |
| 其他应用 | 9 |
| **合计（含重复）** | **65** |

> 注：GEM 同时归属"动态场景与 4D"和"其他应用"，故合计为 65 而非 60。原始论文总数为 60 篇（5 月 1 日至 5 月 18 日）。
