# 3D Gaussian Splatting 论文跟踪 分类索引 (2026年1月)

> 基于 `3dgs_2026-01.md` 中收集的论文，按研究方向细分类。
> ★ 表示被顶会/顶刊录用。

## 目录

- [3D Gaussian Splatting 论文跟踪 分类索引 (2026年1月)](#3D Gaussian Splatting 论文跟踪-分类索引-2026年1月)
  - [目录](#目录)
  - [一、几何与表面重建](#cat-geo-recon)
  - [二、视觉定位](#cat-visloc)
  - [三、核心算法与优化](#cat-core-opt)
  - [四、安全与版权](#cat-security)
  - [五、无线与射频传播](#cat-rf)
  - [六、风格迁移与编辑](#cat-style-edit)
  - [七、语义分割与场景理解](#cat-seg-understand)
  - [八、领域应用](#cat-domain-app)
  - [九、生成式模型](#cat-generative)
  - [十、新视角合成](#cat-nvs)
  - [十一、机器人仿真与具身智能](#cat-robotics)
  - [十二、自动驾驶应用](#cat-autodrive)
  - [十三、数字人与人体重建](#cat-human)
  - [十四、动态场景与4D](#cat-dynamic-4d)
  - [十五、渲染加速与压缩](#cat-render-accel)
  - [十六、流媒体与编码](#cat-streaming)
  - [十七、SLAM与建图](#cat-slam)
  - [十八、逆渲染与光照](#cat-inverserender)
  - [十九、凝聚态物理理论](#cat-condensed-matter)
  - [统计概览](#统计概览)

---

## 一、几何与表面重建 {#cat-geo-recon}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-31 | [GaussLeJEPA](./3dgs_2026-01.md#1-gaussian-constrained-lejepa-representations-for-unsupervised-scene-discovery-and-pose-consistency) | 2602.07016 | 高斯约束,自监督表示,场景发现,位姿估计,运动恢复结构 |
| 2026-01-31 | [GaussianEM](./3dgs_2026-01.md#5-resolving-compositional-and-conformational-heterogeneity-in-cryo-em-with-deformable-3d-gaussian-representations) | 2512.21599 | 3D高斯表示,冷冻电镜,构象异质性,伪原子框架,结构重建 |
| 2026-01-30 | [3DGS2-TR](./3dgs_2026-01.md#2-3dgs-2-tr-scalable-second-order-trust-region-method-for-3d-gaussian-splatting) | 2602.00395 | 二阶优化,信任域,3D高斯溅射,Hessian近似 |
| 2026-01-30 | [GeoRep](./3dgs_2026-01.md#3-learning-geometrically-grounded-3d-visual-representations-for-view-generalizable-robotic-manipulation) | 2601.22988 | 单视角3D预训练,高斯溅射,多步蒸馏,视角泛化 |
| 2026-01-30 | [Diachronic](./3dgs_2026-01.md#4-diachronic-stereo-matching-for-multi-date-satellite-imagery) | 2601.22808 | 历时立体匹配,跨期卫星影像,单目深度先验,三维重建 |
| 2026-01-30 | [RoboArmGS](./3dgs_2026-01.md#7-roboarmgs-high-quality-robotic-arm-splatting-via-b-zier-curve-refinement) | 2511.17961 | 3D高斯溅射,贝塞尔曲线优化,机械臂运动建模,数字资产重建 |
| 2026-01-30 | ★ **[Learning](./3dgs_2026-01.md#8-learning-unified-representation-of-3d-gaussian-splatting)** | 2509.22917 | 3D高斯溅射,嵌入表示,连续子流形场,参数同质化,特征学习 ICLR'26 |
| 2026-01-30 | [Pose Splatter](./3dgs_2026-01.md#9-pose-splatter-a-3d-gaussian-splatting-model-for-quantifying-animal-pose-and-appearance) | 2505.18342 | 3D高斯溅射,形状雕刻,动物姿态估计,无标注建模,视觉嵌入 |
| 2026-01-29 | [SynRealShip](./3dgs_2026-01.md#1-synthetic-to-real-domain-bridging-for-single-view-3d-reconstruction-of-ships-for-maritime-monitoring) | 2601.21786 | 单视角重建,3D高斯,域适应,船舶监控,合成数据训练 |
| 2026-01-28 | ★ **[Fast3DGS](./3dgs_2026-01.md#4-fast-converging-3d-gaussian-splatting-for-1-minute-reconstruction)** | 2601.19489 | 3D高斯泼溅,快速重建,神经高斯表示,并行优化,深度监督 SIGGRAPH Asia'25 |
| 2026-01-28 | [WaveletGaussian](./3dgs_2026-01.md#6-waveletgaussian-wavelet-domain-diffusion-for-sparse-view-3d-gaussian-object-reconstruction) | 2509.19073 | 小波域扩散,稀疏视角重建,3D高斯溅射,训练加速 |
| 2026-01-28 | [Dense-SfM](./3dgs_2026-01.md#7-dense-sfm-structure-from-motion-with-dense-consistent-matching) | 2501.14277 | 运动恢复结构,稠密匹配,高斯泼溅,轨迹扩展,多视图核匹配 |
| 2026-01-27 | [WaterClear-GS](./3dgs_2026-01.md#1-waterclear-gs-optical-aware-gaussian-splatting-for-underwater-reconstruction-and-restoration) | 2601.19753 | 3D高斯泼溅,水下三维重建,光学特性建模,新视角合成,图像恢复 |
| 2026-01-27 | [UniMGS](./3dgs_2026-01.md#5-unimgs-unifying-mesh-and-3d-gaussian-splatting-with-single-pass-rasterization-and-proxy-based-deformation) | 2601.19233 | 3D高斯溅射,网格渲染,单次光栅化,代理形变,抗锯齿混合 |
| 2026-01-26 | [ExoGS](./3dgs_2026-01.md#3-exogs-a-4d-real-to-sim-to-real-framework-for-scalable-manipulation-data-collection) | 2601.18629 | 真仿真迁移,3D高斯重建,被动外骨骼,操作数据收集,策略泛化 |
| 2026-01-25 | [Revisiting](./3dgs_2026-01.md#1-revisiting-3d-reconstruction-kernels-as-low-pass-filters) | 2601.17900 | 3D重建,Jinc核,调制核,低通滤波,信号处理 |
| 2026-01-25 | [SparseVoxel](./3dgs_2026-01.md#2-advancing-structured-priors-for-sparse-voxel-surface-reconstruction) | 2601.17720 | 稀疏体素,3D高斯溅射,表面重建,深度监督,几何先验 |
| 2026-01-25 | [SceneSplat++](./3dgs_2026-01.md#4-scenesplat-a-large-dataset-and-comprehensive-benchmark-for-language-gaussian-splatting) | 2506.08710 | 3D高斯溅射,语言场景理解,泛化范式,语义分割,大规模基准 |
| 2026-01-24 | [Mirage2Matter](./3dgs_2026-01.md#1-mirage2matter-a-physically-grounded-gaussian-world-model-from-video) | 2602.00096 | 3D高斯溅射,世界模型,物理仿真,具身智能 |
| 2026-01-22 | [GS-DT](./3dgs_2026-01.md#1-three-dimensional-damage-visualization-of-civil-structures-via-gaussian-splatting-enabled-digital-twins) | 2602.16713 | 高斯溅射,数字孪生,三维重建,损伤可视化,多尺度策略 |
| 2026-01-22 | [NoMesh](./3dgs_2026-01.md#4-no-mesh-no-problem-estimating-coral-volume-and-surface-from-sparse-multi-view-images) | 2509.11164 | 稀疏多视角,点云融合,体积表面积估算,不确定性估计,珊瑚几何重建 |
| 2026-01-21 | [CAG-Avatar](./3dgs_2026-01.md#3-cag-avatar-cross-attention-guided-gaussian-avatars-for-high-fidelity-head-reconstruction) | 2601.14844 | 3D高斯泼溅,交叉注意力,数字人驱动,头部重建,自适应融合 |
| 2026-01-21 | [POTR](./3dgs_2026-01.md#4-potr-post-training-3dgs-compression) | 2601.14821 | 3DGS压缩,并行剪枝,光照系数重算,率失真优化 |
| 2026-01-21 | [ConeGS](./3dgs_2026-01.md#5-conegs-error-guided-densification-using-pixel-cones-for-improved-reconstruction-with-fewer-primitives) | 2511.06810 | 3D高斯溅射,视锥引导,误差引导优化,基元预算,新视角合成 |
| 2026-01-20 | [RigAware](./3dgs_2026-01.md#2-rig-aware-3d-reconstruction-of-vehicle-undercarriages-using-gaussian-splatting) | 2601.14208 | 高斯泼溅,支架感知SfM,三维重建,实时渲染,车辆检测 |
| 2026-01-20 | [OneShotRefiner](./3dgs_2026-01.md#3-one-shot-refiner-boosting-feed-forward-novel-view-synthesis-via-one-step-diffusion) | 2601.14161 | 新视角合成, 3D高斯溅射, 扩散模型, 双域感知, 联合优化 |
| 2026-01-20 | [ParkingTwin](./3dgs_2026-01.md#4-parkingtwin-training-free-streaming-3d-reconstruction-for-parking-lot-digital-twins) | 2601.13706 | 流式三维重建,OSM先验建图,动态遮挡过滤,光照鲁棒融合 |
| 2026-01-19 | [BladeSDF](./3dgs_2026-01.md#1-bladesdf-unconditional-and-conditional-generative-modeling-of-representative-blade-geometries-using-signed-distance-functions) | 2601.13445 | 符号距离函数,隐式生成模型,涡轮叶片设计,潜空间建模,性能条件生成 |
| 2026-01-19 | [KaoLRM](./3dgs_2026-01.md#6-kaolrm-repurposing-pre-trained-large-reconstruction-models-for-parametric-3d-face-reconstruction) | 2601.12736 | 大型重建模型,2D高斯溅射,参数化人脸重建,FLAME模型 |
| 2026-01-19 | [OceanSplat](./3dgs_2026-01.md#7-oceansplat-object-aware-gaussian-splatting-with-trinocular-view-consistency-for-underwater-scene-reconstruction) | 2601.04984 | 3D高斯泼溅,三眼视图一致性,深度正则化,水下重建 |
| 2026-01-18 | [TIDI-GS](./3dgs_2026-01.md#2-tidi-gs-floater-suppression-in-3d-gaussian-splatting-for-enhanced-indoor-scene-fidelity) | 2601.09291 | 3D高斯泼溅,悬浮点抑制,多视角一致性,几何优化,轻量级插件 |
| 2026-01-18 | [ProFuse](./3dgs_2026-01.md#3-profuse-efficient-cross-view-context-fusion-for-open-vocabulary-3d-gaussian-splatting) | 2601.04754 | 3D高斯泼溅,开放词汇理解,跨视图融合,语义配准 |
| 2026-01-18 | [SA-ResGS](./3dgs_2026-01.md#4-sa-resgs-self-augmented-residual-3d-gaussian-splatting-for-next-best-view-selection) | 2601.03024 | 3D高斯泼溅,残差学习,不确定性量化,视点选择,主动重建 |
| 2026-01-17 | [ActiveMapping](./3dgs_2026-01.md#1-active-semantic-mapping-of-horticultural-environments-using-gaussian-splatting) | 2601.12122 | 3D高斯泼溅,主动语义建图,移动机器人,Octomap,农业场景 |
| 2026-01-17 | ★ **[VRP-UDF](./3dgs_2026-01.md#2-vrp-udf-towards-unbiased-learning-of-unsigned-distance-functions-from-multi-view-images-with-volume-rendering-priors)** | 2407.16396 | 无符号距离函数,体渲染先验,可微渲染,零水平集采样,表面重建 ECCV'24 |
| 2026-01-16 | [studentSplat](./3dgs_2026-01.md#2-studentsplat-your-student-model-learns-single-view-3d-gaussian-splatting) | 2601.11772 | 单视图重建, 3D高斯泼溅, 师生架构, 外推网络, 尺度模糊 |
| 2026-01-15 | [CurvatureFit](./3dgs_2026-01.md#3-curvature-driven-manifold-fitting-under-unbounded-isotropic-noise) | 2601.10133 | 流形拟合,曲率驱动,核估计器,二阶精度,高斯噪声 |
| 2026-01-14 | [JOGS](./3dgs_2026-01.md#4-jogs-joint-optimization-of-pose-estimation-and-3d-gaussian-splatting) | 2510.26117 | 3D高斯溅射,相机位姿估计,联合优化,可微渲染,3D光流 |
| 2026-01-13 | [LearningMVS](./3dgs_2026-01.md#3-learning-based-multi-view-stereo-a-survey) | 2408.15235 | 多视图立体视觉,深度学习,三维重建,深度图估计,算法综述 |
| 2026-01-12 | [R3-RECON](./3dgs_2026-01.md#4-r3-recon-radiance-field-free-active-reconstruction-via-renderability) | 2601.07484 | 主动重建, 视点规划, 可渲染性场, 体素地图, 新视角合成 |
| 2026-01-12 | [Sketch&Patch++](./3dgs_2026-01.md#5-sketch-amp-patch-efficient-structure-aware-3d-gaussian-representation) | 2601.05394 | 3D高斯表示,分层渐进传输,密度聚类,结构感知编码 |
| 2026-01-12 | [GP-GS](./3dgs_2026-01.md#7-gp-gs-gaussian-processes-densification-for-3d-gaussian-splatting) | 2502.02283 | 3D高斯泼溅,高斯过程,点云稠密化,不确定性过滤 |
| 2026-01-11 | [SARA](./3dgs_2026-01.md#1-sara-scene-aware-reconstruction-accelerator) | 2601.06831 | 运动恢复结构,图像对选择,几何驱动,信息加权生成树,重建加速 |
| 2026-01-10 | [3DSceneRep](./3dgs_2026-01.md#1-what-is-the-best-3d-scene-representation-for-robotics-from-geometric-to-foundation-models) | 2512.03422 | 三维场景表示,机器人系统,神经表示,3D高斯泼溅,基础模型 |
| 2026-01-09 | [PointSLAM++](./3dgs_2026-01.md#1-pointslam-robust-dense-neural-gaussian-point-cloud-based-slam) | 2601.11617 | 神经高斯表示,渐进式位姿优化,动态节点分布,RGB-D SLAM,3D重建 |
| 2026-01-09 | [NAS-GS](./3dgs_2026-01.md#3-nas-gs-noise-aware-sonar-gaussian-splatting) | 2601.06285 | 声呐高斯溅射,双向渲染,高斯混合噪声模型,新视角合成,三维重建 |
| 2026-01-09 | [LayerGS](./3dgs_2026-01.md#5-layergs-decomposition-and-inpainting-of-layered-3d-human-avatars-via-2d-gaussian-splatting) | 2601.05853 | 2D高斯溅射,扩散模型修复,人体分层重建,虚拟试穿 |
| 2026-01-08 | [MOSAIC-GS](./3dgs_2026-01.md#4-mosaic-gs-monocular-scene-reconstruction-via-advanced-initialization-for-complex-dynamic-environments) | 2601.05368 | 高斯溅射,单目动态重建,几何初始化,傅里叶轨迹 |
| 2026-01-08 | [Defocus](./3dgs_2026-01.md#5-defocus-aberration-theory-confirms-gaussian-model-in-most-imaging-devices) | 2601.04779 | 散焦深度估计,高斯模糊模型,像差理论,几何光学,三维重建 |
| 2026-01-08 | [InnerGS](./3dgs_2026-01.md#6-innergs-internal-scenes-reconstruction-and-segmentation-via-factorized-3d-gaussian-splatting) | 2508.13287 | 3D高斯泼溅,内部场景重建,文本引导分割,连续体密度建模 |
| 2026-01-06 | [HighOrderPCA](./3dgs_2026-01.md#2-higher-order-pca-like-rotation-invariant-features-for-detailed-shape-descriptors-modulo-rotation) | 2601.03326 | 高阶张量,旋转不变特征,形状描述符,中心矩 |
| 2026-01-05 | [360-GeoGS](./3dgs_2026-01.md#2-360-geogs-geometrically-consistent-feed-forward-3d-gaussian-splatting-reconstruction-for-360-images) | 2601.02102 | 3D高斯泼溅,前馈重建,几何一致性,深度法向正则化 |
| 2026-01-05 | [InpaintHuman](./3dgs_2026-01.md#3-inpainthuman-reconstructing-occluded-humans-with-multi-scale-uv-mapping-and-identity-preserving-diffusion-inpainting) | 2601.02098 | 人体重建,扩散修复,UV映射,身份保持,遮挡处理 |
| 2026-01-05 | [PMGS](./3dgs_2026-01.md#5-pmgs-reconstruction-of-projectile-motion-across-large-spatiotemporal-spans-via-3d-gaussian-splatting) | 2508.02660 | 3D高斯泼溅,抛体运动重建,物理一致性约束,卡尔曼滤波 |
| 2026-01-04 | [ParkGaussian](./3dgs_2026-01.md#3-parkgaussian-surround-view-3d-gaussian-splatting-for-autonomous-parking) | 2601.01386 | 3D高斯溅射,泊车场景重建,车位感知引导,环视相机 |
| 2026-01-04 | [ShadowGS](./3dgs_2026-01.md#4-shadowgs-shadow-aware-3d-gaussian-splatting-for-satellite-imagery) | 2601.00939 | 3D高斯泼溅,阴影建模,卫星影像重建,物理渲染,新视角合成 |
| 2026-01-04 | [MeSS](./3dgs_2026-01.md#6-mess-city-mesh-guided-outdoor-scene-generation-with-cross-view-consistent-diffusion) | 2508.15169 | 城市网格引导,跨视角扩散模型,3D高斯溅射,场景生成,几何对齐 |
| 2026-01-02 | [AdaGaR](./3dgs_2026-01.md#1-adagar-adaptive-gabor-representation-for-dynamic-scene-reconstruction) | 2601.00796 | 自适应Gabor表示,动态场景重建,时域连续性,三维基元优化,帧插值 |
| 2026-01-01 | [Stereo-GS](./3dgs_2026-01.md#3-stereo-gs-multi-view-stereo-vision-model-for-generalizable-3d-gaussian-splatting-reconstruction) | 2507.14921 | 3D高斯泼溅,立体视觉,几何外观解耦,免位姿重建 |

**概要**: 本类论文涉及帧插值、阴影建模、连续子流形场、参数同质化、深度正则化、伪原子框架、物理渲染、并行优化等研究方向，共 59 篇。

---

## 二、视觉定位 {#cat-visloc}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-31 | [GaussLeJEPA](./3dgs_2026-01.md#1-gaussian-constrained-lejepa-representations-for-unsupervised-scene-discovery-and-pose-consistency) | 2602.07016 | 高斯约束,自监督表示,场景发现,位姿估计,运动恢复结构 |

**概要**: 本类论文涉及高斯约束、运动恢复结构、自监督表示、场景发现、位姿估计等研究方向，共 1 篇。

---

## 三、核心算法与优化 {#cat-core-opt}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-31 | [GaussLeJEPA](./3dgs_2026-01.md#1-gaussian-constrained-lejepa-representations-for-unsupervised-scene-discovery-and-pose-consistency) | 2602.07016 | 高斯约束,自监督表示,场景发现,位姿估计,运动恢复结构 |
| 2026-01-31 | [NPNet](./3dgs_2026-01.md#4-npnet-a-non-parametric-network-with-adaptive-gaussian-fourier-positional-encoding-for-3d-classification-and-segmentation) | 2602.00542 | 无参网络,自适应高斯傅里叶编码,3D点云分割,少样本学习 |
| 2026-01-31 | [EKS](./3dgs_2026-01.md#6-affine-equivariant-kernel-space-encoding-for-nerf-editing) | 2508.02831 | 神经辐射场,高斯核编码,特征蒸馏,局部编辑 |
| 2026-01-30 | [3DGS2-TR](./3dgs_2026-01.md#2-3dgs-2-tr-scalable-second-order-trust-region-method-for-3d-gaussian-splatting) | 2602.00395 | 二阶优化,信任域,3D高斯溅射,Hessian近似 |
| 2026-01-30 | ★ **[Learning](./3dgs_2026-01.md#8-learning-unified-representation-of-3d-gaussian-splatting)** | 2509.22917 | 3D高斯溅射,嵌入表示,连续子流形场,参数同质化,特征学习 ICLR'26 |
| 2026-01-30 | [CacheFlow](./3dgs_2026-01.md#10-cacheflow-fast-human-motion-prediction-by-cached-normalizing-flow) | 2505.13140 | 正常化流, 人体运动预测, 缓存机制, 密度估计, 生成模型 |
| 2026-01-29 | [GMC](./3dgs_2026-01.md#2-from-global-to-granular-revealing-iqa-model-performance-via-correlation-surface) | 2601.21738 | 图像质量评估,粒度调制相关性,相关性曲面,细粒度分析,分布调节 |
| 2026-01-29 | [ReLNs](./3dgs_2026-01.md#5-equivariant-neural-networks-for-general-linear-symmetries-on-lie-algebras) | 2510.22984 | 等变神经网络,李代数,广义线性对称性,矩阵特征,伴随不变形式 |
| 2026-01-28 | [LangGS-SLAM](./3dgs_2026-01.md#1-langgs-slam-real-time-language-feature-gaussian-splatting-slam) | 2602.06991 | 高斯溅射,SLAM,语言对齐特征,Top-K渲染,混合场优化 |
| 2026-01-28 | [FreeFix](./3dgs_2026-01.md#2-freefix-boosting-3d-gaussian-splatting-via-fine-tuning-free-diffusion-models) | 2601.20857 | 3D高斯泼溅,扩散模型,免微调优化,2D-3D交替细化,置信度掩码 |
| 2026-01-28 | [GRTX](./3dgs_2026-01.md#3-grtx-efficient-ray-tracing-for-3d-gaussian-based-rendering) | 2601.20429 | 3D高斯渲染,射线追踪,加速结构优化,硬件协同设计 |
| 2026-01-28 | ★ **[Fast3DGS](./3dgs_2026-01.md#4-fast-converging-3d-gaussian-splatting-for-1-minute-reconstruction)** | 2601.19489 | 3D高斯泼溅,快速重建,神经高斯表示,并行优化,深度监督 SIGGRAPH Asia'25 |
| 2026-01-28 | [WaveletGaussian](./3dgs_2026-01.md#6-waveletgaussian-wavelet-domain-diffusion-for-sparse-view-3d-gaussian-object-reconstruction) | 2509.19073 | 小波域扩散,稀疏视角重建,3D高斯溅射,训练加速 |
| 2026-01-27 | [TIGaussian](./3dgs_2026-01.md#4-tigaussian-disentangle-gaussians-for-spatial-awared-text-image-3d-alignment) | 2601.19247 | 3D高斯溅射,跨模态对齐,多分支分词器,扩散先验,空间感知 |
| 2026-01-27 | [UniMGS](./3dgs_2026-01.md#5-unimgs-unifying-mesh-and-3d-gaussian-splatting-with-single-pass-rasterization-and-proxy-based-deformation) | 2601.19233 | 3D高斯溅射,网格渲染,单次光栅化,代理形变,抗锯齿混合 |
| 2026-01-27 | [GDAGS](./3dgs_2026-01.md#6-gradient-direction-aware-density-control-for-3d-gaussian-splatting) | 2508.09239 | 3D高斯泼溅,密度控制,梯度方向感知,新视角合成 |
| 2026-01-25 | [Revisiting](./3dgs_2026-01.md#1-revisiting-3d-reconstruction-kernels-as-low-pass-filters) | 2601.17900 | 3D重建,Jinc核,调制核,低通滤波,信号处理 |
| 2026-01-25 | [SparseVoxel](./3dgs_2026-01.md#2-advancing-structured-priors-for-sparse-voxel-surface-reconstruction) | 2601.17720 | 稀疏体素,3D高斯溅射,表面重建,深度监督,几何先验 |
| 2026-01-25 | [CrossLevel](./3dgs_2026-01.md#3-cross-level-sensor-fusion-with-object-lists-via-transformer-for-3d-object-detection) | 2512.12884 | 跨层级融合,Transformer,3D目标检测,传感器融合,可变形掩码 |
| 2026-01-25 | [Matrix-free](./3dgs_2026-01.md#5-matrix-free-second-order-optimization-of-gaussian-splats-with-residual-sampling) | 2504.12905 | 3D高斯泼溅,二阶优化,免矩阵算法,残差采样,训练加速 |
| 2026-01-22 | [CamPilot](./3dgs_2026-01.md#2-campilot-improving-camera-control-in-video-diffusion-model-with-efficient-camera-reward-feedback) | 2601.16214 | 视频扩散模型,相机控制,3D高斯解码,奖励反馈学习 |
| 2026-01-21 | [ConeGS](./3dgs_2026-01.md#5-conegs-error-guided-densification-using-pixel-cones-for-improved-reconstruction-with-fewer-primitives) | 2511.06810 | 3D高斯溅射,视锥引导,误差引导优化,基元预算,新视角合成 |
| 2026-01-20 | [Gaussian](./3dgs_2026-01.md#1-gaussian-based-adaptive-multi-modal-3d-semantic-occupancy-prediction) | 2601.14448 | 3D高斯模型,多模态融合,语义占据预测,状态空间模型,自适应校准 |
| 2026-01-20 | ★ **[RI3D](./3dgs_2026-01.md#5-ri3d-few-shot-gaussian-splatting-with-repair-and-inpainting-diffusion-priors)** | 2503.10860 | 3D高斯泼溅,扩散模型,新视角合成,两阶段优化,深度初始化 ICCV'25 |
| 2026-01-18 | [GaussianTrimmer](./3dgs_2026-01.md#1-gaussiantrimmer-online-trimming-boundaries-for-3dgs-segmentation) | 2601.12683 | 3D高斯分割,边界修剪,虚拟相机,即插即用后处理 |
| 2026-01-18 | [TIDI-GS](./3dgs_2026-01.md#2-tidi-gs-floater-suppression-in-3d-gaussian-splatting-for-enhanced-indoor-scene-fidelity) | 2601.09291 | 3D高斯泼溅,悬浮点抑制,多视角一致性,几何优化,轻量级插件 |
| 2026-01-17 | ★ **[VRP-UDF](./3dgs_2026-01.md#2-vrp-udf-towards-unbiased-learning-of-unsigned-distance-functions-from-multi-view-images-with-volume-rendering-priors)** | 2407.16396 | 无符号距离函数,体渲染先验,可微渲染,零水平集采样,表面重建 ECCV'24 |
| 2026-01-15 | [CurvatureFit](./3dgs_2026-01.md#3-curvature-driven-manifold-fitting-under-unbounded-isotropic-noise) | 2601.10133 | 流形拟合,曲率驱动,核估计器,二阶精度,高斯噪声 |
| 2026-01-14 | [VBM](./3dgs_2026-01.md#1-variable-basis-mapping-for-real-time-volumetric-visualization) | 2601.09417 | 3D高斯溅射,小波分析,闭式映射,体数据可视化,实时渲染 |
| 2026-01-14 | [GaussianFluent](./3dgs_2026-01.md#2-gaussianfluent-gaussian-simulation-for-dynamic-scenes-with-mixed-materials) | 2601.09265 | 3D高斯泼溅,物理模拟,脆性断裂,物质点法,动态场景 |
| 2026-01-14 | [A^2TG](./3dgs_2026-01.md#3-a-2-tg-adaptive-anisotropic-textured-gaussians-for-efficient-3d-scene-representation) | 2601.09243 | 高斯溅射,各向异性纹理,自适应分配,内存优化 |
| 2026-01-13 | [PINGS-X](./3dgs_2026-01.md#1-pings-x-physics-informed-normalized-gaussian-splatting-with-axes-alignment-for-efficient-super-resolution-of-4d-flow-mri) | 2511.11048 | 高斯溅射,4D血流MRI,超分辨率,轴对齐表示,物理约束 |
| 2026-01-12 | [SOGDD](./3dgs_2026-01.md#1-second-order-gaussian-directional-derivative-representations-for-image-high-resolution-corner-detection) | 2601.08182 | 角点检测,二阶高斯方向导数,高分辨率,图像匹配,三维重建 |
| 2026-01-12 | [GP-GS](./3dgs_2026-01.md#7-gp-gs-gaussian-processes-densification-for-3d-gaussian-splatting) | 2502.02283 | 3D高斯泼溅,高斯过程,点云稠密化,不确定性过滤 |
| 2026-01-12 | [CLIP-GS](./3dgs_2026-01.md#8-clip-gs-unifying-vision-language-representation-with-3d-gaussian-splatting) | 2412.19142 | 3D高斯溅射,多模态表示学习,对比学习,图像投票损失 |
| 2026-01-11 | [SARA](./3dgs_2026-01.md#1-sara-scene-aware-reconstruction-accelerator) | 2601.06831 | 运动恢复结构,图像对选择,几何驱动,信息加权生成树,重建加速 |
| 2026-01-09 | [MultiTask](./3dgs_2026-01.md#4-multi-task-modeling-for-engineering-applications-with-sparse-data) | 2601.05910 | 多任务高斯过程,多保真数据,稀疏数据建模,任务关联,工程预测 |
| 2026-01-09 | [GS-DMSR](./3dgs_2026-01.md#6-gs-dmsr-dynamic-sensitive-multi-scale-manifold-enhancement-for-accelerated-high-quality-3d-gaussian-splatting) | 2601.05584 | 3D高斯溅射,动态场景重建,自适应梯度,流形增强,渲染加速 |
| 2026-01-09 | [FreqGS](./3dgs_2026-01.md#7-frequency-aware-gaussian-splatting-decomposition) | 2503.21226 | 3D高斯溅射,频率感知分解,拉普拉斯金字塔,细节层次渲染 |
| 2026-01-08 | [Akasha 2](./3dgs_2026-01.md#1-akasha-2-hamiltonian-state-space-duality-and-visual-language-joint-embedding-predictive-architectur) | 2601.06212 | 哈密顿状态空间,视语联合预测,物理守恒,3D高斯溅射,流匹配 |
| 2026-01-08 | [Defocus](./3dgs_2026-01.md#5-defocus-aberration-theory-confirms-gaussian-model-in-most-imaging-devices) | 2601.04779 | 散焦深度估计,高斯模糊模型,像差理论,几何光学,三维重建 |
| 2026-01-06 | [HighOrderPCA](./3dgs_2026-01.md#2-higher-order-pca-like-rotation-invariant-features-for-detailed-shape-descriptors-modulo-rotation) | 2601.03326 | 高阶张量,旋转不变特征,形状描述符,中心矩 |
| 2026-01-06 | [SAGOnline](./3dgs_2026-01.md#4-sagonline-segment-any-gaussians-online) | 2508.08219 | 3D高斯溅射,零样本分割,几何共识,实时推理,视频基础模型 |
| 2026-01-05 | ★ **[Joint3DGS](./3dgs_2026-01.md#1-joint-semantic-and-rendering-enhancements-in-3d-gaussian-modeling-with-anisotropic-local-encoding)** | 2601.02339 | 3D高斯溅射,语义分割,各向异性编码,跨场景迁移,联合优化 ICCV'25 |
| 2026-01-03 | [AH-GS](./3dgs_2026-01.md#1-ah-gs-augmented-3d-gaussian-splatting-for-high-frequency-detail-representation) | 2503.22324 | 3D高斯溅射,高频细节表示,特征编码,渲染优化,损失函数 |
| 2026-01-01 | [Clean-GS](./3dgs_2026-01.md#1-clean-gs-semantic-mask-guided-pruning-for-3d-gaussian-splatting) | 2601.00913 | 3D高斯溅射,语义掩码,模型剪枝,伪影去除,模型压缩 |

**概要**: 本类论文涉及局部编辑、语义占据预测、残差采样、连续子流形场、参数同质化、少样本学习、射线追踪、并行优化等研究方向，共 46 篇。

---

## 四、安全与版权 {#cat-security}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-31 | [Comparative](./3dgs_2026-01.md#2-comparative-analysis-of-differential-and-collision-entropy-for-finite-regime-qkd-in-hybrid-quantum-noisy-channels) | 2602.00705 | 混合量子信道,熵度量,高斯混合模型,有限密钥QKD,量子安全 |

**概要**: 本类论文涉及有限密钥QKD、量子安全、高斯混合模型、混合量子信道、熵度量等研究方向，共 1 篇。

---

## 五、无线与射频传播 {#cat-rf}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-31 | [Comparative](./3dgs_2026-01.md#2-comparative-analysis-of-differential-and-collision-entropy-for-finite-regime-qkd-in-hybrid-quantum-noisy-channels) | 2602.00705 | 混合量子信道,熵度量,高斯混合模型,有限密钥QKD,量子安全 |
| 2026-01-23 | [FarView](./3dgs_2026-01.md#2-the-farview-low-frequency-radio-array-on-the-moon-s-far-side-science-and-array-architecture) | 2601.16170 | 低频射电阵列,波束成形,21厘米信号,宇宙黑暗时代 |
| 2026-01-08 | [SPARK](./3dgs_2026-01.md#3-spark-sparse-parametric-antenna-representation-using-kernels) | 2601.05440 | 天线方向图压缩, 免训练模型, 球谐函数, 高斯核, 波束管理 |

**概要**: 本类论文涉及有限密钥QKD、球谐函数、天线方向图压缩、宇宙黑暗时代、免训练模型、高斯核、波束管理、21厘米信号等研究方向，共 3 篇。

---

## 六、风格迁移与编辑 {#cat-style-edit}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-31 | ★ **[Tune-Your-Style](./3dgs_2026-01.md#3-tune-your-style-intensity-tunable-3d-style-transfer-with-gaussian-splatting)** | 2602.00618 | 3D高斯溅射,风格迁移,强度可调,扩散模型引导 ICCV'25 |
| 2026-01-31 | [EKS](./3dgs_2026-01.md#6-affine-equivariant-kernel-space-encoding-for-nerf-editing) | 2508.02831 | 神经辐射场,高斯核编码,特征蒸馏,局部编辑 |
| 2026-01-27 | [DiffStyle3D](./3dgs_2026-01.md#2-diffstyle3d-consistent-3d-gaussian-stylization-via-attention-optimization) | 2601.19717 | 3D高斯溅射,风格迁移,扩散模型,注意力优化,多视图一致性 |
| 2026-01-22 | [ToonifyGB](./3dgs_2026-01.md#6-toonifygb-stylegan-based-gaussian-blendshapes-for-3d-stylized-head-avatars) | 2505.10072 | 3D高斯混合形变, StyleGAN, 风格化数字人, 表情动画 |
| 2026-01-12 | [3DGS-Drag](./3dgs_2026-01.md#2-3dgs-drag-dragging-gaussians-for-intuitive-point-based-3d-editing) | 2601.07963 | 3D高斯溅射, 拖拽编辑, 扩散模型引导, 渐进式策略, 几何编辑 |
| 2026-01-10 | [TRASE](./3dgs_2026-01.md#4-trase-tracking-free-4d-segmentation-and-editing) | 2411.19290 | 4D分割,动态场景理解,对比学习,高斯原语,场景编辑 |
| 2026-01-08 | [GaussianSwap](./3dgs_2026-01.md#2-gaussianswap-animatable-video-face-swapping-with-3d-gaussian-splatting) | 2601.05511 | 3D高斯溅射,FLAME模型绑定,复合身份嵌入,视频换脸,可交互数字人 |
| 2026-01-06 | [CaricatureGS](./3dgs_2026-01.md#3-caricaturegs-exaggerating-3d-gaussian-splatting-faces-with-gaussian-curvature) | 2601.03319 | 3D高斯泼溅,高斯曲率,面部卡通化,实时渲染 |
| 2026-01-05 | [ESGaussianFace](./3dgs_2026-01.md#4-esgaussianface-emotional-and-stylized-audio-driven-facial-animation-via-3d-gaussian-splatting) | 2601.01847 | 3D高斯溅射,音频驱动面部动画,情感注意力,多阶段训练,风格化生成 |

**概要**: 本类论文涉及局部编辑、高斯核编码、场景编辑、渐进式策略、3D高斯泼溅、音频驱动面部动画、多阶段训练、几何编辑等研究方向，共 9 篇。

---

## 七、语义分割与场景理解 {#cat-seg-understand}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-31 | [NPNet](./3dgs_2026-01.md#4-npnet-a-non-parametric-network-with-adaptive-gaussian-fourier-positional-encoding-for-3d-classification-and-segmentation) | 2602.00542 | 无参网络,自适应高斯傅里叶编码,3D点云分割,少样本学习 |
| 2026-01-30 | [GaussianOcc3D](./3dgs_2026-01.md#5-gaussianocc3d-a-gaussian-based-adaptive-multi-modal-3d-occupancy-prediction) | 2601.22729 | 3D高斯表示,多模态融合,3D占据预测,状态空间模型,自动驾驶 |
| 2026-01-28 | [LangGS-SLAM](./3dgs_2026-01.md#1-langgs-slam-real-time-language-feature-gaussian-splatting-slam) | 2602.06991 | 高斯溅射,SLAM,语言对齐特征,Top-K渲染,混合场优化 |
| 2026-01-27 | [TIGaussian](./3dgs_2026-01.md#4-tigaussian-disentangle-gaussians-for-spatial-awared-text-image-3d-alignment) | 2601.19247 | 3D高斯溅射,跨模态对齐,多分支分词器,扩散先验,空间感知 |
| 2026-01-25 | [SceneSplat++](./3dgs_2026-01.md#4-scenesplat-a-large-dataset-and-comprehensive-benchmark-for-language-gaussian-splatting) | 2506.08710 | 3D高斯溅射,语言场景理解,泛化范式,语义分割,大规模基准 |
| 2026-01-20 | [Gaussian](./3dgs_2026-01.md#1-gaussian-based-adaptive-multi-modal-3d-semantic-occupancy-prediction) | 2601.14448 | 3D高斯模型,多模态融合,语义占据预测,状态空间模型,自适应校准 |
| 2026-01-20 | [SuperGSeg](./3dgs_2026-01.md#6-supergseg-open-vocabulary-3d-segmentation-with-structured-super-gaussians) | 2412.10231 | 3D高斯泼溅,开放词汇分割,语言特征蒸馏,结构化高斯,场景理解 |
| 2026-01-19 | [CSGaussian](./3dgs_2026-01.md#4-csgaussian-progressive-rate-distortion-compression-and-segmentation-for-3d-gaussian-splatting) | 2601.12814 | 3D高斯溅射,率失真压缩,语义分割,压缩引导学习,隐式神经超先验 |
| 2026-01-18 | [GaussianTrimmer](./3dgs_2026-01.md#1-gaussiantrimmer-online-trimming-boundaries-for-3dgs-segmentation) | 2601.12683 | 3D高斯分割,边界修剪,虚拟相机,即插即用后处理 |
| 2026-01-18 | [ProFuse](./3dgs_2026-01.md#3-profuse-efficient-cross-view-context-fusion-for-open-vocabulary-3d-gaussian-splatting) | 2601.04754 | 3D高斯泼溅,开放词汇理解,跨视图融合,语义配准 |
| 2026-01-12 | [CLIP-GS](./3dgs_2026-01.md#8-clip-gs-unifying-vision-language-representation-with-3d-gaussian-splatting) | 2412.19142 | 3D高斯溅射,多模态表示学习,对比学习,图像投票损失 |
| 2026-01-10 | [E2-BKI](./3dgs_2026-01.md#2-e2-bki-evidential-ellipsoidal-bayesian-kernel-inference-for-uncertainty-aware-gaussian-semantic-mapping) | 2509.11964 | 证据深度学习,贝叶斯核推理,高斯表示,不确定性感知,语义建图 |
| 2026-01-10 | [TRASE](./3dgs_2026-01.md#4-trase-tracking-free-4d-segmentation-and-editing) | 2411.19290 | 4D分割,动态场景理解,对比学习,高斯原语,场景编辑 |
| 2026-01-08 | [InnerGS](./3dgs_2026-01.md#6-innergs-internal-scenes-reconstruction-and-segmentation-via-factorized-3d-gaussian-splatting) | 2508.13287 | 3D高斯泼溅,内部场景重建,文本引导分割,连续体密度建模 |
| 2026-01-06 | [SAGOnline](./3dgs_2026-01.md#4-sagonline-segment-any-gaussians-online) | 2508.08219 | 3D高斯溅射,零样本分割,几何共识,实时推理,视频基础模型 |
| 2026-01-05 | ★ **[Joint3DGS](./3dgs_2026-01.md#1-joint-semantic-and-rendering-enhancements-in-3d-gaussian-modeling-with-anisotropic-local-encoding)** | 2601.02339 | 3D高斯溅射,语义分割,各向异性编码,跨场景迁移,联合优化 ICCV'25 |

**概要**: 本类论文涉及语义占据预测、无参网络、证据深度学习、场景编辑、不确定性感知、语义配准、3D高斯分割、少样本学习等研究方向，共 16 篇。

---

## 八、领域应用 {#cat-domain-app}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-31 | [GaussianEM](./3dgs_2026-01.md#5-resolving-compositional-and-conformational-heterogeneity-in-cryo-em-with-deformable-3d-gaussian-representations) | 2512.21599 | 3D高斯表示,冷冻电镜,构象异质性,伪原子框架,结构重建 |
| 2026-01-30 | [Diachronic](./3dgs_2026-01.md#4-diachronic-stereo-matching-for-multi-date-satellite-imagery) | 2601.22808 | 历时立体匹配,跨期卫星影像,单目深度先验,三维重建 |
| 2026-01-30 | [Pose Splatter](./3dgs_2026-01.md#9-pose-splatter-a-3d-gaussian-splatting-model-for-quantifying-animal-pose-and-appearance) | 2505.18342 | 3D高斯溅射,形状雕刻,动物姿态估计,无标注建模,视觉嵌入 |
| 2026-01-29 | [SynRealShip](./3dgs_2026-01.md#1-synthetic-to-real-domain-bridging-for-single-view-3d-reconstruction-of-ships-for-maritime-monitoring) | 2601.21786 | 单视角重建,3D高斯,域适应,船舶监控,合成数据训练 |
| 2026-01-27 | [WaterClear-GS](./3dgs_2026-01.md#1-waterclear-gs-optical-aware-gaussian-splatting-for-underwater-reconstruction-and-restoration) | 2601.19753 | 3D高斯泼溅,水下三维重建,光学特性建模,新视角合成,图像恢复 |
| 2026-01-27 | [ClipGS-VR](./3dgs_2026-01.md#3-clipgs-vr-immersive-and-interactive-cinematic-visualization-of-volumetric-medical-data-in-mobile-virtual-reality) | 2601.19310 | 3D高斯溅射,虚拟现实,医学可视化,实时渲染,透明度调制 |
| 2026-01-23 | [GlassesGB](./3dgs_2026-01.md#1-glassesgb-controllable-2d-gan-based-eyewear-personalization-for-3d-gaussian-blendshapes-head-avatars) | 2601.17088 | 3D高斯混合形状,2D生成对抗网络,虚拟试戴,数字人头像,可定制眼镜 |
| 2026-01-23 | [FarView](./3dgs_2026-01.md#2-the-farview-low-frequency-radio-array-on-the-moon-s-far-side-science-and-array-architecture) | 2601.16170 | 低频射电阵列,波束成形,21厘米信号,宇宙黑暗时代 |
| 2026-01-22 | [GS-DT](./3dgs_2026-01.md#1-three-dimensional-damage-visualization-of-civil-structures-via-gaussian-splatting-enabled-digital-twins) | 2602.16713 | 高斯溅射,数字孪生,三维重建,损伤可视化,多尺度策略 |
| 2026-01-22 | [NoMesh](./3dgs_2026-01.md#4-no-mesh-no-problem-estimating-coral-volume-and-surface-from-sparse-multi-view-images) | 2509.11164 | 稀疏多视角,点云融合,体积表面积估算,不确定性估计,珊瑚几何重建 |
| 2026-01-21 | [SplatBus](./3dgs_2026-01.md#1-splatbus-a-gaussian-splatting-viewer-framework-via-gpu-interprocess-communication) | 2601.15431 | 3D高斯溅射, GPU进程间通信, 实时渲染, 渲染管线集成 |
| 2026-01-20 | [RigAware](./3dgs_2026-01.md#2-rig-aware-3d-reconstruction-of-vehicle-undercarriages-using-gaussian-splatting) | 2601.14208 | 高斯泼溅,支架感知SfM,三维重建,实时渲染,车辆检测 |
| 2026-01-19 | [BladeSDF](./3dgs_2026-01.md#1-bladesdf-unconditional-and-conditional-generative-modeling-of-representative-blade-geometries-using-signed-distance-functions) | 2601.13445 | 符号距离函数,隐式生成模型,涡轮叶片设计,潜空间建模,性能条件生成 |
| 2026-01-19 | [OceanSplat](./3dgs_2026-01.md#7-oceansplat-object-aware-gaussian-splatting-with-trinocular-view-consistency-for-underwater-scene-reconstruction) | 2601.04984 | 3D高斯泼溅,三眼视图一致性,深度正则化,水下重建 |
| 2026-01-17 | [ActiveMapping](./3dgs_2026-01.md#1-active-semantic-mapping-of-horticultural-environments-using-gaussian-splatting) | 2601.12122 | 3D高斯泼溅,主动语义建图,移动机器人,Octomap,农业场景 |
| 2026-01-16 | [ARKS](./3dgs_2026-01.md#1-the-alma-survey-to-resolve-exokuiper-belt-substructures-arks-vii-optically-thick-gas-with-broad-co-gaussian-local-line-profiles-in-the-hd-121617-disc) | 2601.11824 | ALMA观测,碎片盘,CO谱线分析,辐射传输建模,光学厚度 |
| 2026-01-13 | [PINGS-X](./3dgs_2026-01.md#1-pings-x-physics-informed-normalized-gaussian-splatting-with-axes-alignment-for-efficient-super-resolution-of-4d-flow-mri) | 2511.11048 | 高斯溅射,4D血流MRI,超分辨率,轴对齐表示,物理约束 |
| 2026-01-12 | [VEG](./3dgs_2026-01.md#6-volume-encoding-gaussians-transfer-function-agnostic-3d-gaussians-for-volume-rendering) | 2504.13339 | 3D高斯,体渲染,传输函数,标量场编码,可微渲染 |
| 2026-01-09 | [NAS-GS](./3dgs_2026-01.md#3-nas-gs-noise-aware-sonar-gaussian-splatting) | 2601.06285 | 声呐高斯溅射,双向渲染,高斯混合噪声模型,新视角合成,三维重建 |
| 2026-01-09 | [MultiTask](./3dgs_2026-01.md#4-multi-task-modeling-for-engineering-applications-with-sparse-data) | 2601.05910 | 多任务高斯过程,多保真数据,稀疏数据建模,任务关联,工程预测 |
| 2026-01-08 | [InnerGS](./3dgs_2026-01.md#6-innergs-internal-scenes-reconstruction-and-segmentation-via-factorized-3d-gaussian-splatting) | 2508.13287 | 3D高斯泼溅,内部场景重建,文本引导分割,连续体密度建模 |

**概要**: 本类论文涉及深度正则化、伪原子框架、2D生成对抗网络、多保真数据、跨期卫星影像、透明度调制、符号距离函数、光学厚度等研究方向，共 21 篇。

---

## 九、生成式模型 {#cat-generative}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-30 | [PSGS](./3dgs_2026-01.md#1-psgs-text-driven-panorama-sliding-scene-generation-via-gaussian-splatting) | 2602.00463 | 文本驱动生成,全景滑动机制,3D高斯溅射,多模态反馈,语义一致性 |
| 2026-01-30 | [CacheFlow](./3dgs_2026-01.md#10-cacheflow-fast-human-motion-prediction-by-cached-normalizing-flow) | 2505.13140 | 正常化流, 人体运动预测, 缓存机制, 密度估计, 生成模型 |
| 2026-01-29 | [Efficient4D](./3dgs_2026-01.md#6-efficient4d-fast-dynamic-3d-object-generation-from-a-single-view-video) | 2401.08742 | 4D高斯溅射,分数蒸馏,置信度加权损失,动态场景生成,实时渲染 |
| 2026-01-28 | [FreeFix](./3dgs_2026-01.md#2-freefix-boosting-3d-gaussian-splatting-via-fine-tuning-free-diffusion-models) | 2601.20857 | 3D高斯泼溅,扩散模型,免微调优化,2D-3D交替细化,置信度掩码 |
| 2026-01-28 | [WaveletGaussian](./3dgs_2026-01.md#6-waveletgaussian-wavelet-domain-diffusion-for-sparse-view-3d-gaussian-object-reconstruction) | 2509.19073 | 小波域扩散,稀疏视角重建,3D高斯溅射,训练加速 |
| 2026-01-27 | [DiffStyle3D](./3dgs_2026-01.md#2-diffstyle3d-consistent-3d-gaussian-stylization-via-attention-optimization) | 2601.19717 | 3D高斯溅射,风格迁移,扩散模型,注意力优化,多视图一致性 |
| 2026-01-27 | [PromptVFX](./3dgs_2026-01.md#7-promptvfx-text-driven-fields-for-open-world-3d-gaussian-animation) | 2506.01091 | 3D高斯,文本驱动,4D流场,大模型,视觉特效 |
| 2026-01-26 | [UA-3DTalk](./3dgs_2026-01.md#1-uncertainty-aware-3d-emotional-talking-face-synthesis-with-emotion-prior-distillation) | 2601.19112 | 3D说话人脸合成,情感蒸馏,不确定性估计,4D高斯编码,多视图融合 |
| 2026-01-26 | [Splat-Portrait](./3dgs_2026-01.md#2-splat-portrait-generalizing-talking-heads-with-gaussian-splatting) | 2601.18633 | 高斯溅射,说话人头生成,音频驱动,3D重建,分数蒸馏 |
| 2026-01-26 | [HeadLighter](./3dgs_2026-01.md#5-headlighter-disentangling-illumination-in-generative-3d-gaussian-heads-via-lightstage-captures) | 2601.02103 | 3D高斯溅射,光照解耦,光棚捕获,可控重光照 |
| 2026-01-24 | [Mirage2Matter](./3dgs_2026-01.md#1-mirage2matter-a-physically-grounded-gaussian-world-model-from-video) | 2602.00096 | 3D高斯溅射,世界模型,物理仿真,具身智能 |
| 2026-01-23 | [GlassesGB](./3dgs_2026-01.md#1-glassesgb-controllable-2d-gan-based-eyewear-personalization-for-3d-gaussian-blendshapes-head-avatars) | 2601.17088 | 3D高斯混合形状,2D生成对抗网络,虚拟试戴,数字人头像,可定制眼镜 |
| 2026-01-22 | [CamPilot](./3dgs_2026-01.md#2-campilot-improving-camera-control-in-video-diffusion-model-with-efficient-camera-reward-feedback) | 2601.16214 | 视频扩散模型,相机控制,3D高斯解码,奖励反馈学习 |
| 2026-01-22 | [CGS-GAN](./3dgs_2026-01.md#5-cgs-gan-3d-consistent-gaussian-splatting-gans-for-high-resolution-human-head-synthesis) | 2505.17590 | 3D高斯溅射,生成对抗网络,三维一致性,高分辨率人脸合成 |
| 2026-01-22 | [ToonifyGB](./3dgs_2026-01.md#6-toonifygb-stylegan-based-gaussian-blendshapes-for-3d-stylized-head-avatars) | 2505.10072 | 3D高斯混合形变, StyleGAN, 风格化数字人, 表情动画 |
| 2026-01-21 | [ScenDi](./3dgs_2026-01.md#2-scendi-3d-to-2d-scene-diffusion-cascades-for-urban-generation) | 2601.15221 | 3D高斯,视频扩散模型,城市场景生成,级联架构,可控生成 |
| 2026-01-20 | [OneShotRefiner](./3dgs_2026-01.md#3-one-shot-refiner-boosting-feed-forward-novel-view-synthesis-via-one-step-diffusion) | 2601.14161 | 新视角合成, 3D高斯溅射, 扩散模型, 双域感知, 联合优化 |
| 2026-01-20 | ★ **[RI3D](./3dgs_2026-01.md#5-ri3d-few-shot-gaussian-splatting-with-repair-and-inpainting-diffusion-priors)** | 2503.10860 | 3D高斯泼溅,扩散模型,新视角合成,两阶段优化,深度初始化 ICCV'25 |
| 2026-01-19 | [BladeSDF](./3dgs_2026-01.md#1-bladesdf-unconditional-and-conditional-generative-modeling-of-representative-blade-geometries-using-signed-distance-functions) | 2601.13445 | 符号距离函数,隐式生成模型,涡轮叶片设计,潜空间建模,性能条件生成 |
| 2026-01-15 | [RSATalker](./3dgs_2026-01.md#1-rsatalker-realistic-socially-aware-talking-head-generation-for-multi-turn-conversation) | 2601.10606 | 3D高斯溅射,数字人生成,社会关系感知,多轮对话 |
| 2026-01-15 | [ELITE](./3dgs_2026-01.md#2-elite-efficient-gaussian-head-avatar-from-a-monocular-video-via-learned-initialization-and-test-time-generative-adaptation) | 2601.10200 | 高斯数字人,单目视频,先验初始化,单步扩散增强,测试时自适应 |
| 2026-01-12 | [3DGS-Drag](./3dgs_2026-01.md#2-3dgs-drag-dragging-gaussians-for-intuitive-point-based-3d-editing) | 2601.07963 | 3D高斯溅射, 拖拽编辑, 扩散模型引导, 渐进式策略, 几何编辑 |
| 2026-01-09 | [RigMo](./3dgs_2026-01.md#2-rigmo-unifying-rig-and-motion-learning-for-generative-animation) | 2601.06378 | 骨架绑定,动作生成,潜空间编码,动态3D建模 |
| 2026-01-09 | [LayerGS](./3dgs_2026-01.md#5-layergs-decomposition-and-inpainting-of-layered-3d-human-avatars-via-2d-gaussian-splatting) | 2601.05853 | 2D高斯溅射,扩散模型修复,人体分层重建,虚拟试穿 |
| 2026-01-08 | [Akasha 2](./3dgs_2026-01.md#1-akasha-2-hamiltonian-state-space-duality-and-visual-language-joint-embedding-predictive-architectur) | 2601.06212 | 哈密顿状态空间,视语联合预测,物理守恒,3D高斯溅射,流匹配 |
| 2026-01-08 | [GaussianSwap](./3dgs_2026-01.md#2-gaussianswap-animatable-video-face-swapping-with-3d-gaussian-splatting) | 2601.05511 | 3D高斯溅射,FLAME模型绑定,复合身份嵌入,视频换脸,可交互数字人 |
| 2026-01-05 | [InpaintHuman](./3dgs_2026-01.md#3-inpainthuman-reconstructing-occluded-humans-with-multi-scale-uv-mapping-and-identity-preserving-diffusion-inpainting) | 2601.02098 | 人体重建,扩散修复,UV映射,身份保持,遮挡处理 |
| 2026-01-05 | [ESGaussianFace](./3dgs_2026-01.md#4-esgaussianface-emotional-and-stylized-audio-driven-facial-animation-via-3d-gaussian-splatting) | 2601.01847 | 3D高斯溅射,音频驱动面部动画,情感注意力,多阶段训练,风格化生成 |
| 2026-01-04 | [MANGO](./3dgs_2026-01.md#1-mango-natural-multi-speaker-3d-talking-head-generation-via-2d-lifted-enhancement) | 2601.01749 | 音频驱动,3D高斯渲染,扩散模型,多人对话,2D监督 |
| 2026-01-04 | [MeSS](./3dgs_2026-01.md#6-mess-city-mesh-guided-outdoor-scene-generation-with-cross-view-consistent-diffusion) | 2508.15169 | 城市网格引导,跨视角扩散模型,3D高斯溅射,场景生成,几何对齐 |
| 2026-01-01 | [JGA-LBD](./3dgs_2026-01.md#2-joint-geometry-appearance-human-reconstruction-in-a-unified-latent-space-via-bridge-diffusion) | 2601.00328 | 桥扩散模型,联合隐空间,3D高斯表示,数字人重建 |

**概要**: 本类论文涉及说话人头生成、2D生成对抗网络、文本驱动、骨架绑定、世界模型、符号距离函数、多轮对话、城市网格引导等研究方向，共 31 篇。

---

## 十、新视角合成 {#cat-nvs}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-30 | [PSGS](./3dgs_2026-01.md#1-psgs-text-driven-panorama-sliding-scene-generation-via-gaussian-splatting) | 2602.00463 | 文本驱动生成,全景滑动机制,3D高斯溅射,多模态反馈,语义一致性 |
| 2026-01-29 | [Efficient4D](./3dgs_2026-01.md#6-efficient4d-fast-dynamic-3d-object-generation-from-a-single-view-video) | 2401.08742 | 4D高斯溅射,分数蒸馏,置信度加权损失,动态场景生成,实时渲染 |
| 2026-01-28 | [FreeFix](./3dgs_2026-01.md#2-freefix-boosting-3d-gaussian-splatting-via-fine-tuning-free-diffusion-models) | 2601.20857 | 3D高斯泼溅,扩散模型,免微调优化,2D-3D交替细化,置信度掩码 |
| 2026-01-28 | ★ **[HDR-4DGS](./3dgs_2026-01.md#5-dynamic-novel-view-synthesis-in-high-dynamic-range)** | 2509.21853 | 高斯泼溅,动态色调映射,高动态范围,新视角合成 ICLR'26 |
| 2026-01-27 | [WaterClear-GS](./3dgs_2026-01.md#1-waterclear-gs-optical-aware-gaussian-splatting-for-underwater-reconstruction-and-restoration) | 2601.19753 | 3D高斯泼溅,水下三维重建,光学特性建模,新视角合成,图像恢复 |
| 2026-01-27 | [GDAGS](./3dgs_2026-01.md#6-gradient-direction-aware-density-control-for-3d-gaussian-splatting) | 2508.09239 | 3D高斯泼溅,密度控制,梯度方向感知,新视角合成 |
| 2026-01-26 | [Splat-Portrait](./3dgs_2026-01.md#2-splat-portrait-generalizing-talking-heads-with-gaussian-splatting) | 2601.18633 | 高斯溅射,说话人头生成,音频驱动,3D重建,分数蒸馏 |
| 2026-01-26 | [StreamLoD-GS](./3dgs_2026-01.md#4-lod-structured-3d-gaussian-splatting-for-streaming-video-reconstruction) | 2601.18475 | 3D高斯溅射,细节层次结构,动态场景分割,流式视频重建,量化压缩 |
| 2026-01-22 | [CamPilot](./3dgs_2026-01.md#2-campilot-improving-camera-control-in-video-diffusion-model-with-efficient-camera-reward-feedback) | 2601.16214 | 视频扩散模型,相机控制,3D高斯解码,奖励反馈学习 |
| 2026-01-22 | [EVolSplat4D](./3dgs_2026-01.md#3-evolsplat4d-efficient-volume-based-gaussian-splatting-for-4d-urban-scene-synthesis) | 2601.15951 | 高斯溅射,新视角合成,4D场景重建,前馈网络,体积预测 |
| 2026-01-21 | [ConeGS](./3dgs_2026-01.md#5-conegs-error-guided-densification-using-pixel-cones-for-improved-reconstruction-with-fewer-primitives) | 2511.06810 | 3D高斯溅射,视锥引导,误差引导优化,基元预算,新视角合成 |
| 2026-01-20 | [OneShotRefiner](./3dgs_2026-01.md#3-one-shot-refiner-boosting-feed-forward-novel-view-synthesis-via-one-step-diffusion) | 2601.14161 | 新视角合成, 3D高斯溅射, 扩散模型, 双域感知, 联合优化 |
| 2026-01-20 | ★ **[RI3D](./3dgs_2026-01.md#5-ri3d-few-shot-gaussian-splatting-with-repair-and-inpainting-diffusion-priors)** | 2503.10860 | 3D高斯泼溅,扩散模型,新视角合成,两阶段优化,深度初始化 ICCV'25 |
| 2026-01-20 | [Deblur4DGS](./3dgs_2026-01.md#7-deblur4dgs-4d-gaussian-splatting-from-blurry-monocular-video) | 2412.06424 | 4D高斯溅射,运动模糊处理,曝光时间估计,动态场景重建,视频增强 |
| 2026-01-19 | [GaussExplorer](./3dgs_2026-01.md#3-gaussexplorer-3d-gaussian-splatting-for-embodied-exploration-and-reasoning) | 2601.13132 | 3D高斯泼溅,视觉语言模型,具身探索,新视角合成,场景推理 |
| 2026-01-19 | [FHAvatar](./3dgs_2026-01.md#5-generalizable-and-animatable-3d-full-head-gaussian-avatar-from-a-single-image) | 2601.12770 | 单图重建,高斯基元,3D GAN先验,数字人动画,UV空间映射 |
| 2026-01-19 | [OceanSplat](./3dgs_2026-01.md#7-oceansplat-object-aware-gaussian-splatting-with-trinocular-view-consistency-for-underwater-scene-reconstruction) | 2601.04984 | 3D高斯泼溅,三眼视图一致性,深度正则化,水下重建 |
| 2026-01-16 | [studentSplat](./3dgs_2026-01.md#2-studentsplat-your-student-model-learns-single-view-3d-gaussian-splatting) | 2601.11772 | 单视图重建, 3D高斯泼溅, 师生架构, 外推网络, 尺度模糊 |
| 2026-01-14 | [JOGS](./3dgs_2026-01.md#4-jogs-joint-optimization-of-pose-estimation-and-3d-gaussian-splatting) | 2510.26117 | 3D高斯溅射,相机位姿估计,联合优化,可微渲染,3D光流 |
| 2026-01-12 | [R3-RECON](./3dgs_2026-01.md#4-r3-recon-radiance-field-free-active-reconstruction-via-renderability) | 2601.07484 | 主动重建, 视点规划, 可渲染性场, 体素地图, 新视角合成 |
| 2026-01-12 | [VEG](./3dgs_2026-01.md#6-volume-encoding-gaussians-transfer-function-agnostic-3d-gaussians-for-volume-rendering) | 2504.13339 | 3D高斯,体渲染,传输函数,标量场编码,可微渲染 |
| 2026-01-09 | [NAS-GS](./3dgs_2026-01.md#3-nas-gs-noise-aware-sonar-gaussian-splatting) | 2601.06285 | 声呐高斯溅射,双向渲染,高斯混合噪声模型,新视角合成,三维重建 |
| 2026-01-09 | [FreqGS](./3dgs_2026-01.md#7-frequency-aware-gaussian-splatting-decomposition) | 2503.21226 | 3D高斯溅射,频率感知分解,拉普拉斯金字塔,细节层次渲染 |
| 2026-01-07 | [SCAR-GS](./3dgs_2026-01.md#1-scar-gs-spatial-context-attention-for-residuals-in-progressive-gaussian-splatting) | 2601.04348 | 3D高斯溅射,渐进式压缩,残差矢量量化,自回归熵模型 |
| 2026-01-05 | [360-GeoGS](./3dgs_2026-01.md#2-360-geogs-geometrically-consistent-feed-forward-3d-gaussian-splatting-reconstruction-for-360-images) | 2601.02102 | 3D高斯泼溅,前馈重建,几何一致性,深度法向正则化 |
| 2026-01-04 | [ShadowGS](./3dgs_2026-01.md#4-shadowgs-shadow-aware-3d-gaussian-splatting-for-satellite-imagery) | 2601.00939 | 3D高斯泼溅,阴影建模,卫星影像重建,物理渲染,新视角合成 |
| 2026-01-04 | [AHA](./3dgs_2026-01.md#5-aha-animating-human-avatars-in-diverse-scenes-with-gaussian-splatting) | 2511.09827 | 3D高斯溅射,人物动画,运动合成,自由视角渲染,场景交互 |
| 2026-01-04 | [MeSS](./3dgs_2026-01.md#6-mess-city-mesh-guided-outdoor-scene-generation-with-cross-view-consistent-diffusion) | 2508.15169 | 城市网格引导,跨视角扩散模型,3D高斯溅射,场景生成,几何对齐 |
| 2026-01-03 | [AH-GS](./3dgs_2026-01.md#1-ah-gs-augmented-3d-gaussian-splatting-for-high-frequency-detail-representation) | 2503.22324 | 3D高斯溅射,高频细节表示,特征编码,渲染优化,损失函数 |
| 2026-01-01 | [JGA-LBD](./3dgs_2026-01.md#2-joint-geometry-appearance-human-reconstruction-in-a-unified-latent-space-via-bridge-diffusion) | 2601.00328 | 桥扩散模型,联合隐空间,3D高斯表示,数字人重建 |
| 2026-01-01 | [Stereo-GS](./3dgs_2026-01.md#3-stereo-gs-multi-view-stereo-vision-model-for-generalizable-3d-gaussian-splatting-reconstruction) | 2507.14921 | 3D高斯泼溅,立体视觉,几何外观解耦,免位姿重建 |

**概要**: 本类论文涉及阴影建模、深度正则化、说话人头生成、动态场景分割、物理渲染、基元预算、细节层次结构、可渲染性场等研究方向，共 31 篇。

---

## 十一、机器人仿真与具身智能 {#cat-robotics}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-30 | [GeoRep](./3dgs_2026-01.md#3-learning-geometrically-grounded-3d-visual-representations-for-view-generalizable-robotic-manipulation) | 2601.22988 | 单视角3D预训练,高斯溅射,多步蒸馏,视角泛化 |
| 2026-01-30 | [RoboArmGS](./3dgs_2026-01.md#7-roboarmgs-high-quality-robotic-arm-splatting-via-b-zier-curve-refinement) | 2511.17961 | 3D高斯溅射,贝塞尔曲线优化,机械臂运动建模,数字资产重建 |
| 2026-01-26 | [ExoGS](./3dgs_2026-01.md#3-exogs-a-4d-real-to-sim-to-real-framework-for-scalable-manipulation-data-collection) | 2601.18629 | 真仿真迁移,3D高斯重建,被动外骨骼,操作数据收集,策略泛化 |
| 2026-01-24 | [Mirage2Matter](./3dgs_2026-01.md#1-mirage2matter-a-physically-grounded-gaussian-world-model-from-video) | 2602.00096 | 3D高斯溅射,世界模型,物理仿真,具身智能 |
| 2026-01-19 | [GaussExplorer](./3dgs_2026-01.md#3-gaussexplorer-3d-gaussian-splatting-for-embodied-exploration-and-reasoning) | 2601.13132 | 3D高斯泼溅,视觉语言模型,具身探索,新视角合成,场景推理 |
| 2026-01-17 | [ActiveMapping](./3dgs_2026-01.md#1-active-semantic-mapping-of-horticultural-environments-using-gaussian-splatting) | 2601.12122 | 3D高斯泼溅,主动语义建图,移动机器人,Octomap,农业场景 |
| 2026-01-10 | [3DSceneRep](./3dgs_2026-01.md#1-what-is-the-best-3d-scene-representation-for-robotics-from-geometric-to-foundation-models) | 2512.03422 | 三维场景表示,机器人系统,神经表示,3D高斯泼溅,基础模型 |

**概要**: 本类论文涉及数字资产重建、单视角3D预训练、机械臂运动建模、机器人系统、多步蒸馏、Octomap、3D高斯泼溅、主动语义建图等研究方向，共 7 篇。

---

## 十二、自动驾驶应用 {#cat-autodrive}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-30 | [GaussianOcc3D](./3dgs_2026-01.md#5-gaussianocc3d-a-gaussian-based-adaptive-multi-modal-3d-occupancy-prediction) | 2601.22729 | 3D高斯表示,多模态融合,3D占据预测,状态空间模型,自动驾驶 |
| 2026-01-25 | [CrossLevel](./3dgs_2026-01.md#3-cross-level-sensor-fusion-with-object-lists-via-transformer-for-3d-object-detection) | 2512.12884 | 跨层级融合,Transformer,3D目标检测,传感器融合,可变形掩码 |
| 2026-01-22 | [EVolSplat4D](./3dgs_2026-01.md#3-evolsplat4d-efficient-volume-based-gaussian-splatting-for-4d-urban-scene-synthesis) | 2601.15951 | 高斯溅射,新视角合成,4D场景重建,前馈网络,体积预测 |
| 2026-01-21 | [ScenDi](./3dgs_2026-01.md#2-scendi-3d-to-2d-scene-diffusion-cascades-for-urban-generation) | 2601.15221 | 3D高斯,视频扩散模型,城市场景生成,级联架构,可控生成 |
| 2026-01-20 | [Gaussian](./3dgs_2026-01.md#1-gaussian-based-adaptive-multi-modal-3d-semantic-occupancy-prediction) | 2601.14448 | 3D高斯模型,多模态融合,语义占据预测,状态空间模型,自适应校准 |
| 2026-01-20 | [ParkingTwin](./3dgs_2026-01.md#4-parkingtwin-training-free-streaming-3d-reconstruction-for-parking-lot-digital-twins) | 2601.13706 | 流式三维重建,OSM先验建图,动态遮挡过滤,光照鲁棒融合 |
| 2026-01-04 | [ParkGaussian](./3dgs_2026-01.md#3-parkgaussian-surround-view-3d-gaussian-splatting-for-autonomous-parking) | 2601.01386 | 3D高斯溅射,泊车场景重建,车位感知引导,环视相机 |

**概要**: 本类论文涉及Transformer、语义占据预测、OSM先验建图、环视相机、泊车场景重建、流式三维重建、状态空间模型、可变形掩码等研究方向，共 7 篇。

---

## 十三、数字人与人体重建 {#cat-human}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-30 | ★ **[FastGHA](./3dgs_2026-01.md#6-fastgha-generalized-few-shot-3d-gaussian-head-avatars-with-real-time-animation)** | 2601.13837 | 3D高斯,数字人重建,实时动画,前向生成,特征融合 ICLR'26 |
| 2026-01-30 | [CacheFlow](./3dgs_2026-01.md#10-cacheflow-fast-human-motion-prediction-by-cached-normalizing-flow) | 2505.13140 | 正常化流, 人体运动预测, 缓存机制, 密度估计, 生成模型 |
| 2026-01-29 | [3DFaceComp](./3dgs_2026-01.md#3-lightweight-high-fidelity-low-bitrate-talking-face-compression-for-3d-video-conference) | 2601.21269 | 3D高斯溅射,参数化人脸建模,低码率压缩,率失真优化,实时渲染 |
| 2026-01-26 | [UA-3DTalk](./3dgs_2026-01.md#1-uncertainty-aware-3d-emotional-talking-face-synthesis-with-emotion-prior-distillation) | 2601.19112 | 3D说话人脸合成,情感蒸馏,不确定性估计,4D高斯编码,多视图融合 |
| 2026-01-26 | [Splat-Portrait](./3dgs_2026-01.md#2-splat-portrait-generalizing-talking-heads-with-gaussian-splatting) | 2601.18633 | 高斯溅射,说话人头生成,音频驱动,3D重建,分数蒸馏 |
| 2026-01-26 | [HeadLighter](./3dgs_2026-01.md#5-headlighter-disentangling-illumination-in-generative-3d-gaussian-heads-via-lightstage-captures) | 2601.02103 | 3D高斯溅射,光照解耦,光棚捕获,可控重光照 |
| 2026-01-23 | [GlassesGB](./3dgs_2026-01.md#1-glassesgb-controllable-2d-gan-based-eyewear-personalization-for-3d-gaussian-blendshapes-head-avatars) | 2601.17088 | 3D高斯混合形状,2D生成对抗网络,虚拟试戴,数字人头像,可定制眼镜 |
| 2026-01-22 | [CGS-GAN](./3dgs_2026-01.md#5-cgs-gan-3d-consistent-gaussian-splatting-gans-for-high-resolution-human-head-synthesis) | 2505.17590 | 3D高斯溅射,生成对抗网络,三维一致性,高分辨率人脸合成 |
| 2026-01-22 | [ToonifyGB](./3dgs_2026-01.md#6-toonifygb-stylegan-based-gaussian-blendshapes-for-3d-stylized-head-avatars) | 2505.10072 | 3D高斯混合形变, StyleGAN, 风格化数字人, 表情动画 |
| 2026-01-21 | [CAG-Avatar](./3dgs_2026-01.md#3-cag-avatar-cross-attention-guided-gaussian-avatars-for-high-fidelity-head-reconstruction) | 2601.14844 | 3D高斯泼溅,交叉注意力,数字人驱动,头部重建,自适应融合 |
| 2026-01-19 | [ICo3D](./3dgs_2026-01.md#2-ico3d-an-interactive-conversational-3d-virtual-human) | 2601.13148 | 高斯溅射,3D虚拟人,大语言模型,实时交互,动态重建 |
| 2026-01-19 | [FHAvatar](./3dgs_2026-01.md#5-generalizable-and-animatable-3d-full-head-gaussian-avatar-from-a-single-image) | 2601.12770 | 单图重建,高斯基元,3D GAN先验,数字人动画,UV空间映射 |
| 2026-01-19 | [KaoLRM](./3dgs_2026-01.md#6-kaolrm-repurposing-pre-trained-large-reconstruction-models-for-parametric-3d-face-reconstruction) | 2601.12736 | 大型重建模型,2D高斯溅射,参数化人脸重建,FLAME模型 |
| 2026-01-15 | [RSATalker](./3dgs_2026-01.md#1-rsatalker-realistic-socially-aware-talking-head-generation-for-multi-turn-conversation) | 2601.10606 | 3D高斯溅射,数字人生成,社会关系感知,多轮对话 |
| 2026-01-15 | [ELITE](./3dgs_2026-01.md#2-elite-efficient-gaussian-head-avatar-from-a-monocular-video-via-learned-initialization-and-test-time-generative-adaptation) | 2601.10200 | 高斯数字人,单目视频,先验初始化,单步扩散增强,测试时自适应 |
| 2026-01-12 | [Mon3tr](./3dgs_2026-01.md#3-mon3tr-monocular-3d-telepresence-with-pre-built-gaussian-avatars-as-amortization) | 2601.07518 | 3D高斯溅射,单目驱动,数字人重建,低带宽传输,实时渲染 |
| 2026-01-09 | [LayerGS](./3dgs_2026-01.md#5-layergs-decomposition-and-inpainting-of-layered-3d-human-avatars-via-2d-gaussian-splatting) | 2601.05853 | 2D高斯溅射,扩散模型修复,人体分层重建,虚拟试穿 |
| 2026-01-08 | [GaussianSwap](./3dgs_2026-01.md#2-gaussianswap-animatable-video-face-swapping-with-3d-gaussian-splatting) | 2601.05511 | 3D高斯溅射,FLAME模型绑定,复合身份嵌入,视频换脸,可交互数字人 |
| 2026-01-06 | [RelightAnyone](./3dgs_2026-01.md#1-relightanyone-a-generalized-relightable-3d-gaussian-head-model) | 2601.03357 | 3D高斯溅射,头部重建,重光照,两阶段学习,跨主体泛化 |
| 2026-01-06 | [CaricatureGS](./3dgs_2026-01.md#3-caricaturegs-exaggerating-3d-gaussian-splatting-faces-with-gaussian-curvature) | 2601.03319 | 3D高斯泼溅,高斯曲率,面部卡通化,实时渲染 |
| 2026-01-05 | [InpaintHuman](./3dgs_2026-01.md#3-inpainthuman-reconstructing-occluded-humans-with-multi-scale-uv-mapping-and-identity-preserving-diffusion-inpainting) | 2601.02098 | 人体重建,扩散修复,UV映射,身份保持,遮挡处理 |
| 2026-01-05 | [ESGaussianFace](./3dgs_2026-01.md#4-esgaussianface-emotional-and-stylized-audio-driven-facial-animation-via-3d-gaussian-splatting) | 2601.01847 | 3D高斯溅射,音频驱动面部动画,情感注意力,多阶段训练,风格化生成 |
| 2026-01-04 | [MANGO](./3dgs_2026-01.md#1-mango-natural-multi-speaker-3d-talking-head-generation-via-2d-lifted-enhancement) | 2601.01749 | 音频驱动,3D高斯渲染,扩散模型,多人对话,2D监督 |
| 2026-01-04 | [DGSM](./3dgs_2026-01.md#2-animated-3dgs-avatars-in-diverse-scenes-with-consistent-lighting-and-shadows) | 2601.01660 | 3D高斯泼溅,深度高斯阴影贴图,实时光照,球谐函数,数字人重光照 |
| 2026-01-04 | [AHA](./3dgs_2026-01.md#5-aha-animating-human-avatars-in-diverse-scenes-with-gaussian-splatting) | 2511.09827 | 3D高斯溅射,人物动画,运动合成,自由视角渲染,场景交互 |
| 2026-01-01 | [JGA-LBD](./3dgs_2026-01.md#2-joint-geometry-appearance-human-reconstruction-in-a-unified-latent-space-via-bridge-diffusion) | 2601.00328 | 桥扩散模型,联合隐空间,3D高斯表示,数字人重建 |

**概要**: 本类论文涉及球谐函数、说话人头生成、2D生成对抗网络、自适应融合、高斯曲率、参数化人脸建模、单图重建、多轮对话等研究方向，共 26 篇。

---

## 十四、动态场景与4D {#cat-dynamic-4d}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-30 | [RoboArmGS](./3dgs_2026-01.md#7-roboarmgs-high-quality-robotic-arm-splatting-via-b-zier-curve-refinement) | 2511.17961 | 3D高斯溅射,贝塞尔曲线优化,机械臂运动建模,数字资产重建 |
| 2026-01-29 | [Efficient4D](./3dgs_2026-01.md#6-efficient4d-fast-dynamic-3d-object-generation-from-a-single-view-video) | 2401.08742 | 4D高斯溅射,分数蒸馏,置信度加权损失,动态场景生成,实时渲染 |
| 2026-01-28 | ★ **[HDR-4DGS](./3dgs_2026-01.md#5-dynamic-novel-view-synthesis-in-high-dynamic-range)** | 2509.21853 | 高斯泼溅,动态色调映射,高动态范围,新视角合成 ICLR'26 |
| 2026-01-27 | [PromptVFX](./3dgs_2026-01.md#7-promptvfx-text-driven-fields-for-open-world-3d-gaussian-animation) | 2506.01091 | 3D高斯,文本驱动,4D流场,大模型,视觉特效 |
| 2026-01-26 | [ExoGS](./3dgs_2026-01.md#3-exogs-a-4d-real-to-sim-to-real-framework-for-scalable-manipulation-data-collection) | 2601.18629 | 真仿真迁移,3D高斯重建,被动外骨骼,操作数据收集,策略泛化 |
| 2026-01-26 | [StreamLoD-GS](./3dgs_2026-01.md#4-lod-structured-3d-gaussian-splatting-for-streaming-video-reconstruction) | 2601.18475 | 3D高斯溅射,细节层次结构,动态场景分割,流式视频重建,量化压缩 |
| 2026-01-22 | [EVolSplat4D](./3dgs_2026-01.md#3-evolsplat4d-efficient-volume-based-gaussian-splatting-for-4d-urban-scene-synthesis) | 2601.15951 | 高斯溅射,新视角合成,4D场景重建,前馈网络,体积预测 |
| 2026-01-20 | [Deblur4DGS](./3dgs_2026-01.md#7-deblur4dgs-4d-gaussian-splatting-from-blurry-monocular-video) | 2412.06424 | 4D高斯溅射,运动模糊处理,曝光时间估计,动态场景重建,视频增强 |
| 2026-01-19 | [Light4GS](./3dgs_2026-01.md#8-light4gs-lightweight-compact-4d-gaussian-splatting-generation-via-context-model) | 2503.13948 | 4D高斯溅射,时空剪枝,上下文模型,数据压缩,动态场景 |
| 2026-01-14 | [GaussianFluent](./3dgs_2026-01.md#2-gaussianfluent-gaussian-simulation-for-dynamic-scenes-with-mixed-materials) | 2601.09265 | 3D高斯泼溅,物理模拟,脆性断裂,物质点法,动态场景 |
| 2026-01-13 | [PINGS-X](./3dgs_2026-01.md#1-pings-x-physics-informed-normalized-gaussian-splatting-with-axes-alignment-for-efficient-super-resolution-of-4d-flow-mri) | 2511.11048 | 高斯溅射,4D血流MRI,超分辨率,轴对齐表示,物理约束 |
| 2026-01-13 | ★ **[Temporal](./3dgs_2026-01.md#2-temporal-smoothness-aware-rate-distortion-optimized-4d-gaussian-splatting)** | 2507.17336 | 4D高斯溅射,率失真优化,小波变换,动态场景压缩,平滑先验 NeurIPS'25 |
| 2026-01-10 | [TRASE](./3dgs_2026-01.md#4-trase-tracking-free-4d-segmentation-and-editing) | 2411.19290 | 4D分割,动态场景理解,对比学习,高斯原语,场景编辑 |
| 2026-01-09 | [RigMo](./3dgs_2026-01.md#2-rigmo-unifying-rig-and-motion-learning-for-generative-animation) | 2601.06378 | 骨架绑定,动作生成,潜空间编码,动态3D建模 |
| 2026-01-09 | [GS-DMSR](./3dgs_2026-01.md#6-gs-dmsr-dynamic-sensitive-multi-scale-manifold-enhancement-for-accelerated-high-quality-3d-gaussian-splatting) | 2601.05584 | 3D高斯溅射,动态场景重建,自适应梯度,流形增强,渲染加速 |
| 2026-01-08 | [MOSAIC-GS](./3dgs_2026-01.md#4-mosaic-gs-monocular-scene-reconstruction-via-advanced-initialization-for-complex-dynamic-environments) | 2601.05368 | 高斯溅射,单目动态重建,几何初始化,傅里叶轨迹 |
| 2026-01-05 | [PMGS](./3dgs_2026-01.md#5-pmgs-reconstruction-of-projectile-motion-across-large-spatiotemporal-spans-via-3d-gaussian-splatting) | 2508.02660 | 3D高斯泼溅,抛体运动重建,物理一致性约束,卡尔曼滤波 |
| 2026-01-04 | [AHA](./3dgs_2026-01.md#5-aha-animating-human-avatars-in-diverse-scenes-with-gaussian-splatting) | 2511.09827 | 3D高斯溅射,人物动画,运动合成,自由视角渲染,场景交互 |
| 2026-01-02 | [AdaGaR](./3dgs_2026-01.md#1-adagar-adaptive-gabor-representation-for-dynamic-scene-reconstruction) | 2601.00796 | 自适应Gabor表示,动态场景重建,时域连续性,三维基元优化,帧插值 |

**概要**: 本类论文涉及帧插值、动态场景分割、文本驱动、物理模拟、骨架绑定、时域连续性、细节层次结构、动态场景重建等研究方向，共 19 篇。

---

## 十五、渲染加速与压缩 {#cat-render-accel}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-29 | [3DFaceComp](./3dgs_2026-01.md#3-lightweight-high-fidelity-low-bitrate-talking-face-compression-for-3d-video-conference) | 2601.21269 | 3D高斯溅射,参数化人脸建模,低码率压缩,率失真优化,实时渲染 |
| 2026-01-29 | [RAVE](./3dgs_2026-01.md#4-rave-rate-adaptive-visual-encoding-for-3d-gaussian-splatting) | 2512.07052 | 3D高斯溅射, 动态码率控制, 神经场景压缩, 免重训插值 |
| 2026-01-28 | [GRTX](./3dgs_2026-01.md#3-grtx-efficient-ray-tracing-for-3d-gaussian-based-rendering) | 2601.20429 | 3D高斯渲染,射线追踪,加速结构优化,硬件协同设计 |
| 2026-01-27 | [ClipGS-VR](./3dgs_2026-01.md#3-clipgs-vr-immersive-and-interactive-cinematic-visualization-of-volumetric-medical-data-in-mobile-virtual-reality) | 2601.19310 | 3D高斯溅射,虚拟现实,医学可视化,实时渲染,透明度调制 |
| 2026-01-26 | [StreamLoD-GS](./3dgs_2026-01.md#4-lod-structured-3d-gaussian-splatting-for-streaming-video-reconstruction) | 2601.18475 | 3D高斯溅射,细节层次结构,动态场景分割,流式视频重建,量化压缩 |
| 2026-01-25 | [Matrix-free](./3dgs_2026-01.md#5-matrix-free-second-order-optimization-of-gaussian-splats-with-residual-sampling) | 2504.12905 | 3D高斯泼溅,二阶优化,免矩阵算法,残差采样,训练加速 |
| 2026-01-21 | [SplatBus](./3dgs_2026-01.md#1-splatbus-a-gaussian-splatting-viewer-framework-via-gpu-interprocess-communication) | 2601.15431 | 3D高斯溅射, GPU进程间通信, 实时渲染, 渲染管线集成 |
| 2026-01-21 | [POTR](./3dgs_2026-01.md#4-potr-post-training-3dgs-compression) | 2601.14821 | 3DGS压缩,并行剪枝,光照系数重算,率失真优化 |
| 2026-01-19 | [CSGaussian](./3dgs_2026-01.md#4-csgaussian-progressive-rate-distortion-compression-and-segmentation-for-3d-gaussian-splatting) | 2601.12814 | 3D高斯溅射,率失真压缩,语义分割,压缩引导学习,隐式神经超先验 |
| 2026-01-19 | [Light4GS](./3dgs_2026-01.md#8-light4gs-lightweight-compact-4d-gaussian-splatting-generation-via-context-model) | 2503.13948 | 4D高斯溅射,时空剪枝,上下文模型,数据压缩,动态场景 |
| 2026-01-14 | [VBM](./3dgs_2026-01.md#1-variable-basis-mapping-for-real-time-volumetric-visualization) | 2601.09417 | 3D高斯溅射,小波分析,闭式映射,体数据可视化,实时渲染 |
| 2026-01-14 | [A^2TG](./3dgs_2026-01.md#3-a-2-tg-adaptive-anisotropic-textured-gaussians-for-efficient-3d-scene-representation) | 2601.09243 | 高斯溅射,各向异性纹理,自适应分配,内存优化 |
| 2026-01-13 | ★ **[Temporal](./3dgs_2026-01.md#2-temporal-smoothness-aware-rate-distortion-optimized-4d-gaussian-splatting)** | 2507.17336 | 4D高斯溅射,率失真优化,小波变换,动态场景压缩,平滑先验 NeurIPS'25 |
| 2026-01-12 | [Mon3tr](./3dgs_2026-01.md#3-mon3tr-monocular-3d-telepresence-with-pre-built-gaussian-avatars-as-amortization) | 2601.07518 | 3D高斯溅射,单目驱动,数字人重建,低带宽传输,实时渲染 |
| 2026-01-12 | [Sketch&Patch++](./3dgs_2026-01.md#5-sketch-amp-patch-efficient-structure-aware-3d-gaussian-representation) | 2601.05394 | 3D高斯表示,分层渐进传输,密度聚类,结构感知编码 |
| 2026-01-09 | [GS-DMSR](./3dgs_2026-01.md#6-gs-dmsr-dynamic-sensitive-multi-scale-manifold-enhancement-for-accelerated-high-quality-3d-gaussian-splatting) | 2601.05584 | 3D高斯溅射,动态场景重建,自适应梯度,流形增强,渲染加速 |
| 2026-01-09 | [FreqGS](./3dgs_2026-01.md#7-frequency-aware-gaussian-splatting-decomposition) | 2503.21226 | 3D高斯溅射,频率感知分解,拉普拉斯金字塔,细节层次渲染 |
| 2026-01-08 | [Akasha 2](./3dgs_2026-01.md#1-akasha-2-hamiltonian-state-space-duality-and-visual-language-joint-embedding-predictive-architectur) | 2601.06212 | 哈密顿状态空间,视语联合预测,物理守恒,3D高斯溅射,流匹配 |
| 2026-01-07 | [SCAR-GS](./3dgs_2026-01.md#1-scar-gs-spatial-context-attention-for-residuals-in-progressive-gaussian-splatting) | 2601.04348 | 3D高斯溅射,渐进式压缩,残差矢量量化,自回归熵模型 |
| 2026-01-01 | [Clean-GS](./3dgs_2026-01.md#1-clean-gs-semantic-mask-guided-pruning-for-3d-gaussian-splatting) | 2601.00913 | 3D高斯溅射,语义掩码,模型剪枝,伪影去除,模型压缩 |

**概要**: 本类论文涉及平滑先验、残差采样、闭式映射、医学可视化、伪影去除、动态码率控制、内存优化、射线追踪等研究方向，共 20 篇。

---

## 十六、流媒体与编码 {#cat-streaming}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-29 | [3DFaceComp](./3dgs_2026-01.md#3-lightweight-high-fidelity-low-bitrate-talking-face-compression-for-3d-video-conference) | 2601.21269 | 3D高斯溅射,参数化人脸建模,低码率压缩,率失真优化,实时渲染 |
| 2026-01-29 | [RAVE](./3dgs_2026-01.md#4-rave-rate-adaptive-visual-encoding-for-3d-gaussian-splatting) | 2512.07052 | 3D高斯溅射, 动态码率控制, 神经场景压缩, 免重训插值 |
| 2026-01-12 | [Mon3tr](./3dgs_2026-01.md#3-mon3tr-monocular-3d-telepresence-with-pre-built-gaussian-avatars-as-amortization) | 2601.07518 | 3D高斯溅射,单目驱动,数字人重建,低带宽传输,实时渲染 |
| 2026-01-12 | [Sketch&Patch++](./3dgs_2026-01.md#5-sketch-amp-patch-efficient-structure-aware-3d-gaussian-representation) | 2601.05394 | 3D高斯表示,分层渐进传输,密度聚类,结构感知编码 |
| 2026-01-07 | [SCAR-GS](./3dgs_2026-01.md#1-scar-gs-spatial-context-attention-for-residuals-in-progressive-gaussian-splatting) | 2601.04348 | 3D高斯溅射,渐进式压缩,残差矢量量化,自回归熵模型 |

**概要**: 本类论文涉及结构感知编码、单目驱动、低带宽传输、实时渲染、参数化人脸建模、3D高斯表示、密度聚类、动态码率控制等研究方向，共 5 篇。

---

## 十七、SLAM与建图 {#cat-slam}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-28 | [LangGS-SLAM](./3dgs_2026-01.md#1-langgs-slam-real-time-language-feature-gaussian-splatting-slam) | 2602.06991 | 高斯溅射,SLAM,语言对齐特征,Top-K渲染,混合场优化 |
| 2026-01-20 | [ParkingTwin](./3dgs_2026-01.md#4-parkingtwin-training-free-streaming-3d-reconstruction-for-parking-lot-digital-twins) | 2601.13706 | 流式三维重建,OSM先验建图,动态遮挡过滤,光照鲁棒融合 |
| 2026-01-18 | [SA-ResGS](./3dgs_2026-01.md#4-sa-resgs-self-augmented-residual-3d-gaussian-splatting-for-next-best-view-selection) | 2601.03024 | 3D高斯泼溅,残差学习,不确定性量化,视点选择,主动重建 |
| 2026-01-17 | [ActiveMapping](./3dgs_2026-01.md#1-active-semantic-mapping-of-horticultural-environments-using-gaussian-splatting) | 2601.12122 | 3D高斯泼溅,主动语义建图,移动机器人,Octomap,农业场景 |
| 2026-01-10 | [3DSceneRep](./3dgs_2026-01.md#1-what-is-the-best-3d-scene-representation-for-robotics-from-geometric-to-foundation-models) | 2512.03422 | 三维场景表示,机器人系统,神经表示,3D高斯泼溅,基础模型 |
| 2026-01-10 | [E2-BKI](./3dgs_2026-01.md#2-e2-bki-evidential-ellipsoidal-bayesian-kernel-inference-for-uncertainty-aware-gaussian-semantic-mapping) | 2509.11964 | 证据深度学习,贝叶斯核推理,高斯表示,不确定性感知,语义建图 |
| 2026-01-10 | [VPGS-SLAM](./3dgs_2026-01.md#3-vpgs-slam-voxel-based-progressive-3d-gaussian-slam-in-large-scale-scenes) | 2505.18992 | 3D高斯溅射,大规模SLAM,体素建图,子图融合,回环检测 |
| 2026-01-09 | [PointSLAM++](./3dgs_2026-01.md#1-pointslam-robust-dense-neural-gaussian-point-cloud-based-slam) | 2601.11617 | 神经高斯表示,渐进式位姿优化,动态节点分布,RGB-D SLAM,3D重建 |

**概要**: 本类论文涉及混合场优化、证据深度学习、OSM先验建图、不确定性感知、机器人系统、流式三维重建、Octomap、3D高斯泼溅等研究方向，共 8 篇。

---

## 十八、逆渲染与光照 {#cat-inverserender}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-28 | ★ **[HDR-4DGS](./3dgs_2026-01.md#5-dynamic-novel-view-synthesis-in-high-dynamic-range)** | 2509.21853 | 高斯泼溅,动态色调映射,高动态范围,新视角合成 ICLR'26 |
| 2026-01-26 | [HeadLighter](./3dgs_2026-01.md#5-headlighter-disentangling-illumination-in-generative-3d-gaussian-heads-via-lightstage-captures) | 2601.02103 | 3D高斯溅射,光照解耦,光棚捕获,可控重光照 |
| 2026-01-06 | [RelightAnyone](./3dgs_2026-01.md#1-relightanyone-a-generalized-relightable-3d-gaussian-head-model) | 2601.03357 | 3D高斯溅射,头部重建,重光照,两阶段学习,跨主体泛化 |
| 2026-01-04 | [DGSM](./3dgs_2026-01.md#2-animated-3dgs-avatars-in-diverse-scenes-with-consistent-lighting-and-shadows) | 2601.01660 | 3D高斯泼溅,深度高斯阴影贴图,实时光照,球谐函数,数字人重光照 |
| 2026-01-04 | [ShadowGS](./3dgs_2026-01.md#4-shadowgs-shadow-aware-3d-gaussian-splatting-for-satellite-imagery) | 2601.00939 | 3D高斯泼溅,阴影建模,卫星影像重建,物理渲染,新视角合成 |

**概要**: 本类论文涉及球谐函数、阴影建模、高动态范围、3D高斯泼溅、深度高斯阴影贴图、物理渲染、头部重建、新视角合成等研究方向，共 5 篇。

---

## 十九、凝聚态物理理论 {#cat-condensed-matter}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-01-02 | [Linear](./3dgs_2026-01.md#2-linear-magnetoresistance-of-two-dimensional-massless-dirac-fermions-in-the-quantum-limit) | 2512.13475 | 线性磁阻,二维狄拉克费米子,量子极限,自洽玻恩近似 |

**概要**: 本类论文涉及线性磁阻、二维狄拉克费米子、量子极限、自洽玻恩近似等研究方向，共 1 篇。

---

## 统计概览

| 类别 | 论文数 |
|------|--------|
| 几何与表面重建 | 59 |
| 视觉定位 | 1 |
| 核心算法与优化 | 46 |
| 安全与版权 | 1 |
| 无线与射频传播 | 3 |
| 风格迁移与编辑 | 9 |
| 语义分割与场景理解 | 16 |
| 领域应用 | 21 |
| 生成式模型 | 31 |
| 新视角合成 | 31 |
| 机器人仿真与具身智能 | 7 |
| 自动驾驶应用 | 7 |
| 数字人与人体重建 | 26 |
| 动态场景与4D | 19 |
| 渲染加速与压缩 | 20 |
| 流媒体与编码 | 5 |
| SLAM与建图 | 8 |
| 逆渲染与光照 | 5 |
| 凝聚态物理理论 | 1 |
| **合计** | **316** |
