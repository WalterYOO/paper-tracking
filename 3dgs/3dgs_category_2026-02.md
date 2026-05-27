# 3D Gaussian Splatting 论文跟踪 分类索引 (2026年2月)

> 基于 `3dgs_2026-02.md` 中收集的论文，按研究方向细分类。
> ★ 表示被顶会/顶刊录用。

## 目录

- [3D Gaussian Splatting 论文跟踪 分类索引 (2026年2月)](#3D Gaussian Splatting 论文跟踪-分类索引-2026年2月)
  - [目录](#目录)
  - [一、几何与表面重建](#cat-geo-recon)
  - [二、新视角合成](#cat-nvs)
  - [三、视觉定位](#cat-visloc)
  - [四、机器人仿真与具身智能](#cat-robotics)
  - [五、生成式模型](#cat-generative)
  - [六、自动驾驶应用](#cat-autodrive)
  - [七、渲染加速与压缩](#cat-render-accel)
  - [八、动态场景与4D](#cat-dynamic-4d)
  - [九、核心算法与优化](#cat-core-opt)
  - [十、SLAM与建图](#cat-slam)
  - [十一、风格迁移与编辑](#cat-style-edit)
  - [十二、语义分割与场景理解](#cat-seg-understand)
  - [十三、领域应用](#cat-domain-app)
  - [十四、数字人与人体重建](#cat-human)
  - [十五、安全与版权](#cat-security)
  - [十六、逆渲染与光照](#cat-inverserender)
  - [十七、无线与射频传播](#cat-rf)
  - [统计概览](#统计概览)

---

## 一、几何与表面重建 {#cat-geo-recon}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-28 | [TokenSplat](3dgs_2026-02.md#1-tokensplat-token-aligned-3d-gaussian-splatting-for-feed-forward-pose-free-reconstruction) | 2603.00697 | 3D高斯溅射,无位姿重建,相机位姿估计,前馈网络,Token对齐 |
| 2026-02-28 | ★ **[HorizonForge](3dgs_2026-02.md#3-horizonforge-driving-scene-editing-with-any-trajectories-and-any-vehicles)** | 2602.21333 | 高斯溅射,视频扩散,场景编辑,自动驾驶仿真,几何重建 CVPR'26 |
| 2026-02-28 | ★ **[PD2GS](3dgs_2026-02.md#5-pd-2-gs-part-level-decoupling-and-continuous-deformation-of-articulated-objects-via-gaussian-splatting)** | 2506.09663 | 高斯溅射,铰接物体,部件解耦,连续形变,运动学建模 ICLR'26 |
| 2026-02-27 | ★ **[Compact3DGS](3dgs_2026-02.md#1-prune-wisely-reconstruct-sharply-compact-3d-gaussian-splatting-via-adaptive-pruning-and-difference-of-gaussian-primitives)** | 2602.24136 | 3D高斯泼溅,自适应剪枝,高斯差分基元,模型压缩 CVPR'26 |
| 2026-02-27 | [SR3R](3dgs_2026-02.md#2-sr3r-rethinking-super-resolution-3d-reconstruction-with-feed-forward-gaussian-splatting) | 2602.24020 | 3D高斯溅射,超分辨率,前馈网络,稀疏视图重建,零样本泛化 |
| 2026-02-26 | ★ **[CrossSensorVS](3dgs_2026-02.md#1-no-calibration-no-depth-no-problem-cross-sensor-view-synthesis-with-3d-consistency)** | 2602.23559 | 跨模态新视角合成,3D高斯泼溅,免标定对齐,RGB-X融合,点云稠密化 CVPR'26 |
| 2026-02-26 | [Sapling-NeRF](3dgs_2026-02.md#3-sapling-nerf-geo-localised-sapling-reconstruction-in-forests-for-ecological-monitoring) | 2602.22731 | NeRF,激光SLAM,GNSS定位,三维重建,生态监测 |
| 2026-02-26 | ★ **[One2Scene](3dgs_2026-02.md#4-one2scene-geometric-consistent-explorable-3d-scene-generation-from-a-single-image)** | 2602.19766 | 单图3D生成,高斯溅射,几何骨架,新视角合成,跨视图一致性 ICLR'26 |
| 2026-02-26 | ★ **[USplat4D](3dgs_2026-02.md#5-uncertainty-matters-in-dynamic-gaussian-splatting-for-monocular-4d-reconstruction)** | 2510.12768 | 动态高斯溅射,不确定性估计,时空图优化,单目4D重建 ICLR'26 |
| 2026-02-26 | ★ **[G4Splat](3dgs_2026-02.md#6-g4splat-geometry-guided-gaussian-splatting-with-generative-prior)** | 2510.12099 | 高斯溅射, 扩散模型先验, 几何引导, 深度估计, 场景重建 ICLR'26 |
| 2026-02-26 | [SplatSDF](3dgs_2026-02.md#9-splatsdf-boosting-sdf-nerf-via-architecture-level-fusion-with-gaussian-splats) | 2411.15468 | SDF-NeRF,3D高斯泼溅,架构级融合,梯度加速,几何重建 |
| 2026-02-25 | [GIFSplat](3dgs_2026-02.md#2-gifsplat-generative-prior-guided-iterative-feed-forward-3d-gaussian-splatting-from-sparse-views) | 2602.22571 | 3D高斯溅射, 前向迭代优化, 扩散先验蒸馏, 稀疏视角重建 |
| 2026-02-25 | [SwiftNDC](3dgs_2026-02.md#3-swiftndc-fast-neural-depth-correction-for-high-fidelity-3d-reconstruction) | 2602.22565 | 神经深度校正,3D高斯溅射,几何初始化,网格重建,新视角合成 |
| 2026-02-25 | [DGGS](3dgs_2026-02.md#4-distractor-free-generalizable-3d-gaussian-splatting) | 2411.17605 | 3D高斯溅射,可泛化重建,干扰掩码预测,两阶段推理剪枝 |
| 2026-02-24 | ★ **[DropAnSH-GS](3dgs_2026-02.md#2-dropping-anchor-and-spherical-harmonics-for-sparse-view-gaussian-splatting)** | 2602.20933 | 高斯泼溅,稀疏视角重建,锚点丢弃,球谐函数,模型压缩 CVPR'26 |
| 2026-02-24 | [Monocular](3dgs_2026-02.md#4-monocular-endoscopic-tissue-3d-reconstruction-with-multi-level-geometry-regularization) | 2602.20718 | 3D高斯泼溅,符号距离场,形变正则化,内窥镜重建,表面约束 |
| 2026-02-24 | [WildGHand](3dgs_2026-02.md#5-wildghand-learning-anti-perturbation-gaussian-hand-avatars-from-monocular-in-the-wild-videos) | 2602.20556 | 3D高斯溅射,手部重建,扰动解耦,野外视频,优化策略 |
| 2026-02-24 | [CuriGS](3dgs_2026-02.md#6-curigs-curriculum-guided-gaussian-splatting-for-sparse-view-synthesis) | 2511.16030 | 3D高斯溅射,稀疏视角合成,课程学习,伪视图生成,几何一致性 |
| 2026-02-24 | ★ **[UPNet](3dgs_2026-02.md#7-peering-into-the-unknown-active-view-selection-with-neural-uncertainty-maps-for-3d-reconstruction)** | 2506.14856 | 主动视角选择,神经不确定性图,3D重建,新视角合成 ICLR'26 |
| 2026-02-23 | [Large-scale](3dgs_2026-02.md#2-large-scale-photorealistic-outdoor-3d-scene-reconstruction-from-uav-imagery-using-gaussian-splatting-techniques) | 2602.20342 | 3D高斯泼溅,无人机三维重建,实时渲染,位姿估计,低延迟管线 |
| 2026-02-23 | ★ **[AugRF](3dgs_2026-02.md#3-augmented-radiance-field-a-general-framework-for-enhanced-gaussian-splatting)** | 2602.19916 | 3D高斯泼溅,增强高斯核,镜面反射建模,误差补偿,辐射场重建 ICLR'26 |
| 2026-02-23 | ★ **[RAP](3dgs_2026-02.md#4-rap-fast-feedforward-rendering-free-attribute-guided-primitive-importance-score-prediction-for-efficient-3d-gaussian-splatting-processing)** | 2602.19753 | 3D高斯泼溅,基元重要性预测,免渲染网络,属性引导,模型压缩 CVPR'26 |
| 2026-02-23 | ★ **[OnlineSCD](3dgs_2026-02.md#5-changes-in-real-time-online-scene-change-detection-with-multi-view-fusion)** | 2511.12370 | 在线场景变化检测, 3D高斯溅射, 多视图融合, 自监督学习, 实时姿态估计 CVPR'26 |
| 2026-02-23 | [MOGS](3dgs_2026-02.md#6-mogs-monocular-object-guided-gaussian-splatting-in-large-scenes) | 2509.06685 | 3D高斯溅射,单目重建,语义形状先验,视觉惯性SfM,深度优化 |
| 2026-02-22 | [DefenseSplat](3dgs_2026-02.md#1-defensesplat-enhancing-the-robustness-of-3d-gaussian-splatting-via-frequency-aware-filtering) | 2602.19323 | 3D高斯泼溅, 对抗防御, 频率感知滤波, 小波变换, 鲁棒性 |
| 2026-02-20 | [Diff2DGS](3dgs_2026-02.md#2-diff2dgs-reliable-reconstruction-of-occluded-surgical-scenes-via-2d-gaussian-splatting) | 2602.18314 | 2D高斯溅射,扩散模型,遮挡修复,动态形变,手术场景重建 |
| 2026-02-20 | ★ **[UrbanGS](3dgs_2026-02.md#3-urbangs-a-scalable-and-efficient-architecture-for-geometrically-accurate-large-scene-reconstruction)** | 2602.02089 | 3D高斯溅射,深度法线正则化,自适应剪枝,城市场景重建 ICLR'26 |
| 2026-02-19 | [Local-EndoGS](3dgs_2026-02.md#1-4d-monocular-surgical-reconstruction-under-arbitrary-camera-motions) | 2602.17473 | 单目内窥镜,4D重建,3D高斯溅射,可变形场景,窗口化表示 |
| 2026-02-19 | [MultimodalGS](3dgs_2026-02.md#4-3d-scene-rendering-with-multimodal-gaussian-splatting) | 2602.17124 | 高斯溅射,射频传感,多模态融合,3D场景渲染,深度预测 |
| 2026-02-17 | [SemanticGS](3dgs_2026-02.md#1-semantic-guided-3d-gaussian-splatting-for-transient-object-removal) | 2602.15516 | 3D高斯溅射,瞬态物体去除,语义引导,CLIP评分,高斯剪枝 |
| 2026-02-17 | [DARB-Splatting](3dgs_2026-02.md#3-darb-splatting-generalizing-splatting-with-decaying-anisotropic-radial-basis-functions) | 2501.12369 | 3D高斯泼溅, 径向基函数, 重建核, 新视角合成, 3D重建 |
| 2026-02-16 | [Wrivinder](3dgs_2026-02.md#2-wrivinder-towards-spatial-intelligence-for-geo-locating-ground-images-onto-satellite-imagery) | 2602.14929 | 3D高斯泼溅,跨视角对齐,地理定位,零样本框架,场景重建 |
| 2026-02-16 | [GMR](3dgs_2026-02.md#3-gaussian-mesh-renderer-for-lightweight-differentiable-rendering) | 2602.14493 | 可微渲染,3D高斯溅射,网格重建,梯度优化,轻量级渲染 |
| 2026-02-16 | [DigitalTwin](3dgs_2026-02.md#5-digital-twin-generation-from-visual-data-a-survey) | 2504.13159 | 数字孪生,3D高斯泼溅,基础模型,语义分割,视觉重建 |
| 2026-02-14 | [Planetary3D](3dgs_2026-02.md#1-high-fidelity-3d-reconstruction-for-planetary-exploration) | 2602.13909 | 神经辐射场, 高斯溅射, 三维重建, 行星探测, 机器人建图 |
| 2026-02-14 | [DiWR](3dgs_2026-02.md#2-joint-orientation-and-weight-optimization-for-robust-watertight-surface-reconstruction-via-dirichlet-regularized-winding-fields) | 2602.13801 | 水密表面重建,绕数场,联合优化,法向估计,Dirichlet正则化 |
| 2026-02-13 | [PBR-GS](3dgs_2026-02.md#1-nighttime-autonomous-driving-scene-reconstruction-with-physically-based-gaussian-splatting) | 2602.13549 | 3D高斯溅射,物理渲染,BRDF材质优化,夜间场景重建 |
| 2026-02-13 | [GSM-GS](3dgs_2026-02.md#3-gsm-gs-geometry-constrained-single-and-multi-view-gaussian-splatting-for-surface-reconstruction) | 2602.12796 | 3D高斯溅射,几何约束,表面重建,自适应加权,多视图一致性 |
| 2026-02-12 | [TG-Field](3dgs_2026-02.md#3-tg-field-geometry-aware-radiative-gaussian-fields-for-tomographic-reconstruction) | 2602.11705 | 3D高斯泼溅,几何感知形变,稀疏CT重建,动态场景建模,时空注意力 |
| 2026-02-12 | ★ **[NGFF](3dgs_2026-02.md#5-learning-physics-grounded-4d-dynamics-with-neural-gaussian-force-fields)** | 2602.00148 | 神经高斯力场,物理驱动建模,4D视频生成,3D高斯溅射,世界模型 ICLR'26 |
| 2026-02-12 | [EDGS](3dgs_2026-02.md#7-edgs-eliminating-densification-for-efficient-convergence-of-3dgs) | 2504.13204 | 3D高斯泼溅,密集初始化,密度增长消除,快速收敛,几何重建 |
| 2026-02-12 | [NeRF](3dgs_2026-02.md#8-nerf-neural-radiance-field-in-3d-vision-a-comprehensive-review-updated-post-gaussian-splatting) | 2210.00379 | 神经辐射场,隐式神经场,高斯泼溅,新视角合成,可微渲染 |
| 2026-02-11 | [LeafFit](3dgs_2026-02.md#1-leaffit-plant-assets-creation-from-3d-gaussian-splatting) | 2602.11577 | 3D高斯溅射,网格重建,可微形变,实例化资产,顶点着色器 |
| 2026-02-11 | ★ **[SplatDistill](3dgs_2026-02.md#2-splat-and-distill-augmenting-teachers-with-feed-forward-3d-reconstruction-for-3d-aware-distillation)** | 2602.06032 | 3D高斯表示,知识蒸馏,前馈重建,3D感知,视觉基础模型 ICLR'26 |
| 2026-02-11 | [LighthouseGS](3dgs_2026-02.md#3-lighthousegs-indoor-structure-aware-3d-gaussian-splatting-for-panorama-style-mobile-captures) | 2507.06109 | 3D高斯溅射,平面结构先验,几何与光度校正,新视角合成,移动端全景 |
| 2026-02-10 | [ERGO](3dgs_2026-02.md#1-ergo-excess-risk-guided-optimization-for-high-fidelity-monocular-3d-gaussian-splatting) | 2602.10278 | 单目3D重建, 高斯溅射, 超额风险分解, 自适应优化 |
| 2026-02-10 | [Faster-GS](3dgs_2026-02.md#4-faster-gs-analyzing-and-improving-gaussian-splatting-optimization) | 2602.09999 | 3D高斯泼溅,训练加速,梯度近似,数值稳定性,4D重建 |
| 2026-02-10 | [CompSplat](3dgs_2026-02.md#5-compsplat-compression-aware-3d-gaussian-splatting-for-real-world-video) | 2602.09816 | 3D高斯溅射,新视角合成,压缩感知,自适应剪枝,几何一致性 |
| 2026-02-09 | [Converged3DGS](3dgs_2026-02.md#1-analysis-of-converged-3d-gaussian-splatting-solutions-density-effects-and-prediction-limit) | 2602.08909 | 3D高斯溅射,密度分层,参数预测,渲染优化,可见性分析 |
| 2026-02-08 | ★ **[Informative](3dgs_2026-02.md#1-informative-object-centric-next-best-view-for-object-aware-3d-gaussian-splatting-in-cluttered-scenes)** | 2602.08266 | 3D高斯泼溅,下一最佳视点,实例感知,主动视点规划,杂乱场景重建 ICRA'26 |
| 2026-02-08 | [ThermoSplat](3dgs_2026-02.md#2-thermosplat-cross-modal-3d-gaussian-splatting-with-feature-modulation-and-geometry-decoupling) | 2601.15897 | 3D高斯溅射,跨模态重建,特征调制,几何解耦,热红外感知 |
| 2026-02-08 | [Color3D](3dgs_2026-02.md#4-color3d-controllable-and-consistent-3d-colorization-with-personalized-colorizer) | 2510.10152 | 个性化色彩化, 高斯溅射, 跨视角一致性, 动态3D重建, 单视图引导 |
| 2026-02-05 | [XSIM](3dgs_2026-02.md#2-unified-sensor-simulation-for-autonomous-driving) | 2602.05617 | 3D高斯溅射, 传感器仿真, 卷帘快门建模, 相位建模, 自动驾驶 |
| 2026-02-05 | [Mini-Splatting2](3dgs_2026-02.md#3-efficient-scene-modeling-via-structure-aware-and-region-prioritized-3d-gaussians) | 2411.12788 | 3D高斯溅射,结构感知分布,区域优先优化,几何正则化,高效建模 |
| 2026-02-05 | [MVGS](3dgs_2026-02.md#4-mvgs-multi-view-regulated-gaussian-splatting-for-novel-view-synthesis) | 2410.02103 | 3D高斯泼溅, 多视图训练, 跨射线密集化, 新视角合成, 几何重建 |
| 2026-02-04 | [JOintGS](3dgs_2026-02.md#3-jointgs-joint-optimization-of-cameras-bodies-and-3d-gaussians-for-in-the-wild-monocular-reconstruction) | 2602.04317 | 3D高斯溅射,联合优化,人体重建,相机标定,前景背景解耦 |
| 2026-02-04 | [3DGS-SLAM](3dgs_2026-02.md#4-towards-next-generation-slam-a-survey-on-3dgs-slam-focusing-on-performance-robustness-and-future-directions) | 2602.04251 | 3D高斯泼溅,SLAM,性能优化,动态鲁棒性,系统综述 |
| 2026-02-03 | [AnyStyle](3dgs_2026-02.md#1-anystyle-single-pass-multimodal-stylization-for-3d-gaussian-splatting) | 2602.04043 | 3D高斯泼溅,风格迁移,多模态条件,前馈重建,零样本 |
| 2026-02-03 | [Pi-GS](3dgs_2026-02.md#2-pi-gs-sparse-view-gaussian-splatting-with-dense-3-initialization) | 2602.03327 | 3D高斯泼溅,稀疏视角,点云初始化,几何正则化,新视角合成 |
| 2026-02-03 | ★ **[SurfSplat](3dgs_2026-02.md#3-surfsplat-conquering-feedforward-2d-gaussian-splatting-with-surface-continuity-priors)** | 2602.02000 | 2D高斯泼溅,表面连续性先验,前馈三维重建,高分辨率渲染 ICLR'26 |
| 2026-02-03 | [MaterialGS](3dgs_2026-02.md#4-material-informed-gaussian-splatting-for-3d-world-reconstruction-in-a-digital-twin) | 2511.20348 | 3D高斯溅射,材质感知,数字孪生,传感器仿真,纯相机重建 |
| 2026-02-02 | [TVGS](3dgs_2026-02.md#4-from-slices-to-structures-unsupervised-3d-reconstruction-of-female-pelvic-anatomy-from-freehand-transvaginal-ultrasound) | 2508.14552 | 高斯泼溅,无监督三维重建,超声成像,联合位姿优化,可微光栅化 |
| 2026-02-02 | [Feat2GS](3dgs_2026-02.md#5-feat2gs-probing-visual-foundation-models-with-gaussian-splatting) | 2412.09606 | 3D高斯溅射,视觉基础模型,新视角合成,三维感知评估 |
| 2026-02-02 | [HI-SLAM2](3dgs_2026-02.md#6-hi-slam2-geometry-aware-gaussian-slam-for-fast-monocular-scene-reconstruction) | 2411.17982 | 3D高斯溅射,单目SLAM,几何感知,稠密重建,尺度对齐 |
| 2026-02-01 | [Split&Splat](3dgs_2026-02.md#1-split-amp-splat-zero-shot-panoptic-segmentation-via-explicit-instance-modeling-and-3d-gaussian-splatting) | 2602.03809 | 3D高斯溅射,全景分割,实例建模,场景重建 |
| 2026-02-01 | [Radioactive](3dgs_2026-02.md#3-radioactive-3d-gaussian-ray-tracing-for-tomographic-reconstruction) | 2602.01057 | 3D高斯溅射,光线追踪,断层重建,解析线积分,几何校正 |

**概要**: 本类论文涉及绕数场、法向估计、个性化色彩化、跨视角一致性、单目4D重建、动态形变、运动学建模、系统综述等研究方向，共 66 篇。

---

## 二、新视角合成 {#cat-nvs}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-28 | [TokenSplat](3dgs_2026-02.md#1-tokensplat-token-aligned-3d-gaussian-splatting-for-feed-forward-pose-free-reconstruction) | 2603.00697 | 3D高斯溅射,无位姿重建,相机位姿估计,前馈网络,Token对齐 |
| 2026-02-28 | [SplatNet](3dgs_2026-02.md#4-splat-the-net-radiance-fields-with-splattable-neural-primitives) | 2510.08491 | 神经基元,辐射场,高斯泼溅,免射线步进渲染,新视角合成 |
| 2026-02-27 | ★ **[MEGS2](3dgs_2026-02.md#5-megs-2-memory-efficient-gaussian-splatting-via-spherical-gaussians-and-unified-pruning)** | 2509.07021 | 3D高斯溅射,显存压缩,球面高斯瓣,统一软剪枝 ICLR'26 |
| 2026-02-26 | ★ **[CrossSensorVS](3dgs_2026-02.md#1-no-calibration-no-depth-no-problem-cross-sensor-view-synthesis-with-3d-consistency)** | 2602.23559 | 跨模态新视角合成,3D高斯泼溅,免标定对齐,RGB-X融合,点云稠密化 CVPR'26 |
| 2026-02-26 | ★ **[One2Scene](3dgs_2026-02.md#4-one2scene-geometric-consistent-explorable-3d-scene-generation-from-a-single-image)** | 2602.19766 | 单图3D生成,高斯溅射,几何骨架,新视角合成,跨视图一致性 ICLR'26 |
| 2026-02-26 | ★ **[G4Splat](3dgs_2026-02.md#6-g4splat-geometry-guided-gaussian-splatting-with-generative-prior)** | 2510.12099 | 高斯溅射, 扩散模型先验, 几何引导, 深度估计, 场景重建 ICLR'26 |
| 2026-02-26 | ★ **[UBS](3dgs_2026-02.md#7-universal-beta-splatting)** | 2510.03312 | Beta核,高斯溅射,辐射场渲染,实时渲染,各向异性建模 ICLR'26 |
| 2026-02-25 | [BetterScene](3dgs_2026-02.md#1-betterscene-3d-scene-synthesis-with-representation-aligned-generative-model) | 2602.22596 | 新视角合成, 扩散模型, 3D高斯溅射, 表示对齐 |
| 2026-02-25 | [GIFSplat](3dgs_2026-02.md#2-gifsplat-generative-prior-guided-iterative-feed-forward-3d-gaussian-splatting-from-sparse-views) | 2602.22571 | 3D高斯溅射, 前向迭代优化, 扩散先验蒸馏, 稀疏视角重建 |
| 2026-02-25 | [SwiftNDC](3dgs_2026-02.md#3-swiftndc-fast-neural-depth-correction-for-high-fidelity-3d-reconstruction) | 2602.22565 | 神经深度校正,3D高斯溅射,几何初始化,网格重建,新视角合成 |
| 2026-02-24 | [CuriGS](3dgs_2026-02.md#6-curigs-curriculum-guided-gaussian-splatting-for-sparse-view-synthesis) | 2511.16030 | 3D高斯溅射,稀疏视角合成,课程学习,伪视图生成,几何一致性 |
| 2026-02-24 | ★ **[UPNet](3dgs_2026-02.md#7-peering-into-the-unknown-active-view-selection-with-neural-uncertainty-maps-for-3d-reconstruction)** | 2506.14856 | 主动视角选择,神经不确定性图,3D重建,新视角合成 ICLR'26 |
| 2026-02-23 | [AestheticField](3dgs_2026-02.md#1-aesthetic-camera-viewpoint-suggestion-with-3d-aesthetic-field) | 2602.20363 | 3D美学场,3D高斯溅射,视角推荐,知识蒸馏,梯度优化 |
| 2026-02-23 | ★ **[AugRF](3dgs_2026-02.md#3-augmented-radiance-field-a-general-framework-for-enhanced-gaussian-splatting)** | 2602.19916 | 3D高斯泼溅,增强高斯核,镜面反射建模,误差补偿,辐射场重建 ICLR'26 |
| 2026-02-20 | ★ **[Luminance-GS++](3dgs_2026-02.md#1-unifying-color-and-lightness-correction-with-view-adaptive-curve-adjustment-for-robust-3d-novel-view-synthesis)** | 2602.18322 | 3D高斯溅射,新视角合成,亮度校正,视角自适应,光度一致性 CVPR'25 |
| 2026-02-19 | [MultimodalGS](3dgs_2026-02.md#4-3d-scene-rendering-with-multimodal-gaussian-splatting) | 2602.17124 | 高斯溅射,射频传感,多模态融合,3D场景渲染,深度预测 |
| 2026-02-17 | [SemanticGS](3dgs_2026-02.md#1-semantic-guided-3d-gaussian-splatting-for-transient-object-removal) | 2602.15516 | 3D高斯溅射,瞬态物体去除,语义引导,CLIP评分,高斯剪枝 |
| 2026-02-17 | [DARB-Splatting](3dgs_2026-02.md#3-darb-splatting-generalizing-splatting-with-decaying-anisotropic-radial-basis-functions) | 2501.12369 | 3D高斯泼溅, 径向基函数, 重建核, 新视角合成, 3D重建 |
| 2026-02-16 | [TimeArchival](3dgs_2026-02.md#1-time-archival-camera-virtualization-for-sports-and-visual-performances) | 2602.15181 | 相机虚拟化,神经体积渲染,动态场景,时间归档,新视角合成 |
| 2026-02-16 | [MS-Splatting](3dgs_2026-02.md#4-multi-spectral-gaussian-splatting-with-neural-color-representation) | 2506.03407 | 多光谱渲染, 3D高斯溅射, 神经色彩表示, 联合特征编码 |
| 2026-02-12 | [NeRF](3dgs_2026-02.md#8-nerf-neural-radiance-field-in-3d-vision-a-comprehensive-review-updated-post-gaussian-splatting) | 2210.00379 | 神经辐射场,隐式神经场,高斯泼溅,新视角合成,可微渲染 |
| 2026-02-11 | [LighthouseGS](3dgs_2026-02.md#3-lighthousegs-indoor-structure-aware-3d-gaussian-splatting-for-panorama-style-mobile-captures) | 2507.06109 | 3D高斯溅射,平面结构先验,几何与光度校正,新视角合成,移动端全景 |
| 2026-02-10 | [CompSplat](3dgs_2026-02.md#5-compsplat-compression-aware-3d-gaussian-splatting-for-real-world-video) | 2602.09816 | 3D高斯溅射,新视角合成,压缩感知,自适应剪枝,几何一致性 |
| 2026-02-08 | [Color3D](3dgs_2026-02.md#4-color3d-controllable-and-consistent-3d-colorization-with-personalized-colorizer) | 2510.10152 | 个性化色彩化, 高斯溅射, 跨视角一致性, 动态3D重建, 单视图引导 |
| 2026-02-05 | [MVGS](3dgs_2026-02.md#4-mvgs-multi-view-regulated-gaussian-splatting-for-novel-view-synthesis) | 2410.02103 | 3D高斯泼溅, 多视图训练, 跨射线密集化, 新视角合成, 几何重建 |
| 2026-02-04 | [PoseGaussian](3dgs_2026-02.md#1-posegaussian-pose-driven-novel-view-synthesis-for-robust-3d-human-reconstruction) | 2602.05190 | 高斯溅射, 姿态引导, 新视角合成, 人体重建, 实时渲染 |
| 2026-02-04 | [QuantumGS](3dgs_2026-02.md#2-quantumgs-quantum-encoding-framework-for-gaussian-splatting) | 2602.05047 | 3D高斯泼溅,变分量子电路,布洛赫球编码,视角相关渲染 |
| 2026-02-03 | [Pi-GS](3dgs_2026-02.md#2-pi-gs-sparse-view-gaussian-splatting-with-dense-3-initialization) | 2602.03327 | 3D高斯泼溅,稀疏视角,点云初始化,几何正则化,新视角合成 |
| 2026-02-03 | ★ **[SurfSplat](3dgs_2026-02.md#3-surfsplat-conquering-feedforward-2d-gaussian-splatting-with-surface-continuity-priors)** | 2602.02000 | 2D高斯泼溅,表面连续性先验,前馈三维重建,高分辨率渲染 ICLR'26 |
| 2026-02-02 | [Feat2GS](3dgs_2026-02.md#5-feat2gs-probing-visual-foundation-models-with-gaussian-splatting) | 2412.09606 | 3D高斯溅射,视觉基础模型,新视角合成,三维感知评估 |

**概要**: 本类论文涉及个性化色彩化、联合特征编码、跨视角一致性、人体重建、网格重建、多光谱渲染、扩散模型、2D高斯泼溅等研究方向，共 30 篇。

---

## 三、视觉定位 {#cat-visloc}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-28 | [TokenSplat](3dgs_2026-02.md#1-tokensplat-token-aligned-3d-gaussian-splatting-for-feed-forward-pose-free-reconstruction) | 2603.00697 | 3D高斯溅射,无位姿重建,相机位姿估计,前馈网络,Token对齐 |
| 2026-02-16 | [Wrivinder](3dgs_2026-02.md#2-wrivinder-towards-spatial-intelligence-for-geo-locating-ground-images-onto-satellite-imagery) | 2602.14929 | 3D高斯泼溅,跨视角对齐,地理定位,零样本框架,场景重建 |

**概要**: 本类论文涉及地理定位、前馈网络、场景重建、Token对齐、3D高斯溅射、跨视角对齐、相机位姿估计、3D高斯泼溅等研究方向，共 2 篇。

---

## 四、机器人仿真与具身智能 {#cat-robotics}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-28 | [RobMRAG](3dgs_2026-02.md#2-zero-shot-robotic-manipulation-via-3d-gaussian-splatting-enhanced-multimodal-retrieval-augmented-generation) | 2603.00500 | 3D高斯泼溅,检索增强生成,零样本操作,多模态大模型,姿态优化 |
| 2026-02-28 | ★ **[PD2GS](3dgs_2026-02.md#5-pd-2-gs-part-level-decoupling-and-continuous-deformation-of-articulated-objects-via-gaussian-splatting)** | 2506.09663 | 高斯溅射,铰接物体,部件解耦,连续形变,运动学建模 ICLR'26 |
| 2026-02-26 | [SplatSDF](3dgs_2026-02.md#9-splatsdf-boosting-sdf-nerf-via-architecture-level-fusion-with-gaussian-splats) | 2411.15468 | SDF-NeRF,3D高斯泼溅,架构级融合,梯度加速,几何重建 |
| 2026-02-17 | [Relightable3DGS](3dgs_2026-02.md#2-zero-shot-uav-navigation-in-forests-via-relightable-3d-gaussian-splatting) | 2602.07101 | 3D高斯溅射,可重光照,强化学习,零样本迁移,无人机导航 |
| 2026-02-14 | [ReaDy-Go](3dgs_2026-02.md#3-ready-go-real-to-sim-dynamic-3d-gaussian-splatting-simulation-for-environment-specific-visual-navigation-with-moving-obstacles) | 2602.11575 | 3D高斯溅射,虚实迁移仿真,动态场景,视觉导航,移动障碍物 |
| 2026-02-13 | [FlowHOI](3dgs_2026-02.md#2-flowhoi-flow-based-semantics-grounded-generation-of-hand-object-interactions-for-dexterous-robot-manipulation) | 2602.13444 | 流匹配,手物交互生成,语义对齐,具身操作,3D高斯重建 |
| 2026-02-12 | [LatentAM](3dgs_2026-02.md#1-latentam-real-time-large-scale-latent-gaussian-attention-mapping-via-online-dictionary-learning) | 2602.12314 | 3D高斯溅射,在线字典学习,开放词汇感知,机器人建图,特征映射 |
| 2026-02-12 | [3DGSNav](3dgs_2026-02.md#2-3dgsnav-enhancing-vision-language-model-reasoning-for-object-navigation-via-active-3d-gaussian-splatting) | 2602.12159 | 3D高斯泼溅,视觉语言模型,主动感知,物体导航,思维链 |
| 2026-02-08 | ★ **[Informative](3dgs_2026-02.md#1-informative-object-centric-next-best-view-for-object-aware-3d-gaussian-splatting-in-cluttered-scenes)** | 2602.08266 | 3D高斯泼溅,下一最佳视点,实例感知,主动视点规划,杂乱场景重建 ICRA'26 |
| 2026-02-02 | [SoMA](3dgs_2026-02.md#2-soma-a-real-to-sim-neural-simulator-for-robotic-soft-body-manipulation) | 2602.02402 | 3D高斯泼溅,神经模拟器,软体操作,真实到仿真 |

**概要**: 本类论文涉及3D高斯重建、SDF-NeRF、思维链、强化学习、运动学建模、零样本操作、视觉语言模型、主动感知等研究方向，共 10 篇。

---

## 五、生成式模型 {#cat-generative}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-28 | [RobMRAG](3dgs_2026-02.md#2-zero-shot-robotic-manipulation-via-3d-gaussian-splatting-enhanced-multimodal-retrieval-augmented-generation) | 2603.00500 | 3D高斯泼溅,检索增强生成,零样本操作,多模态大模型,姿态优化 |
| 2026-02-28 | ★ **[HorizonForge](3dgs_2026-02.md#3-horizonforge-driving-scene-editing-with-any-trajectories-and-any-vehicles)** | 2602.21333 | 高斯溅射,视频扩散,场景编辑,自动驾驶仿真,几何重建 CVPR'26 |
| 2026-02-27 | ★ **[Stylos](3dgs_2026-02.md#4-stylos-multi-view-3d-stylization-with-single-forward-gaussian-splatting)** | 2509.26455 | 3D高斯溅射,风格迁移,单次前向传播,双路径架构,零样本生成 ICLR'26 |
| 2026-02-26 | ★ **[One2Scene](3dgs_2026-02.md#4-one2scene-geometric-consistent-explorable-3d-scene-generation-from-a-single-image)** | 2602.19766 | 单图3D生成,高斯溅射,几何骨架,新视角合成,跨视图一致性 ICLR'26 |
| 2026-02-26 | ★ **[G4Splat](3dgs_2026-02.md#6-g4splat-geometry-guided-gaussian-splatting-with-generative-prior)** | 2510.12099 | 高斯溅射, 扩散模型先验, 几何引导, 深度估计, 场景重建 ICLR'26 |
| 2026-02-25 | [BetterScene](3dgs_2026-02.md#1-betterscene-3d-scene-synthesis-with-representation-aligned-generative-model) | 2602.22596 | 新视角合成, 扩散模型, 3D高斯溅射, 表示对齐 |
| 2026-02-25 | [GIFSplat](3dgs_2026-02.md#2-gifsplat-generative-prior-guided-iterative-feed-forward-3d-gaussian-splatting-from-sparse-views) | 2602.22571 | 3D高斯溅射, 前向迭代优化, 扩散先验蒸馏, 稀疏视角重建 |
| 2026-02-16 | [DigitalTwin](3dgs_2026-02.md#5-digital-twin-generation-from-visual-data-a-survey) | 2504.13159 | 数字孪生,3D高斯泼溅,基础模型,语义分割,视觉重建 |
| 2026-02-13 | [FlowHOI](3dgs_2026-02.md#2-flowhoi-flow-based-semantics-grounded-generation-of-hand-object-interactions-for-dexterous-robot-manipulation) | 2602.13444 | 流匹配,手物交互生成,语义对齐,具身操作,3D高斯重建 |
| 2026-02-12 | [OMEGA-Avatar](3dgs_2026-02.md#4-omega-avatar-one-shot-modeling-of-360-gaussian-avatars) | 2602.11693 | 单图重建,3D高斯溅射,数字人生成,前向网络,网格变形 |
| 2026-02-12 | ★ **[NGFF](3dgs_2026-02.md#5-learning-physics-grounded-4d-dynamics-with-neural-gaussian-force-fields)** | 2602.00148 | 神经高斯力场,物理驱动建模,4D视频生成,3D高斯溅射,世界模型 ICLR'26 |
| 2026-02-10 | [FG-3DGS](3dgs_2026-02.md#6-toward-fine-grained-facial-control-in-3d-talking-head-generation) | 2602.09736 | 3D高斯泼溅,频率感知解耦,数字人生成,唇形同步 |
| 2026-02-05 | [SuperHead](3dgs_2026-02.md#1-from-blurry-to-believable-enhancing-low-quality-talking-heads-with-3d-generative-priors) | 2602.06122 | 3D高斯溅射,生成先验反演,数字人重建,动态超分辨率 |
| 2026-02-04 | [StyleMe3D](3dgs_2026-02.md#5-styleme3d-stylization-with-disentangled-priors-by-multiple-encoders-on-3d-gaussians) | 2504.15281 | 3D高斯溅射,风格迁移,扩散模型蒸馏,CLIP对齐,几何保真 |

**概要**: 本类论文涉及3D高斯重建、视觉重建、零样本生成、风格迁移、场景重建、稀疏视角重建、零样本操作、扩散先验蒸馏等研究方向，共 14 篇。

---

## 六、自动驾驶应用 {#cat-autodrive}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-28 | ★ **[HorizonForge](3dgs_2026-02.md#3-horizonforge-driving-scene-editing-with-any-trajectories-and-any-vehicles)** | 2602.21333 | 高斯溅射,视频扩散,场景编辑,自动驾驶仿真,几何重建 CVPR'26 |
| 2026-02-26 | [LaGS](3dgs_2026-02.md#2-latent-gaussian-splatting-for-4d-panoptic-occupancy-tracking) | 2602.23172 | 潜在高斯溅射,4D占据网格,全景分割,动态场景跟踪,多视图聚合 |
| 2026-02-26 | ★ **[ST-GS](3dgs_2026-02.md#8-st-gs-vision-based-3d-semantic-occupancy-prediction-with-spatial-temporal-gaussian-splatting)** | 2509.16552 | 3D占用预测, 高斯溅射, 时空建模, 注意力机制, 自动驾驶 ICRA'26 |
| 2026-02-23 | [MOGS](3dgs_2026-02.md#6-mogs-monocular-object-guided-gaussian-splatting-in-large-scenes) | 2509.06685 | 3D高斯溅射,单目重建,语义形状先验,视觉惯性SfM,深度优化 |
| 2026-02-13 | [PBR-GS](3dgs_2026-02.md#1-nighttime-autonomous-driving-scene-reconstruction-with-physically-based-gaussian-splatting) | 2602.13549 | 3D高斯溅射,物理渲染,BRDF材质优化,夜间场景重建 |
| 2026-02-12 | ★ **[ArmGS](3dgs_2026-02.md#6-armgs-composite-gaussian-appearance-refinement-for-modeling-dynamic-urban-environments)** | 2507.03886 | 3D高斯泼溅, 多粒度外观优化, 动态城市场景, 自动驾驶仿真 ICRA'26 |
| 2026-02-05 | [XSIM](3dgs_2026-02.md#2-unified-sensor-simulation-for-autonomous-driving) | 2602.05617 | 3D高斯溅射, 传感器仿真, 卷帘快门建模, 相位建模, 自动驾驶 |
| 2026-02-03 | [MaterialGS](3dgs_2026-02.md#4-material-informed-gaussian-splatting-for-3d-world-reconstruction-in-a-digital-twin) | 2511.20348 | 3D高斯溅射,材质感知,数字孪生,传感器仿真,纯相机重建 |

**概要**: 本类论文涉及数字孪生、多粒度外观优化、相位建模、BRDF材质优化、3D高斯泼溅、4D占据网格、卷帘快门建模、注意力机制等研究方向，共 8 篇。

---

## 七、渲染加速与压缩 {#cat-render-accel}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-28 | [SplatNet](3dgs_2026-02.md#4-splat-the-net-radiance-fields-with-splattable-neural-primitives) | 2510.08491 | 神经基元,辐射场,高斯泼溅,免射线步进渲染,新视角合成 |
| 2026-02-27 | ★ **[Compact3DGS](3dgs_2026-02.md#1-prune-wisely-reconstruct-sharply-compact-3d-gaussian-splatting-via-adaptive-pruning-and-difference-of-gaussian-primitives)** | 2602.24136 | 3D高斯泼溅,自适应剪枝,高斯差分基元,模型压缩 CVPR'26 |
| 2026-02-27 | ★ **[MEGS2](3dgs_2026-02.md#5-megs-2-memory-efficient-gaussian-splatting-via-spherical-gaussians-and-unified-pruning)** | 2509.07021 | 3D高斯溅射,显存压缩,球面高斯瓣,统一软剪枝 ICLR'26 |
| 2026-02-26 | ★ **[UBS](3dgs_2026-02.md#7-universal-beta-splatting)** | 2510.03312 | Beta核,高斯溅射,辐射场渲染,实时渲染,各向异性建模 ICLR'26 |
| 2026-02-24 | ★ **[DropAnSH-GS](3dgs_2026-02.md#2-dropping-anchor-and-spherical-harmonics-for-sparse-view-gaussian-splatting)** | 2602.20933 | 高斯泼溅,稀疏视角重建,锚点丢弃,球谐函数,模型压缩 CVPR'26 |
| 2026-02-23 | [Large-scale](3dgs_2026-02.md#2-large-scale-photorealistic-outdoor-3d-scene-reconstruction-from-uav-imagery-using-gaussian-splatting-techniques) | 2602.20342 | 3D高斯泼溅,无人机三维重建,实时渲染,位姿估计,低延迟管线 |
| 2026-02-23 | ★ **[RAP](3dgs_2026-02.md#4-rap-fast-feedforward-rendering-free-attribute-guided-primitive-importance-score-prediction-for-efficient-3d-gaussian-splatting-processing)** | 2602.19753 | 3D高斯泼溅,基元重要性预测,免渲染网络,属性引导,模型压缩 CVPR'26 |
| 2026-02-16 | [GMR](3dgs_2026-02.md#3-gaussian-mesh-renderer-for-lightweight-differentiable-rendering) | 2602.14493 | 可微渲染,3D高斯溅射,网格重建,梯度优化,轻量级渲染 |
| 2026-02-11 | [LeafFit](3dgs_2026-02.md#1-leaffit-plant-assets-creation-from-3d-gaussian-splatting) | 2602.11577 | 3D高斯溅射,网格重建,可微形变,实例化资产,顶点着色器 |
| 2026-02-10 | [CompSplat](3dgs_2026-02.md#5-compsplat-compression-aware-3d-gaussian-splatting-for-real-world-video) | 2602.09816 | 3D高斯溅射,新视角合成,压缩感知,自适应剪枝,几何一致性 |
| 2026-02-06 | [GaussianPOP](3dgs_2026-02.md#1-gaussianpop-principled-simplification-framework-for-compact-3d-gaussian-splatting-via-error-quantification) | 2602.06830 | 3D高斯泼溅, 误差量化, 模型剪枝, 渲染优化 |
| 2026-02-05 | [Mini-Splatting2](3dgs_2026-02.md#3-efficient-scene-modeling-via-structure-aware-and-region-prioritized-3d-gaussians) | 2411.12788 | 3D高斯溅射,结构感知分布,区域优先优化,几何正则化,高效建模 |

**概要**: 本类论文涉及神经基元、模型压缩、高效建模、可微渲染、稀疏视角重建、免射线步进渲染、可微形变、结构感知分布等研究方向，共 12 篇。

---

## 八、动态场景与4D {#cat-dynamic-4d}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-28 | ★ **[PD2GS](3dgs_2026-02.md#5-pd-2-gs-part-level-decoupling-and-continuous-deformation-of-articulated-objects-via-gaussian-splatting)** | 2506.09663 | 高斯溅射,铰接物体,部件解耦,连续形变,运动学建模 ICLR'26 |
| 2026-02-27 | [DAGS-SLAM](3dgs_2026-02.md#3-dags-slam-dynamic-aware-3dgs-slam-via-spatiotemporal-motion-probability-and-uncertainty-aware-scheduling) | 2602.21644 | 3D高斯泼溅,动态SLAM,运动概率估计,不确定性调度,实时重建 |
| 2026-02-26 | [LaGS](3dgs_2026-02.md#2-latent-gaussian-splatting-for-4d-panoptic-occupancy-tracking) | 2602.23172 | 潜在高斯溅射,4D占据网格,全景分割,动态场景跟踪,多视图聚合 |
| 2026-02-26 | ★ **[USplat4D](3dgs_2026-02.md#5-uncertainty-matters-in-dynamic-gaussian-splatting-for-monocular-4d-reconstruction)** | 2510.12768 | 动态高斯溅射,不确定性估计,时空图优化,单目4D重建 ICLR'26 |
| 2026-02-26 | ★ **[ST-GS](3dgs_2026-02.md#8-st-gs-vision-based-3d-semantic-occupancy-prediction-with-spatial-temporal-gaussian-splatting)** | 2509.16552 | 3D占用预测, 高斯溅射, 时空建模, 注意力机制, 自动驾驶 ICRA'26 |
| 2026-02-24 | [RU4D-SLAM](3dgs_2026-02.md#3-ru4d-slam-reweighting-uncertainty-in-gaussian-splatting-slam-for-4d-scene-reconstruction) | 2602.20807 | 高斯溅射,SLAM,4D重建,不确定性建模,动态场景 |
| 2026-02-23 | ★ **[OnlineSCD](3dgs_2026-02.md#5-changes-in-real-time-online-scene-change-detection-with-multi-view-fusion)** | 2511.12370 | 在线场景变化检测, 3D高斯溅射, 多视图融合, 自监督学习, 实时姿态估计 CVPR'26 |
| 2026-02-20 | [Diff2DGS](3dgs_2026-02.md#2-diff2dgs-reliable-reconstruction-of-occluded-surgical-scenes-via-2d-gaussian-splatting) | 2602.18314 | 2D高斯溅射,扩散模型,遮挡修复,动态形变,手术场景重建 |
| 2026-02-19 | [Local-EndoGS](3dgs_2026-02.md#1-4d-monocular-surgical-reconstruction-under-arbitrary-camera-motions) | 2602.17473 | 单目内窥镜,4D重建,3D高斯溅射,可变形场景,窗口化表示 |
| 2026-02-19 | [NRGS-SLAM](3dgs_2026-02.md#2-nrgs-slam-monocular-non-rigid-slam-for-endoscopy-via-deformation-aware-3d-gaussian-splatting) | 2602.17182 | 3D高斯泼溅,非刚性SLAM,形变感知,贝叶斯自监督,内窥镜应用 |
| 2026-02-19 | [i-PhysGaussian](3dgs_2026-02.md#5-i-physgaussian-implicit-physical-simulation-for-3d-gaussian-splatting) | 2602.17117 | 3D高斯溅射,隐式物质点法,物理仿真,动量平衡优化 |
| 2026-02-16 | [TimeArchival](3dgs_2026-02.md#1-time-archival-camera-virtualization-for-sports-and-visual-performances) | 2602.15181 | 相机虚拟化,神经体积渲染,动态场景,时间归档,新视角合成 |
| 2026-02-14 | [ReaDy-Go](3dgs_2026-02.md#3-ready-go-real-to-sim-dynamic-3d-gaussian-splatting-simulation-for-environment-specific-visual-navigation-with-moving-obstacles) | 2602.11575 | 3D高斯溅射,虚实迁移仿真,动态场景,视觉导航,移动障碍物 |
| 2026-02-12 | [TG-Field](3dgs_2026-02.md#3-tg-field-geometry-aware-radiative-gaussian-fields-for-tomographic-reconstruction) | 2602.11705 | 3D高斯泼溅,几何感知形变,稀疏CT重建,动态场景建模,时空注意力 |
| 2026-02-12 | ★ **[NGFF](3dgs_2026-02.md#5-learning-physics-grounded-4d-dynamics-with-neural-gaussian-force-fields)** | 2602.00148 | 神经高斯力场,物理驱动建模,4D视频生成,3D高斯溅射,世界模型 ICLR'26 |
| 2026-02-12 | ★ **[ArmGS](3dgs_2026-02.md#6-armgs-composite-gaussian-appearance-refinement-for-modeling-dynamic-urban-environments)** | 2507.03886 | 3D高斯泼溅, 多粒度外观优化, 动态城市场景, 自动驾驶仿真 ICRA'26 |
| 2026-02-10 | [Faster-GS](3dgs_2026-02.md#4-faster-gs-analyzing-and-improving-gaussian-splatting-optimization) | 2602.09999 | 3D高斯泼溅,训练加速,梯度近似,数值稳定性,4D重建 |
| 2026-02-08 | [Color3D](3dgs_2026-02.md#4-color3d-controllable-and-consistent-3d-colorization-with-personalized-colorizer) | 2510.10152 | 个性化色彩化, 高斯溅射, 跨视角一致性, 动态3D重建, 单视图引导 |
| 2026-02-05 | [XSIM](3dgs_2026-02.md#2-unified-sensor-simulation-for-autonomous-driving) | 2602.05617 | 3D高斯溅射, 传感器仿真, 卷帘快门建模, 相位建模, 自动驾驶 |
| 2026-02-02 | [FastPhysGS](3dgs_2026-02.md#3-fastphysgs-accelerating-physics-based-dynamic-3dgs-simulation-via-interior-completion-and-adaptive-optimization) | 2602.01723 | 3D高斯泼溅,物理模拟,粒子填充,双向图优化,动态场景 |

**概要**: 本类论文涉及个性化色彩化、跨视角一致性、单目4D重建、动态形变、运动学建模、连续形变、多粒度外观优化、动态场景建模等研究方向，共 20 篇。

---

## 九、核心算法与优化 {#cat-core-opt}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-27 | [SR3R](3dgs_2026-02.md#2-sr3r-rethinking-super-resolution-3d-reconstruction-with-feed-forward-gaussian-splatting) | 2602.24020 | 3D高斯溅射,超分辨率,前馈网络,稀疏视图重建,零样本泛化 |
| 2026-02-26 | ★ **[USplat4D](3dgs_2026-02.md#5-uncertainty-matters-in-dynamic-gaussian-splatting-for-monocular-4d-reconstruction)** | 2510.12768 | 动态高斯溅射,不确定性估计,时空图优化,单目4D重建 ICLR'26 |
| 2026-02-26 | ★ **[UBS](3dgs_2026-02.md#7-universal-beta-splatting)** | 2510.03312 | Beta核,高斯溅射,辐射场渲染,实时渲染,各向异性建模 ICLR'26 |
| 2026-02-26 | [SplatSDF](3dgs_2026-02.md#9-splatsdf-boosting-sdf-nerf-via-architecture-level-fusion-with-gaussian-splats) | 2411.15468 | SDF-NeRF,3D高斯泼溅,架构级融合,梯度加速,几何重建 |
| 2026-02-25 | [DGGS](3dgs_2026-02.md#4-distractor-free-generalizable-3d-gaussian-splatting) | 2411.17605 | 3D高斯溅射,可泛化重建,干扰掩码预测,两阶段推理剪枝 |
| 2026-02-24 | [M-Gaussian](3dgs_2026-02.md#1-m-gaussian-an-magnetic-gaussian-framework-for-efficient-multi-stack-mri-reconstruction) | 2603.00145 | 3D高斯泼溅,MRI重建,神经残差场,物理渲染,多分辨率训练 |
| 2026-02-24 | ★ **[DropAnSH-GS](3dgs_2026-02.md#2-dropping-anchor-and-spherical-harmonics-for-sparse-view-gaussian-splatting)** | 2602.20933 | 高斯泼溅,稀疏视角重建,锚点丢弃,球谐函数,模型压缩 CVPR'26 |
| 2026-02-24 | ★ **[UPNet](3dgs_2026-02.md#7-peering-into-the-unknown-active-view-selection-with-neural-uncertainty-maps-for-3d-reconstruction)** | 2506.14856 | 主动视角选择,神经不确定性图,3D重建,新视角合成 ICLR'26 |
| 2026-02-23 | [AestheticField](3dgs_2026-02.md#1-aesthetic-camera-viewpoint-suggestion-with-3d-aesthetic-field) | 2602.20363 | 3D美学场,3D高斯溅射,视角推荐,知识蒸馏,梯度优化 |
| 2026-02-23 | ★ **[AugRF](3dgs_2026-02.md#3-augmented-radiance-field-a-general-framework-for-enhanced-gaussian-splatting)** | 2602.19916 | 3D高斯泼溅,增强高斯核,镜面反射建模,误差补偿,辐射场重建 ICLR'26 |
| 2026-02-23 | ★ **[RAP](3dgs_2026-02.md#4-rap-fast-feedforward-rendering-free-attribute-guided-primitive-importance-score-prediction-for-efficient-3d-gaussian-splatting-processing)** | 2602.19753 | 3D高斯泼溅,基元重要性预测,免渲染网络,属性引导,模型压缩 CVPR'26 |
| 2026-02-23 | ★ **[OnlineSCD](3dgs_2026-02.md#5-changes-in-real-time-online-scene-change-detection-with-multi-view-fusion)** | 2511.12370 | 在线场景变化检测, 3D高斯溅射, 多视图融合, 自监督学习, 实时姿态估计 CVPR'26 |
| 2026-02-20 | ★ **[UrbanGS](3dgs_2026-02.md#3-urbangs-a-scalable-and-efficient-architecture-for-geometrically-accurate-large-scene-reconstruction)** | 2602.02089 | 3D高斯溅射,深度法线正则化,自适应剪枝,城市场景重建 ICLR'26 |
| 2026-02-19 | [i-PhysGaussian](3dgs_2026-02.md#5-i-physgaussian-implicit-physical-simulation-for-3d-gaussian-splatting) | 2602.17117 | 3D高斯溅射,隐式物质点法,物理仿真,动量平衡优化 |
| 2026-02-17 | [DARB-Splatting](3dgs_2026-02.md#3-darb-splatting-generalizing-splatting-with-decaying-anisotropic-radial-basis-functions) | 2501.12369 | 3D高斯泼溅, 径向基函数, 重建核, 新视角合成, 3D重建 |
| 2026-02-16 | [GMR](3dgs_2026-02.md#3-gaussian-mesh-renderer-for-lightweight-differentiable-rendering) | 2602.14493 | 可微渲染,3D高斯溅射,网格重建,梯度优化,轻量级渲染 |
| 2026-02-16 | [MS-Splatting](3dgs_2026-02.md#4-multi-spectral-gaussian-splatting-with-neural-color-representation) | 2506.03407 | 多光谱渲染, 3D高斯溅射, 神经色彩表示, 联合特征编码 |
| 2026-02-13 | [GSM-GS](3dgs_2026-02.md#3-gsm-gs-geometry-constrained-single-and-multi-view-gaussian-splatting-for-surface-reconstruction) | 2602.12796 | 3D高斯溅射,几何约束,表面重建,自适应加权,多视图一致性 |
| 2026-02-12 | [EDGS](3dgs_2026-02.md#7-edgs-eliminating-densification-for-efficient-convergence-of-3dgs) | 2504.13204 | 3D高斯泼溅,密集初始化,密度增长消除,快速收敛,几何重建 |
| 2026-02-11 | ★ **[SplatDistill](3dgs_2026-02.md#2-splat-and-distill-augmenting-teachers-with-feed-forward-3d-reconstruction-for-3d-aware-distillation)** | 2602.06032 | 3D高斯表示,知识蒸馏,前馈重建,3D感知,视觉基础模型 ICLR'26 |
| 2026-02-10 | [ERGO](3dgs_2026-02.md#1-ergo-excess-risk-guided-optimization-for-high-fidelity-monocular-3d-gaussian-splatting) | 2602.10278 | 单目3D重建, 高斯溅射, 超额风险分解, 自适应优化 |
| 2026-02-10 | [XSPLAIN](3dgs_2026-02.md#2-xsplain-xai-enabling-splat-based-prototype-learning-for-attribute-aware-interpretability) | 2602.10239 | 3D高斯溅射,可解释人工智能,原型学习,特征解耦,分类 |
| 2026-02-10 | [Faster-GS](3dgs_2026-02.md#4-faster-gs-analyzing-and-improving-gaussian-splatting-optimization) | 2602.09999 | 3D高斯泼溅,训练加速,梯度近似,数值稳定性,4D重建 |
| 2026-02-09 | [Converged3DGS](3dgs_2026-02.md#1-analysis-of-converged-3d-gaussian-splatting-solutions-density-effects-and-prediction-limit) | 2602.08909 | 3D高斯溅射,密度分层,参数预测,渲染优化,可见性分析 |
| 2026-02-08 | [ThermoSplat](3dgs_2026-02.md#2-thermosplat-cross-modal-3d-gaussian-splatting-with-feature-modulation-and-geometry-decoupling) | 2601.15897 | 3D高斯溅射,跨模态重建,特征调制,几何解耦,热红外感知 |
| 2026-02-06 | [GaussianPOP](3dgs_2026-02.md#1-gaussianpop-principled-simplification-framework-for-compact-3d-gaussian-splatting-via-error-quantification) | 2602.06830 | 3D高斯泼溅, 误差量化, 模型剪枝, 渲染优化 |
| 2026-02-05 | [Mini-Splatting2](3dgs_2026-02.md#3-efficient-scene-modeling-via-structure-aware-and-region-prioritized-3d-gaussians) | 2411.12788 | 3D高斯溅射,结构感知分布,区域优先优化,几何正则化,高效建模 |
| 2026-02-05 | [MVGS](3dgs_2026-02.md#4-mvgs-multi-view-regulated-gaussian-splatting-for-novel-view-synthesis) | 2410.02103 | 3D高斯泼溅, 多视图训练, 跨射线密集化, 新视角合成, 几何重建 |
| 2026-02-04 | [QuantumGS](3dgs_2026-02.md#2-quantumgs-quantum-encoding-framework-for-gaussian-splatting) | 2602.05047 | 3D高斯泼溅,变分量子电路,布洛赫球编码,视角相关渲染 |
| 2026-02-02 | [FastPhysGS](3dgs_2026-02.md#3-fastphysgs-accelerating-physics-based-dynamic-3dgs-simulation-via-interior-completion-and-adaptive-optimization) | 2602.01723 | 3D高斯泼溅,物理模拟,粒子填充,双向图优化,动态场景 |

**概要**: 本类论文涉及联合特征编码、单目4D重建、零样本泛化、超分辨率、网格重建、多光谱渲染、基元重要性预测、热红外感知等研究方向，共 30 篇。

---

## 十、SLAM与建图 {#cat-slam}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-27 | [DAGS-SLAM](3dgs_2026-02.md#3-dags-slam-dynamic-aware-3dgs-slam-via-spatiotemporal-motion-probability-and-uncertainty-aware-scheduling) | 2602.21644 | 3D高斯泼溅,动态SLAM,运动概率估计,不确定性调度,实时重建 |
| 2026-02-26 | [Sapling-NeRF](3dgs_2026-02.md#3-sapling-nerf-geo-localised-sapling-reconstruction-in-forests-for-ecological-monitoring) | 2602.22731 | NeRF,激光SLAM,GNSS定位,三维重建,生态监测 |
| 2026-02-24 | [RU4D-SLAM](3dgs_2026-02.md#3-ru4d-slam-reweighting-uncertainty-in-gaussian-splatting-slam-for-4d-scene-reconstruction) | 2602.20807 | 高斯溅射,SLAM,4D重建,不确定性建模,动态场景 |
| 2026-02-23 | [Large-scale](3dgs_2026-02.md#2-large-scale-photorealistic-outdoor-3d-scene-reconstruction-from-uav-imagery-using-gaussian-splatting-techniques) | 2602.20342 | 3D高斯泼溅,无人机三维重建,实时渲染,位姿估计,低延迟管线 |
| 2026-02-23 | [MOGS](3dgs_2026-02.md#6-mogs-monocular-object-guided-gaussian-splatting-in-large-scenes) | 2509.06685 | 3D高斯溅射,单目重建,语义形状先验,视觉惯性SfM,深度优化 |
| 2026-02-19 | [NRGS-SLAM](3dgs_2026-02.md#2-nrgs-slam-monocular-non-rigid-slam-for-endoscopy-via-deformation-aware-3d-gaussian-splatting) | 2602.17182 | 3D高斯泼溅,非刚性SLAM,形变感知,贝叶斯自监督,内窥镜应用 |
| 2026-02-14 | [Planetary3D](3dgs_2026-02.md#1-high-fidelity-3d-reconstruction-for-planetary-exploration) | 2602.13909 | 神经辐射场, 高斯溅射, 三维重建, 行星探测, 机器人建图 |
| 2026-02-12 | [LatentAM](3dgs_2026-02.md#1-latentam-real-time-large-scale-latent-gaussian-attention-mapping-via-online-dictionary-learning) | 2602.12314 | 3D高斯溅射,在线字典学习,开放词汇感知,机器人建图,特征映射 |
| 2026-02-10 | [OpenMonoGS-SLAM](3dgs_2026-02.md#7-openmonogs-slam-monocular-gaussian-splatting-slam-with-open-set-semantics) | 2512.08625 | 单目SLAM, 3D高斯溅射, 开集语义, 视觉基础模型, 语义建图 |
| 2026-02-04 | [3DGS-SLAM](3dgs_2026-02.md#4-towards-next-generation-slam-a-survey-on-3dgs-slam-focusing-on-performance-robustness-and-future-directions) | 2602.04251 | 3D高斯泼溅,SLAM,性能优化,动态鲁棒性,系统综述 |
| 2026-02-02 | [HI-SLAM2](3dgs_2026-02.md#6-hi-slam2-geometry-aware-gaussian-slam-for-fast-monocular-scene-reconstruction) | 2411.17982 | 3D高斯溅射,单目SLAM,几何感知,稠密重建,尺度对齐 |

**概要**: 本类论文涉及稠密重建、生态监测、开集语义、系统综述、形变感知、语义建图、视觉基础模型、动态鲁棒性等研究方向，共 11 篇。

---

## 十一、风格迁移与编辑 {#cat-style-edit}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-27 | ★ **[Stylos](3dgs_2026-02.md#4-stylos-multi-view-3d-stylization-with-single-forward-gaussian-splatting)** | 2509.26455 | 3D高斯溅射,风格迁移,单次前向传播,双路径架构,零样本生成 ICLR'26 |
| 2026-02-19 | ★ **[MeGA](3dgs_2026-02.md#6-mega-hybrid-mesh-gaussian-head-avatar-for-high-fidelity-rendering-and-head-editing)** | 2404.19026 | 混合网格高斯,头部数字人,神经渲染,动态形变,属性编辑 CVPR'25 |
| 2026-02-10 | [ArtisanGS](3dgs_2026-02.md#3-artisangs-interactive-tools-for-gaussian-splat-selection-with-ai-and-human-in-the-loop) | 2602.10173 | 3D高斯溅射,交互式分割,掩码传播,局部编辑,视频扩散模型 |
| 2026-02-04 | [StyleMe3D](3dgs_2026-02.md#5-styleme3d-stylization-with-disentangled-priors-by-multiple-encoders-on-3d-gaussians) | 2504.15281 | 3D高斯溅射,风格迁移,扩散模型蒸馏,CLIP对齐,几何保真 |
| 2026-02-03 | [AnyStyle](3dgs_2026-02.md#1-anystyle-single-pass-multimodal-stylization-for-3d-gaussian-splatting) | 2602.04043 | 3D高斯泼溅,风格迁移,多模态条件,前馈重建,零样本 |

**概要**: 本类论文涉及多模态条件、零样本生成、风格迁移、动态形变、3D高斯泼溅、CLIP对齐、扩散模型蒸馏、属性编辑等研究方向，共 5 篇。

---

## 十二、语义分割与场景理解 {#cat-seg-understand}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-26 | [LaGS](3dgs_2026-02.md#2-latent-gaussian-splatting-for-4d-panoptic-occupancy-tracking) | 2602.23172 | 潜在高斯溅射,4D占据网格,全景分割,动态场景跟踪,多视图聚合 |
| 2026-02-26 | ★ **[ST-GS](3dgs_2026-02.md#8-st-gs-vision-based-3d-semantic-occupancy-prediction-with-spatial-temporal-gaussian-splatting)** | 2509.16552 | 3D占用预测, 高斯溅射, 时空建模, 注意力机制, 自动驾驶 ICRA'26 |
| 2026-02-19 | [B3-Seg](3dgs_2026-02.md#3-b-3-seg-camera-free-training-free-3dgs-segmentation-via-analytic-eig-and-beta-bernoulli-bayesian-updates) | 2602.17134 | 3D高斯溅射,贝叶斯更新,期望信息增益,开放词汇分割,主动视角选择 |
| 2026-02-16 | [DigitalTwin](3dgs_2026-02.md#5-digital-twin-generation-from-visual-data-a-survey) | 2504.13159 | 数字孪生,3D高斯泼溅,基础模型,语义分割,视觉重建 |
| 2026-02-11 | ★ **[SplatDistill](3dgs_2026-02.md#2-splat-and-distill-augmenting-teachers-with-feed-forward-3d-reconstruction-for-3d-aware-distillation)** | 2602.06032 | 3D高斯表示,知识蒸馏,前馈重建,3D感知,视觉基础模型 ICLR'26 |
| 2026-02-10 | [XSPLAIN](3dgs_2026-02.md#2-xsplain-xai-enabling-splat-based-prototype-learning-for-attribute-aware-interpretability) | 2602.10239 | 3D高斯溅射,可解释人工智能,原型学习,特征解耦,分类 |
| 2026-02-10 | [ArtisanGS](3dgs_2026-02.md#3-artisangs-interactive-tools-for-gaussian-splat-selection-with-ai-and-human-in-the-loop) | 2602.10173 | 3D高斯溅射,交互式分割,掩码传播,局部编辑,视频扩散模型 |
| 2026-02-10 | [OpenMonoGS-SLAM](3dgs_2026-02.md#7-openmonogs-slam-monocular-gaussian-splatting-slam-with-open-set-semantics) | 2512.08625 | 单目SLAM, 3D高斯溅射, 开集语义, 视觉基础模型, 语义建图 |
| 2026-02-10 | [VALA](3dgs_2026-02.md#8-visibility-aware-language-aggregation-for-open-vocabulary-segmentation-in-3d-gaussian-splatting) | 2509.05515 | 3D高斯溅射,开放词汇分割,可见性门控,多视图特征融合 |
| 2026-02-08 | [G2P](3dgs_2026-02.md#3-g2p-gaussian-to-point-attribute-alignment-for-boundary-aware-3d-semantic-segmentation) | 2601.03510 | 3D高斯泼溅,点云分割,属性对齐,边界感知,语义分割 |
| 2026-02-01 | [Split&Splat](3dgs_2026-02.md#1-split-amp-splat-zero-shot-panoptic-segmentation-via-explicit-instance-modeling-and-3d-gaussian-splatting) | 2602.03809 | 3D高斯溅射,全景分割,实例建模,场景重建 |

**概要**: 本类论文涉及贝叶斯更新、多视图特征融合、开集语义、期望信息增益、视觉重建、场景重建、边界感知、语义建图等研究方向，共 11 篇。

---

## 十三、领域应用 {#cat-domain-app}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-26 | [Sapling-NeRF](3dgs_2026-02.md#3-sapling-nerf-geo-localised-sapling-reconstruction-in-forests-for-ecological-monitoring) | 2602.22731 | NeRF,激光SLAM,GNSS定位,三维重建,生态监测 |
| 2026-02-24 | [M-Gaussian](3dgs_2026-02.md#1-m-gaussian-an-magnetic-gaussian-framework-for-efficient-multi-stack-mri-reconstruction) | 2603.00145 | 3D高斯泼溅,MRI重建,神经残差场,物理渲染,多分辨率训练 |
| 2026-02-24 | [Monocular](3dgs_2026-02.md#4-monocular-endoscopic-tissue-3d-reconstruction-with-multi-level-geometry-regularization) | 2602.20718 | 3D高斯泼溅,符号距离场,形变正则化,内窥镜重建,表面约束 |
| 2026-02-20 | [Diff2DGS](3dgs_2026-02.md#2-diff2dgs-reliable-reconstruction-of-occluded-surgical-scenes-via-2d-gaussian-splatting) | 2602.18314 | 2D高斯溅射,扩散模型,遮挡修复,动态形变,手术场景重建 |
| 2026-02-19 | [Local-EndoGS](3dgs_2026-02.md#1-4d-monocular-surgical-reconstruction-under-arbitrary-camera-motions) | 2602.17473 | 单目内窥镜,4D重建,3D高斯溅射,可变形场景,窗口化表示 |
| 2026-02-19 | [NRGS-SLAM](3dgs_2026-02.md#2-nrgs-slam-monocular-non-rigid-slam-for-endoscopy-via-deformation-aware-3d-gaussian-splatting) | 2602.17182 | 3D高斯泼溅,非刚性SLAM,形变感知,贝叶斯自监督,内窥镜应用 |
| 2026-02-16 | [TimeArchival](3dgs_2026-02.md#1-time-archival-camera-virtualization-for-sports-and-visual-performances) | 2602.15181 | 相机虚拟化,神经体积渲染,动态场景,时间归档,新视角合成 |
| 2026-02-16 | [MS-Splatting](3dgs_2026-02.md#4-multi-spectral-gaussian-splatting-with-neural-color-representation) | 2506.03407 | 多光谱渲染, 3D高斯溅射, 神经色彩表示, 联合特征编码 |
| 2026-02-16 | [DigitalTwin](3dgs_2026-02.md#5-digital-twin-generation-from-visual-data-a-survey) | 2504.13159 | 数字孪生,3D高斯泼溅,基础模型,语义分割,视觉重建 |
| 2026-02-14 | [Planetary3D](3dgs_2026-02.md#1-high-fidelity-3d-reconstruction-for-planetary-exploration) | 2602.13909 | 神经辐射场, 高斯溅射, 三维重建, 行星探测, 机器人建图 |
| 2026-02-12 | [TG-Field](3dgs_2026-02.md#3-tg-field-geometry-aware-radiative-gaussian-fields-for-tomographic-reconstruction) | 2602.11705 | 3D高斯泼溅,几何感知形变,稀疏CT重建,动态场景建模,时空注意力 |
| 2026-02-02 | [TVGS](3dgs_2026-02.md#4-from-slices-to-structures-unsupervised-3d-reconstruction-of-female-pelvic-anatomy-from-freehand-transvaginal-ultrasound) | 2508.14552 | 高斯泼溅,无监督三维重建,超声成像,联合位姿优化,可微光栅化 |
| 2026-02-01 | [Radioactive](3dgs_2026-02.md#3-radioactive-3d-gaussian-ray-tracing-for-tomographic-reconstruction) | 2602.01057 | 3D高斯溅射,光线追踪,断层重建,解析线积分,几何校正 |

**概要**: 本类论文涉及时空注意力、稀疏CT重建、生态监测、联合特征编码、2D高斯溅射、视觉重建、断层重建、可变形场景等研究方向，共 13 篇。

---

## 十四、数字人与人体重建 {#cat-human}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-24 | [WildGHand](3dgs_2026-02.md#5-wildghand-learning-anti-perturbation-gaussian-hand-avatars-from-monocular-in-the-wild-videos) | 2602.20556 | 3D高斯溅射,手部重建,扰动解耦,野外视频,优化策略 |
| 2026-02-19 | ★ **[MeGA](3dgs_2026-02.md#6-mega-hybrid-mesh-gaussian-head-avatar-for-high-fidelity-rendering-and-head-editing)** | 2404.19026 | 混合网格高斯,头部数字人,神经渲染,动态形变,属性编辑 CVPR'25 |
| 2026-02-12 | [OMEGA-Avatar](3dgs_2026-02.md#4-omega-avatar-one-shot-modeling-of-360-gaussian-avatars) | 2602.11693 | 单图重建,3D高斯溅射,数字人生成,前向网络,网格变形 |
| 2026-02-10 | [FG-3DGS](3dgs_2026-02.md#6-toward-fine-grained-facial-control-in-3d-talking-head-generation) | 2602.09736 | 3D高斯泼溅,频率感知解耦,数字人生成,唇形同步 |
| 2026-02-05 | [SuperHead](3dgs_2026-02.md#1-from-blurry-to-believable-enhancing-low-quality-talking-heads-with-3d-generative-priors) | 2602.06122 | 3D高斯溅射,生成先验反演,数字人重建,动态超分辨率 |
| 2026-02-04 | [PoseGaussian](3dgs_2026-02.md#1-posegaussian-pose-driven-novel-view-synthesis-for-robust-3d-human-reconstruction) | 2602.05190 | 高斯溅射, 姿态引导, 新视角合成, 人体重建, 实时渲染 |
| 2026-02-04 | [JOintGS](3dgs_2026-02.md#3-jointgs-joint-optimization-of-cameras-bodies-and-3d-gaussians-for-in-the-wild-monocular-reconstruction) | 2602.04317 | 3D高斯溅射,联合优化,人体重建,相机标定,前景背景解耦 |

**概要**: 本类论文涉及相机标定、前景背景解耦、动态形变、人体重建、姿态引导、实时渲染、野外视频、前向网络等研究方向，共 7 篇。

---

## 十五、安全与版权 {#cat-security}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-22 | [DefenseSplat](3dgs_2026-02.md#1-defensesplat-enhancing-the-robustness-of-3d-gaussian-splatting-via-frequency-aware-filtering) | 2602.19323 | 3D高斯泼溅, 对抗防御, 频率感知滤波, 小波变换, 鲁棒性 |
| 2026-02-02 | [3DGS-IP](3dgs_2026-02.md#1-intellectual-property-protection-for-3d-gaussian-splatting-assets-a-survey) | 2602.03878 | 3D高斯泼溅,知识产权保护,扰动机制,鲁棒性评估,综述 |
| 2026-02-01 | [3DGS水印](3dgs_2026-02.md#2-position-3d-gaussian-splatting-watermarking-should-be-scenario-driven-and-threat-model-explicit) | 2602.02602 | 3D高斯溅射,数字水印,威胁模型,场景驱动,版权保护 |

**概要**: 本类论文涉及对抗防御、数字水印、小波变换、3D高斯溅射、版权保护、鲁棒性评估、威胁模型、频率感知滤波等研究方向，共 3 篇。

---

## 十六、逆渲染与光照 {#cat-inverserender}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-20 | ★ **[Luminance-GS++](3dgs_2026-02.md#1-unifying-color-and-lightness-correction-with-view-adaptive-curve-adjustment-for-robust-3d-novel-view-synthesis)** | 2602.18322 | 3D高斯溅射,新视角合成,亮度校正,视角自适应,光度一致性 CVPR'25 |
| 2026-02-17 | [Relightable3DGS](3dgs_2026-02.md#2-zero-shot-uav-navigation-in-forests-via-relightable-3d-gaussian-splatting) | 2602.07101 | 3D高斯溅射,可重光照,强化学习,零样本迁移,无人机导航 |
| 2026-02-13 | [PBR-GS](3dgs_2026-02.md#1-nighttime-autonomous-driving-scene-reconstruction-with-physically-based-gaussian-splatting) | 2602.13549 | 3D高斯溅射,物理渲染,BRDF材质优化,夜间场景重建 |

**概要**: 本类论文涉及BRDF材质优化、强化学习、无人机导航、光度一致性、亮度校正、视角自适应、新视角合成、3D高斯溅射等研究方向，共 3 篇。

---

## 十七、无线与射频传播 {#cat-rf}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-02-19 | [MultimodalGS](3dgs_2026-02.md#4-3d-scene-rendering-with-multimodal-gaussian-splatting) | 2602.17124 | 高斯溅射,射频传感,多模态融合,3D场景渲染,深度预测 |

**概要**: 本类论文涉及射频传感、多模态融合、高斯溅射、深度预测、3D场景渲染等研究方向，共 1 篇。

---

## 统计概览

| 类别 | 论文数 |
|------|--------|
| 几何与表面重建 | 66 |
| 新视角合成 | 30 |
| 视觉定位 | 2 |
| 机器人仿真与具身智能 | 10 |
| 生成式模型 | 14 |
| 自动驾驶应用 | 8 |
| 渲染加速与压缩 | 12 |
| 动态场景与4D | 20 |
| 核心算法与优化 | 30 |
| SLAM与建图 | 11 |
| 风格迁移与编辑 | 5 |
| 语义分割与场景理解 | 11 |
| 领域应用 | 13 |
| 数字人与人体重建 | 7 |
| 安全与版权 | 3 |
| 逆渲染与光照 | 3 |
| 无线与射频传播 | 1 |
| **合计** | **246** |
