# 3D Gaussian Splatting 论文分类索引 (2026-05)

> 基于 `3dgs_2026-05.md` 中收集的论文，按研究方向细分类。
> ★ 表示被顶会/顶刊录用。

## 目录

- [一、核心算法与优化](3dgs_2026-05.md#cat-core-opt)
- [二、渲染加速与压缩](3dgs_2026-05.md#cat-render-accel)
- [三、新视角合成](3dgs_2026-05.md#cat-nvs)
  - [3.1 可泛化 / 前向](3dgs_2026-05.md#cat-nvs-generalizable)
  - [3.2 稀疏视角](3dgs_2026-05.md#cat-nvs-sparse)
- [四、动态场景与 4D](3dgs_2026-05.md#cat-dynamic-4d)
- [五、语义分割与场景理解](3dgs_2026-05.md#cat-seg-understand)
- [六、视觉定位](3dgs_2026-05.md#cat-visloc)
- [七、几何与表面重建](3dgs_2026-05.md#cat-geo-recon)
- [八、逆渲染与光照](3dgs_2026-05.md#cat-invrender)
- [九、生成式模型](3dgs_2026-05.md#cat-generative)
- [十、流媒体与编码](3dgs_2026-05.md#cat-streaming)
- [十一、无线与射频传播](3dgs_2026-05.md#cat-wireless)
- [十二、安全与版权](3dgs_2026-05.md#cat-security)
- [十三、自动驾驶应用](3dgs_2026-05.md#cat-ads)
- [十四、机器人、SLAM 与具身智能](3dgs_2026-05.md#cat-robotics)
- [十五、其他应用](3dgs_2026-05.md#cat-other)

---

## 一、核心算法与优化 {#cat-core-opt}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-20 | ★ **[CAdam](3dgs_2026-05.md#3-cadam-context-adaptive-moment-estimation-for-3d-gaussian-densification-in-generative-distillation)** | 2605.20872 | 上下文自适应密度控制，基元数减 85-97% (SIGGRAPH'26) |
| 2026-05-18 | [3D Skew Gaussian Splatting](3dgs_2026-05.md#6-3d-skew-gaussian-splatting-with-any-camera-trajectory-visualization-engine) | 2605.18334 | 偏态高斯基元，任意相机轨迹可视化引擎 |
| 2026-05-19 | [TideGS](3dgs_2026-05.md#2-tidegs-scalable-training-of-over-one-billion-3d-gaussian-splatting-primitives-via-out-of-core-optimization) | 2605.20150 | 超十亿基元 out-of-core 训练 |
| 2026-05-15 | [Learn2Splat](3dgs_2026-05.md#3-learn2splat-extending-the-horizon-of-learned-3dgs-optimization) | 2605.15760 | 学习型优化器，元学习 |
| 2026-05-14 | [Denoising-GS](3dgs_2026-05.md#3-denoising-gs-gaussian-splatting-with-spatial-aware-denoising) | 2605.14880 | 空间感知去噪，冗余基元裁剪 |
| 2026-05-14 | [Skew-Normal Splatting](3dgs_2026-05.md#5-3d-skew-normal-splatting) | 2605.15010 | 偏态正态核，非对称基元 |
| 2026-05-11 | [PG-3DGS](3dgs_2026-05.md#1-pg-3dgs-optimizing-3d-gaussian-splatting-to-satisfy-physics-objectives) | 2605.11266 | 可微物理模拟引导优化 |
| 2026-05-09 | [ReorgGS](3dgs_2026-05.md#2-reorggs-equivalent-distribution-reorganization-for-3d-gaussian-splatting) | 2605.08739 | 分布重组，抑制浮动伪影 |
| 2026-05-08 | [AV1 Motion Vector for 3DGS](3dgs_2026-05.md#2-efficient-dense-matching-for-enhanced-gaussian-splatting-using-av1-motion-vectors) | 2605.14629 | AV1 运动向量替代穷举匹配 |
| 2026-05-07 | [AdpSplit](3dgs_2026-05.md#1-adpsplit-error-driven-adaptive-splitting-for-faster-geometry-discovery-in-3d-gaussian-splatting) | 2605.06876 | 误差驱动自适应分裂 |
| 2026-05-07 | ★ **[AdamW-GS](3dgs_2026-05.md#5-a-step-to-decouple-optimization-in-3dgs)** | 2601.16736 | 优化解耦分析，AdamW-GS 优化器 (ICLR'26) |
| 2026-05-01 | [LeGS](3dgs_2026-05.md#2-beyond-heuristics-learnable-density-control-for-3d-gaussian-splatting) | 2605.00408 | 强化学习密度控制 |

**概要**: 改进 3DGS 基础优化过程，包括优化器设计、密度控制、基元分裂/裁剪策略、基元分布模型等。

---

## 二、渲染加速与压缩 {#cat-render-accel}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-19 | [Lattice VQ for 3DGS](3dgs_2026-05.md#7-improving-3d-gaussian-splatting-compression-by-scene-adaptive-lattice-vector-quantization) | 2509.13482 | 场景自适应格点矢量量化 |
| 2026-05-18 | [MMGS](3dgs_2026-05.md#4-mmgs-104-compressed-3dgs-through-optimal-transport-aggregation-based-on-multi-view-ranking) | 2605.19304 | 最优传输聚合，10 倍压缩，仅留 10% 基元 |
| 2026-05-18 | [TensorGS](3dgs_2026-05.md#2-accelerating-3d-gaussian-splatting-using-tensor-cores-tensorgs) | 2605.17855 | Tensor Core 张量化，1.65x 加速 |
| 2026-05-12 | [3DGS³](3dgs_2026-05.md#4-3dgs-cubed-joint-super-sampling-and-frame-interpolation-for-real-time-large-scale-3dgs-rendering) | 2605.11489 | 超采样+帧插值，后处理框架 |
| 2026-05-06 | [QuadBox](3dgs_2026-05.md#3-quadbox-accelerating-3d-gaussian-splatting-with-geometry-aware-boxes) | 2605.04844 | 几何感知包围盒，1.85x 加速 |
| 2026-05-07 | [MesonGS++](3dgs_2026-05.md#4-mesongs-post-training-compression-of-3d-gaussian-splatting-with-hyperparameter-searching) | 2604.26799 | 后训练压缩超参数搜索，34x 压缩 |
| 2026-05-03 | [GETA-3DGS](3dgs_2026-05.md#2-geta-3dgs-automatic-joint-structured-pruning-and-quantization-for-3d-gaussian-splatting) | 2605.02086 | 联合剪枝+量化，~5x 压缩 |
| 2026-05-09 | [NiFi](3dgs_2026-05.md#6-nix-and-fix-targeting-1000x-compression-of-3d-gaussian-splatting-with-diffusion-models) | 2602.04549 | 扩散模型一步蒸馏，1000x 压缩 |
| 2026-05-09 | ★ **[Turbo-GS](3dgs_2026-05.md#7-turbo-gs-accelerating-3d-gaussian-fitting-for-high-quality-radiance-fields)** | 2412.13547 | 稀释渲染+收敛感知预算 (CVPR'26) |

**概要**: 提升 3DGS 渲染性能或降低存储开销，包括硬件加速、包围盒裁剪、剪枝量化、后处理超采样等。

---

## 三、新视角合成 {#cat-nvs}

### 3.1 可泛化 / 前向 {#cat-nvs-generalizable}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-22 | ★ **[GlowGS](3dgs_2026-05.md#2-glowgs-generative-semantic-feature-learning-for-3d-gaussian-splatting-in-nighttime-glow-scenes)** | 2605.23602 | 夜间光晕场景，扩散模型+VFM 语义特征 (CVPR Findings'26) |
| 2026-05-22 | ★ **[LangFlash](3dgs_2026-05.md#3-langflash-feed-forward-3d-language-gaussian-splatting-from-sparse-unposed-images)** | 2605.23287 | 前向 3D 语言高斯拼接，无需位姿 (CVPR Findings'26) |
| 2026-05-13 | ★ **[SkySplat](3dgs_2026-05.md#8-skysplat-generalizable-3d-gaussian-splatting-from-multi-temporal-sparse-satellite-images)** | 2508.09479 | 多时相稀疏卫星图像可泛化 3DGS (AAAI'26) |
| 2026-05-21 | [ForeSplat](3dgs_2026-05.md#4-foresplat-optimization-aware-foresight-for-feed-forward-3d-gaussian-splatting) | 2605.22020 | 优化感知前向训练，元梯度加速收敛 |
| 2026-05-19 | [Cross-View Splatter](3dgs_2026-05.md#5-cross-view-splatter-feed-forward-view-synthesis-with-georeferenced-images) | 2605.19656 | 卫星+街景融合，地理参考前向合成 |
| 2026-05-13 | [RoSplat](3dgs_2026-05.md#4-rosplat-robust-feed-forward-pixel-wise-gaussian-splatting-for-varying-input-views-and-high-resolution-rendering) | 2605.13093 | alpha 归一化，多视角鲁棒 |
| 2026-05-13 | ★ **[Z-Order Transformer for 3DGS](3dgs_2026-05.md#5-z-order-transformer-for-feed-forward-gaussian-splatting)** | 2605.13465 | Z 序稀疏注意力，单次前向 (CVPR'26 Oral) |
| 2026-05-11 | [AdaptSplat](3dgs_2026-05.md#2-adaptsplat-adapting-vision-foundation-models-for-feed-forward-3d-gaussian-splatting) | 2605.10239 | 频率保持适配器，1.5M 参数 |
| 2026-05-10 | [ConFixGS](3dgs_2026-05.md#1-confixgs-learning-to-fix-feedforward-3d-gaussian-splatting-with-confidence-aware-diffusion-priors-in-driving-scenes) | 2605.09688 | 置信感知扩散修复 |
| 2026-05-08 | [SplatWeaver](3dgs_2026-05.md#8-splatweaver-learning-to-allocate-gaussian-primitives-for-generalizable-novel-view-synthesis) | 2605.07287 | 动态基元分配，像素级路由 |
| 2026-05-09 | ★ **[Turbo-GS](3dgs_2026-05.md#7-turbo-gs-accelerating-3d-gaussian-fitting-for-high-quality-radiance-fields)** | 2412.13547 | 稀释渲染+收敛感知预算，加速 3DGS 拟合 (CVPR'26) |
| 2026-05-06 | [Ground4D](3dgs_2026-05.md#6-ground4d-spatially-grounded-feedforward-4d-reconstruction-for-unstructured-off-road-scenes) | 2605.04435 | 空间锚定前向 4D，越野场景 |
| 2026-05-06 | [KFC-W](3dgs_2026-05.md#10-kfc-w-generating-3d-consistent-videos-from-unposed-internet-photos) | 2411.13549 | 自监督 3D 感知视频模型 |

### 3.2 稀疏视角 {#cat-nvs-sparse}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-21 | ★ **[TWINGS](3dgs_2026-05.md#3-twings-thin-plate-splines-warp-aligned-initialization-for-sparse-view-gaussian-splatting)** | 2605.22069 | 薄板样条形变对齐初始化 (CVPR'25) |
| 2026-05-19 | [AnyCity](3dgs_2026-05.md#4-feed-forward-gaussian-splatting-from-sparse-aerial-views) | 2605.19949 | 稀疏航拍前向 3DGS，生成式城市重建 |
| 2026-05-13 | [PanoPlane](3dgs_2026-05.md#1-panoplane-plane-aware-panoramic-completion-for-sparse-view-indoor-3d-gaussian-splatting) | 2605.14135 | 平面感知全景补全，3 视图 SOTA |
| 2026-05-12 | [PairDropGS](3dgs_2026-05.md#7-pairdropgs-paired-dropout-induced-consistency-regularization-for-sparse-view-gaussian-splatting) | 2605.12072 | 成对 Dropout 一致性正则化 |
| 2026-05-12 | ★ **[GeoQuery](3dgs_2026-05.md#8-geoquery-geometry-query-diffusion-for-sparse-view-reconstruction)** | 2605.12399 | 几何引导扩散修复伪像 (SIGGRAPH'26) |
| 2026-05-08 | [SatSurfGS](3dgs_2026-05.md#2-satsurfgs-generalizable-2d-gaussian-splatting-for-sparse-view-satellite-surface-reconstruction) | 2605.07181 | 2DGS 可泛化卫星表面重建 |
| 2026-05-04 | [LGDWT-GS](3dgs_2026-05.md#3-lgdwt-gs-local-and-global-discrete-wavelet-regularized-3d-gaussian-splatting-for-sparse-view-scene-reconstruction) | 2601.17185 | 局部+全局小波正则化稀疏视角重建 |

**概要**: 无需逐场景优化即可合成新视角（可泛化/前向方法），或从极少输入视角重建场景（稀疏视角方法）。

---

## 四、动态场景与 4D {#cat-dynamic-4d}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-22 | [RiGS](3dgs_2026-05.md#1-rigs-rigid-aware-4d-gaussian-splatting-from-a-single-monocular-video) | 2605.23672 | 三类高斯基元，跨时尺度 4D 动态场景重建 |
| 2026-05-21 | [NoPo4D](3dgs_2026-05.md#2-nopo4d-feed-forward-dynamic-gaussians-from-unposed-multi-view-videos) | 2605.22190 | 前向动态 4D Gaussian，无需位姿 |
| 2026-05-17 | [GEM](3dgs_2026-05.md#1-gem-gaussian-evolution-model-for-occupancy-forecasting-and-motion-planning) | 2605.17682 | 非自回归 4D 世界模型，占用预测 |
| 2026-05-12 | ★ **[Retrospective Dynamic NVS](3dgs_2026-05.md#3-3d-gaussian-splatting-for-efficient-retrospective-dynamic-scene-novel-view-synthesis-with-a-standardized-benchmark)** | 2605.12437 | 同步多视图回溯重建 (CVPR'26) |
| 2026-05-11 | [DySurface](3dgs_2026-05.md#4-dysurface-consistent-4d-surface-reconstruction-via-bridging-explicit-gaussians-and-implicit-functions) | 2605.10360 | 显式高斯+隐式 SDF 桥接 |
| 2026-05-06 | ★ **[RetimeGS](3dgs_2026-05.md#7-retimogs-continuous-time-reconstruction-of-4d-gaussian-splatting)** | 2603.13783 | 连续时间 4DGS 重建 (CVPR'26) |
| 2026-05-06 | ★ **[LTGS](3dgs_2026-05.md#8-ltgs-long-term-gaussian-scene-chronology-from-sparse-view-updates)** | 2510.09881 | 长期高斯场景编年史 (CVPR'26 Findings) |
| 2026-05-06 | [RoDyGS](3dgs_2026-05.md#9-rodysg-robust-dynamic-gaussian-splatting-for-casual-videos) | 2412.03077 | 鲁棒动态 3DGS，休闲视频 |
| 2026-05-04 | ★ **[Flux4D](3dgs_2026-05.md#6-flux4d-flow-based-unsupervised-4d-reconstruction)** | 2512.03210 | 无监督流式 4D 重建 (NeurIPS'25) |
| 2026-05-05 | [FreeTimeGS++](3dgs_2026-05.md#1-freetimesgs-secrets-of-dynamic-gaussian-splatting-and-their-principles) | 2605.03337 | 4DGS 关键因子分析，门控边缘化 |
| 2026-05-11 | [4D-NVS](3dgs_2026-05.md#7-4d-neural-voxel-splatting-dynamic-scene-rendering-with-voxelized-gaussian-splatting) | 2511.00560 | 4D 神经体素光栅化，形变场 |

**概要**: 处理随时间变化的动态场景，包括 4D 高斯表示、动态表面重建、时序一致性等。

---

## 五、语义分割与场景理解 {#cat-seg-understand}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-21 | [SpaceDG](3dgs_2026-05.md#1-spacedg-benchmarking-spatial-intelligence-under-visual-degradation) | 2605.22536 | 视觉降质下空间智能基准，3DGS 渲染退化合成 |
| 2026-05-19 | [OP2GS](3dgs_2026-05.md#3-op2gs-object-aware-3d-gaussian-splatting-with-dual-opacity-primitives) | 2605.20044 | 双透明度原语，对象感知分割 |
| 2026-05-15 | [Prior-Guided 3DGS Segmentation](3dgs_2026-05.md#1-robust-prior-guided-segmentation-for-editable-3d-gaussian-splatting) | 2605.16065 | SAM-HQ 先验引导，多视角一致分割 |
| 2026-05-13 | [SCOUP](3dgs_2026-05.md#6-sparse-code-uplifting-for-efficient-3d-language-gaussian-splatting) | 2605.13600 | 稀疏码本提升，训练提速 400x |
| 2026-05-12 | ★ **[PointGS](3dgs_2026-05.md#2-pointgs-semantic-consistent-unsupervised-3d-point-cloud-segmentation-with-3d-gaussian-splatting)** | 2605.11520 | 3DGS 桥接 2D-3D 语义迁移 (CVPR'26) |
| 2026-05-10 | ★ **[BEA-GS](3dgs_2026-05.md#4-bea-gs-beyond-radiance-supervision-in-3dgs-for-precise-object-extraction)** | 2605.09662 | 超越辐射监督的精确物体提取 (CVPR'26 Highlight) |
| 2026-05-07 | [OpenGaFF](3dgs_2026-05.md#2-opengaff-open-vocabulary-gaussian-feature-field-with-codebook-attention) | 2605.06088 | 码本注意力，开放词汇特征场 |
| 2026-05-06 | [Ilov3Splat](3dgs_2026-05.md#2-ilov3splat-instance-level-open-vocabulary-3d-scene-understanding-in-gaussian-splatting) | 2605.04506 | 实例级开放词汇场景理解 |
| 2026-05-03 | ★ **[GLMap](3dgs_2026-05.md#3-multi-scale-gaussian-language-map-for-zero-shot-embodied-navigation-and-reasoning)** | 2605.01736 | 多尺度高斯-语言地图 (CVPR'26) |
| 2026-05-04 | [Chorus](3dgs_2026-05.md#5-chorus-multi-teacher-pretraining-for-holistic-3d-gaussian-scene-encoding) | 2512.17817 | 多教师蒸馏 3DGS 场景编码器 |
| 2026-05-01 | ★ **[Semantic Foam](3dgs_2026-05.md#4-semantic-foam-unifying-spatial-and-semantic-scene-decomposition)** | 2604.26262 | Voronoi 网格+语义场，对象级分解 (CVPR'26 Highlight) |

**概要**: 3DGS 上的语义分割、开放词汇场景理解、语言 grounding 和物体级提取。

---

## 六、视觉定位 {#cat-visloc}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-18 | [LiteLoc](3dgs_2026-05.md#3-efficient-sparse-to-dense-visual-localization-via-compact-gaussian-scene-representation-and-accelerated-dense-pose-estimation-liteloc) | 2605.17777 | 去除颜色场减 94% 存储，PnP 蒸馏 19x |
| 2026-05-12 | [PoseCompass](3dgs_2026-05.md#5-posecompass-intelligent-synthetic-pose-selection-for-visual-localization) | 2605.12144 | 3DGS 合成位姿智能筛选 |
| 2026-05-08 | [SplitGS-Loc](3dgs_2026-05.md#4-disambiguating-2d-3d-correspondences-in-gaussian-splatting-based-feature-fields-for-visual-localization) | 2605.07351 | 高斯分裂消歧 2D-3D 对应 |
| 2026-05-06 | ★ **[ULF-Loc](3dgs_2026-05.md#5-ulf-loc-unbiased-landmark-feature-for-robust-visual-localization-with-3d-gaussian-splatting)** | 2605.04730 | 无偏地标特征 (CVPR'26 Highlight) |

**概要**: 基于 3DGS 场景表示的视觉定位，包括紧凑场景表示、特征场、2D-3D 匹配消歧等。

---

## 七、几何与表面重建 {#cat-geo-recon}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-16 | ★ **[P2GS](3dgs_2026-05.md#3-p2gs-physical-prior-guided-gaussian-splatting-for-photometrically-consistent-urban-reconstruction)** | 2605.16925 | 物理先引导光度一致重建 (CVPR'26) |
| 2026-05-13 | [HarmoGS](3dgs_2026-05.md#2-harmogs-robust-3d-gaussian-splatting-in-the-wild-via-conflict-aware-gradient-harmonization) | 2605.13073 | 冲突感知梯度调和，野生场景 |
| 2026-05-09 | [ELoG-GS](3dgs_2026-05.md#5-elog-gs-dual-branch-gaussian-splatting-with-luminance-guided-enhancement-for-extreme-low-light-3d-reconstruction) | 2604.12592 | 亮度引导双分支 3DGS，极弱光重建 |
| 2026-05-08 | [High-Fidelity Surface Splatting](3dgs_2026-05.md#6-high-fidelity-surface-splatting-based-3d-reconstruction-from-multi-view-images) | 2605.07254 | 多项式核 IMLS，高频几何保真 |
| 2026-05-08 | [AsyncEvGS](3dgs_2026-05.md#3-asyncevs-asynchronous-event-assisted-gaussian-splatting-for-handheld-motion-blurred-scenes) | 2605.07192 | 异步事件辅助，运动模糊场景 |
| 2026-05-02 | ★ **[SplAttN](3dgs_2026-05.md#1-splatttn-bridging-2d-and-3d-with-gaussian-soft-splatting-and-attention-for-point-cloud-completion)** | 2605.01466 | 高斯软光栅化，点云补全 (ICML'26 Spotlight) |
| 2026-05-01 | [2D-SuGaR](3dgs_2026-05.md#1-2d-sugar-surface-aware-gaussian-splatting-for-geometrically-accurate-mesh-reconstruction) | 2605.00569 | 单目深度法线先验增强 2DGS |

**概要**: 从图像重建几何准确的表面、网格或点云，包括表面光栅化、高频细节恢复、多传感器融合等。

---

## 八、逆渲染与光照 {#cat-invrender}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-18 | ★ **[RT-Splatting](3dgs_2026-05.md#7-rt-splatting-joint-reflection-transmission-modeling-with-gaussian-splatting)** | 2605.18263 | 反射-传输联合建模 (CVPR'26 Highlight) |
| 2026-05-09 | [Relightable GS for VP](3dgs_2026-05.md#1-relightable-gaussian-splatting-for-virtual-production-using-image-based-illumination) | 2605.09024 | 基于图像照明的重光照 |
| 2026-05-07 | [3DSS](3dgs_2026-05.md#3-3dss-3d-surface-splatting-for-inverse-rendering) | 2605.05876 | 首个表面光栅化可微逆渲染器 |
| 2026-05-01 | [GOR-IS](3dgs_2026-05.md#3-gor-is-3d-gaussian-object-removal-in-the-intrinsic-space) | 2605.00498 | 内秉空间物体移除，全局光照一致 |
| 2026-05-01 | [LCD-GS](3dgs_2026-05.md#6-high-dynamic-range-3d-gaussian-splatting-via-luminance-chromaticity-decomposition) | 2511.12895 | 亮度-色度解耦 HDR 3DGS |

**概要**: 从渲染结果反推材质、光照、形状等内秉属性，或实现物理一致的重光照。

---

## 九、生成式模型 {#cat-generative}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-18 | [PanoWorld](3dgs_2026-05.md#1-panoworld-a-generative-spatial-world-model-for-consistent-whole-house-panorama-synthesis) | 2605.17916 | 自回归全屋全景生成，3DGS 空间记忆 |
| 2026-05-18 | [GaussianZoom](3dgs_2026-05.md#8-gaussianzoom-progressive-zoom-in-generative-3d-gaussian-splatting-with-geometric-and-semantic-guidance) | 2605.18252 | 渐进式生成放大，几何+语义引导 |
| 2026-05-08 | ★ **[DeG](3dgs_2026-05.md#7-generative-3d-gaussians-with-learned-density-control)** | 2605.16355 | Octree+扩散模型，学习密度控制 (SIGGRAPH'26) |
| 2026-05-14 | [3DEditSafe](3dgs_2026-05.md#4-3d-editsafe-defending-3d-editing-pipelines-from-unsafe-generation) | 2605.15398 | 3DGS 文本驱动编辑安全防御 |
| 2026-05-01 | [VecSet-Edit](3dgs_2026-05.md#5-vecset-edit-unleashing-pre-trained-lrm-for-mesh-editing-from-single-image) | 2602.04349 | VecSet LRM 骨干单图网格编辑 |

**概要**: 使用扩散模型、自回归模型等生成式方法生成或编辑 3DGS 场景。

---

## 十、流媒体与编码 {#cat-streaming}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-20 | [Transcoding 3DGS](3dgs_2026-05.md#2-transcoding-a-3d-gaussian-splatting-model-from-a-plenoptic-point-cloud-or-mesh-without-the-original-multi-view-images) | 2605.21051 | 点云/网格到 3DGS 编解码，自定义初始化 |
| 2026-05-16 | [DSGS](3dgs_2026-05.md#2-a-single-atlas-is-all-you-need-decoder-side-gaussian-splatting-for-immersive-video) | 2605.17002 | 解码端前向 3DGS，沉浸式视频 |
| 2026-05-10 | ★ **[CAGS](3dgs_2026-05.md#2-cags-color-adaptive-volumetric-video-streaming-with-dynamic-3d-gaussian-splatting)** | 2605.09279 | 矢量量化+颜色自适应，体视频流 (SIGGRAPH'26) |
| 2026-05-09 | [TIGAS](3dgs_2026-05.md#4-thin-client-interactive-gaussian-adaptive-streaming-over-http3) | 2605.08699 | HTTP/3 轻量端自适应流式传输 |

**概要**: 3DGS 场景或动态 3DGS 的视频编码、流式传输和带宽优化。

---

## 十一、无线与射频传播 {#cat-wireless}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-18 | ★ **[GAI-GS](3dgs_2026-05.md#5-a-geometric-algebra-informed-3d-gaussian-splatting-framework-for-wireless-scene-representation)** | 2605.19065 | 几何代数引导无线场景建模 (CVPR'26) |
| 2026-05-14 | [Eff-WRFGS](3dgs_2026-05.md#1-eff-wrfgs-efficient-wireless-radiance-field-using-3d-gaussian-splatting) | 2605.15324 | 可学习掩码裁剪，存储减 44x |
| 2026-05-08 | [PropSplat](3dgs_2026-05.md#9-propsplat-map-free-rf-field-reconstruction-via-3d-gaussian-propagation-splatting) | 2605.08035 | 无地图 RF 场重建 (IEEE DySPAN'26) |
| 2026-05-12 | [XFreq-GS](3dgs_2026-05.md#1-xfreq-gs-cross-frequency-wireless-radiation-field-reconstruction-with-3d-gaussian-splatting) | 2605.11432 | 共享几何+频率自适应，跨频率泛化 |
| 2026-05-08 | [Differentiable Ray Tracing](3dgs_2026-05.md#5-differentiable-ray-tracing-with-gaussians-for-unified-radio-propagation-simulation-and-view-synthesis) | 2605.07781 | 高斯可微光线追踪，统一射频+视图 |
| 2026-05-06 | [Radio Map Tutorial](3dgs_2026-05.md#11-a-tutorial-on-learning-based-radio-map-construction-data-paradigms-and-physics-awareness) | 2603.17499 | 学习型无线电地图构建教程，3DGS 辐射场建模 |

**概要**: 将 3DGS 用于无线信道辐射场建模和射频传播仿真。

---

## 十二、安全与版权 {#cat-security}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-13 | [GuardMarkGS](3dgs_2026-05.md#3-guardmarkgs-unified-ownership-tracing-and-edit-deterrence-for-3d-gaussian-splatting) | 2605.12919 | 统一水印追踪与编辑威慑 |

**概要**: 3DGS 资产的版权保护、水印和编辑安全。

---

## 十三、自动驾驶应用 {#cat-ads}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-20 | [RCGDet3D](3dgs_2026-05.md#1-rcgdet3d-rethinking-4d-radar-camera-fusion-based-3d-object-detection-with-enhanced-radar-feature-encoding) | 2605.21112 | 高斯编码雷达特征增强，雷达-相机融合 3D 检测 |
| 2026-05-15 | [GSDrive](3dgs_2026-05.md#5-gsdrive-reinforcing-driving-policies-by-multi-mode-future-trajectory-probing-with-3d-gaussian-splatting-environment) | 2604.28111 | 3DGS 环境多模式轨迹探测+RL 强化驾驶 (v2) |
| 2026-05-08 | [LR-SGS](3dgs_2026-05.md#10-lr-sgs-robust-lidar-reflectance-guided-salient-gaussian-splatting-for-self-driving-scene-reconstruction) | 2603.12647 | 激光雷达反射率引导显著高斯 |
| 2026-05-12 | [PointForward](3dgs_2026-05.md#6-pointforward-feedforward-driving-reconstruction-through-point-aligned-representations) | 2605.11594 | 空间稀疏查询，前向驾驶重建 |
| 2026-05-02 | ★ **[SaLF](3dgs_2026-05.md#4-salf-sparse-local-fields-for-multi-sensor-rendering-in-real-time)** | 2507.18713 | 稀疏局部场多传感器实时渲染 (ICRA'26) |
| 2026-05-02 | [3DGS vs Moving Objects](3dgs_2026-05.md#5-3d-gaussian-splatting-against-moving-objects-for-high-fidelity-street-scene-reconstruction) | 2503.12001 | 自适应透明度移除运动物体，街道场景重建 |
| 2026-05-09 | [REAP](3dgs_2026-05.md#3-reap-reinforcement-learning-end-to-end-autonomous-parking-with-gaussian-splatting-simulator-for-real2sim2real-transfer) | 2605.08713 | 3DGS 模拟器，RL 端到端泊车 |
| 2026-05-03 | [3DGS for ADS Editing](3dgs_2026-05.md#1-from-concept-to-capability-evaluating-3d-gaussian-splatting-for-synthetic-scene-editing-in-autonomous-driving) | 2605.01995 | 合成场景编辑 fidelity 评估 |

**概要**: 3DGS 在自动驾驶场景重建、合成数据生成、场景编辑和仿真中的应用。

---

## 十四、机器人、SLAM 与具身智能 {#cat-robotics}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-22 | [GAF](3dgs_2026-05.md#4-gaf-gaussian-action-field-as-a-4d-representation-for-dynamic-world-modeling-in-robotic-manipulation) | 2506.14135 | 高斯动作场 4D 表示，机器人操作动态世界建模 |
| 2026-05-19 | [Conflict-Aware CBF Navigation](3dgs_2026-05.md#1-conflict-aware-active-perception-and-control-in-3d-gaussian-splatting-fields-via-control-barrier-functions) | 2605.20566 | CBF 导航，避障与数据采集统一优化 |
| 2026-05-15 | ★ **[GRaD-Nav++](3dgs_2026-05.md#6-grad-nav-vision-language-model-enabled-visual-drone-navigation-with-gaussian-radiance-fields-and-differentiable-dynamics)** | 2506.14009 | 3DGS 仿真+DiffRL 语言无人机导航 (IEEE RAL) |
| 2026-05-12 | ★ **[Compact 3DGS SLAM](3dgs_2026-05.md#9-compact-3d-gaussian-splatting-for-dense-visual-slam)** | 2403.11247 | 滑动窗口掩码+几何码本压缩 (IJCV'26) |
| 2026-05-11 | [MAGS-SLAM](3dgs_2026-05.md#5-mags-slam-monocular-multi-agent-gaussian-splatting-slam-for-geometrically-and-photometrically-consistent-reconstruction) | 2605.10760 | 仅 RGB 多智能体 3DGS SLAM |
| 2026-05-11 | [VEGA](3dgs_2026-05.md#6-vega-visual-encoder-grounding-alignment-for-spatially-aware-vision-language-action-models) | 2605.10485 | 3DGS 监督 VLA 空间感知对齐 |
| 2026-05-04 | ★ **[Digital Twin](3dgs_2026-05.md#4-a-high-fidelity-digital-twin-for-robotic-manipulation-based-on-3d-gaussian-splatting)** | 2601.03200 | 3DGS 高保真数字孪生，机器人操作 (JRL) |
| 2026-05-02 | [DMP for IL](3dgs_2026-05.md#2-a-principled-approach-for-creating-high-fidelity-synthetic-demonstrations-for-imitation-learning) | 2605.01232 | 3DGS 场景+DMP 模仿学习演示 |
| 2026-05-02 | [TAIL-Safe](3dgs_2026-05.md#3-tail-safe-task-agnostic-safety-monitoring-for-imitation-learning-policies) | 2605.01195 | 3DGS 数字孪生，安全监控 IL |

**概要**: 3DGS 在机器人 SLAM、模仿学习、具身导航和操作任务中的应用。

---

## 十五、其他应用 {#cat-other}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-19 | [FlyMirage](3dgs_2026-05.md#6-flymirage-a-fully-automated-generation-pipeline-for-diverse-and-scalable-uav-flight-data-via-generative-world-model) | 2605.19600 | 生成式世界模型，UAV 飞行数据自动生成 |
| 2026-05-15 | [FLUIDSPLAT](3dgs_2026-05.md#4-fluidsplat-reconstructing-physical-fields-from-sparse-sensors-via-gaussian-primitives) | 2605.18866 | 高斯基元物理场重建，理论近似率证明 |
| 2026-05-14 | [St. John's Co-Cathedral](3dgs_2026-05.md#6-st-johns-co-cathedral-large-scale-photogrammetric-documentation-of-st-johns-co-cathedral-a-workflow-for-cultural-heritage-preservation) | 2604.24316 | 文化遗产摄影测量，300亿三角面 |
| 2026-05-13 | [G-SHARP](3dgs_2026-05.md#7-g-sharp-gaussian-surgical-hardware-accelerated-real-time-pipeline) | 2512.02482 | 商用许可实时手术 3DGS (IGX Orin/Thor) |
| 2026-05-13 | ★ **[3D-UIR](3dgs_2026-05.md#9-3d-uir-3d-gaussian-for-underwater-3d-scene-reconstruction-via-physics-based-appearance-medium-decoupling)** | 2505.21238 | 物理外观-介质解耦，水下重建 (IEEE TIP'26) |
| 2026-05-17 | [GEM](3dgs_2026-05.md#1-gem-gaussian-evolution-model-for-occupancy-forecasting-and-motion-planning) * | 2605.17682 | 4D 世界模型，占用预测+规划 |
| 2026-05-16 | [Topo-GS](3dgs_2026-05.md#1-topo-gs-continuous-volumetric-embedding-of-high-dimensional-data-via-topological-gaussian-splatting) | 2605.17011 | 3DGS 复用于降维可视化 |
| 2026-05-11 | [SDTalk](3dgs_2026-05.md#3-sdtalk-structured-facial-priors-and-dual-branch-motion-fields-for-generalizable-gaussian-talking-head-synthesis) | 2605.09956 | 单帧可泛化说话人头合成 |
| 2026-05-10 | [LagrangianSplats](3dgs_2026-05.md#3-lagrangiansplats-divergence-free-transport-of-gaussian-primitives-for-fluid-reconstruction) | 2605.09299 | 无散度核，流体场重建 |
| 2026-05-10 | [FrameTwin](3dgs_2026-05.md#5-frametwin-curve-anchored-gaussian-alignment-from-sparse-views-for-adaptive-wireframe-3d-printing) | 2605.09362 | 曲线锚定高斯，自适应线框 3D 打印 |
| 2026-05-08 | [GD-DIFF](3dgs_2026-05.md#1-from-pixels-to-primitives-scene-change-detection-in-3d-gaussian-splatting) | 2605.07203 | 基元属性级场景变化检测 |
| 2026-05-06 | [CoherentRaster](3dgs_2026-05.md#1-coherentraster-efficient-3d-gaussian-splatting-for-light-field-displays) | 2605.04509 | 子像素光栅化，光场显示 |
| 2026-05-06 | [Aes3D](3dgs_2026-05.md#4-aes3d-aesthetic-assessment-in-3d-gaussian-splatting) | 2605.05155 | 3DGS 场景美学评估框架 |
| 2026-05-04 | [HumanSplatHMR](3dgs_2026-05.md#1-humansplathmr-closing-the-loop-between-human-mesh-recovery-and-gaussian-splatting-avatar) | 2605.02784 | 姿态估计+数字人渲染闭环 |
| 2026-05-04 | ★ **[VRGaussianAvatar](3dgs_2026-05.md#2-vrgaussianavatar-integrating-3d-gaussian-avatars-into-vr)** | 2602.01674 | HMD 驱动的实时 3DGS VR 数字人 (IEEE VR'26) |
| 2026-05-04 | [AR Disaster Response](3dgs_2026-05.md#7-interactive-augmented-reality-enabled-outdoor-scene-visualization-for-enhanced-real-time-disaster-response) | 2602.21874 | 3DGS 户外 AR 灾难响应可视化 |
| 2026-05-03 | [DynFOA](3dgs_2026-05.md#4-dynfoa-generating-first-order-ambisonics-with-conditional-diffusion-for-dynamic-and-acoustically-complex-360-degree-videos) | 2602.06846 | 3DGS 场景重建+扩散模型生成空间音频 |
| 2026-05-02 | [GSDeformer](3dgs_2026-05.md#6-gsdeformer-direct-real-time-and-extensible-cage-based-deformation-for-3d-gaussian-splatting) | 2405.15491 | 3DGS 笼形形变，实时可扩展 |

* GEM 同时在"动态场景与 4D"中列出。

**概要**: 3DGS 在其他领域的应用扩展，包括数字人、流体模拟、3D 打印、变化检测、光场显示、美学评估和数据可视化等。

---

## 统计概览

| 类别 | 论文数 |
|------|--------|
| 新视角合成 | 20 |
| 其他应用 | 18 |
| 核心算法与优化 | 12 |
| 动态场景与 4D | 11 |
| 语义分割与场景理解 | 11 |
| 渲染加速与压缩 | 9 |
| 机器人、SLAM 与具身智能 | 9 |
| 几何与表面重建 | 7 |
| 自动驾驶应用 | 8 |
| 无线与射频传播 | 6 |
| 视觉定位 | 4 |
| 逆渲染与光照 | 5 |
| 生成式模型 | 5 |
| 流媒体与编码 | 4 |
| 安全与版权 | 1 |
| **合计（含重复）** | **130** |

> 注：GEM 同时归属"动态场景与 4D"和"其他应用"；Turbo-GS 同时归属"渲染加速与压缩"和"新视角合成"，故合计为 130 而非 128。原始论文总数为 129 篇（5 月 1 日至 5 月 22 日）。
