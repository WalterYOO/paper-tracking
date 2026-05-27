# 3D Gaussian Splatting 论文分类索引 (2026-04)

> 基于 `3dgs_2026-04.md` 中收集的论文，按研究方向细分类。
> 注：★ 表示被顶会/顶刊录用。

## 目录

- [3D Gaussian Splatting 论文分类索引 (2026-04)](3dgs_2026-04.md#3d-gaussian-splatting-论文分类索引-2026-04)
  - [目录](3dgs_2026-04.md#目录)
  - [一、核心算法与优化](3dgs_2026-04.md#cat-core-opt)
  - [二、渲染加速与压缩](3dgs_2026-04.md#cat-render-accel)
  - [三、新视角合成](3dgs_2026-04.md#cat-nvs)
    - [3.1 可泛化 / 前向](3dgs_2026-04.md#cat-nvs-gg)
    - [3.2 稀疏视角](3dgs_2026-04.md#cat-nvs-sparse)
  - [四、动态场景与 4D](3dgs_2026-04.md#cat-dynamic-4d)
  - [五、语义分割与场景理解](3dgs_2026-04.md#cat-seg-understand)
  - [六、视觉定位与安全](3dgs_2026-04.md#cat-visloc)
  - [七、几何与表面重建](3dgs_2026-04.md#cat-geo-recon)
  - [八、生成式模型](3dgs_2026-04.md#cat-generative)
  - [九、流媒体与编码](3dgs_2026-04.md#cat-streaming)
  - [十、SLAM 与建图](3dgs_2026-04.md#cat-slam)
  - [十一、机器人与仿真](3dgs_2026-04.md#cat-robot-sim)
  - [十二、数字人与人体重建](3dgs_2026-04.md#cat-avatar-human)
  - [十三、风格迁移与编辑](3dgs_2026-04.md#cat-style-edit)
  - [十四、领域应用](3dgs_2026-04.md#cat-domain-special)
  - [v2 版本更新论文](3dgs_2026-04.md#v2-版本更新论文)
    - [4/26-30 v2 更新](3dgs_2026-04.md#v2-426-30)
    - [4/21-25 v2 更新](3dgs_2026-04.md#v2-421-25)
  - [统计概览](3dgs_2026-04.md#统计概览)

---

## 一、核心算法与优化 {#cat-core-opt}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-30 | ★ **[Structure-Aware Densification](3dgs_2026-04.md#4-faster-3d-gaussian-splatting-convergence-via-structure-aware-densification)** | [2604.28016](https://arxiv.org/abs/2604.28016) | 多尺度频率分析各向异性分裂，加速收敛（SIGGRAPH'26） |
| 2026-04-30 | [Softmax-GS](3dgs_2026-04.md#7-softmax-gs-generalized-gaussians-learning-when-to-blend-or-bound) | [2604.27437](https://arxiv.org/abs/2604.27437) | Softmax 竞争机制，高斯重叠区平滑到锐利边界过渡 |
| 2026-04-29 | [Two-View Accumulation](3dgs_2026-04.md#1-two-view-accumulation-as-the-primary-training-lever-for-hybrid-capture-gaussian-splatting) | [2605.00052](https://arxiv.org/abs/2605.00052) | 混合捕获双视角积累，方差分解解释主导效应 |
| 2026-04-29 | [EnerGS](3dgs_2026-04.md#4-energs-energy-based-gaussian-splatting-with-partial-geometric-priors) | [2604.26238](https://arxiv.org/abs/2604.26238) | 部分几何能量场软引导，稀疏多视角光度质量提升 |
| 2026-04-29 | [Deformation Overfitting](3dgs_2026-04.md#2-incoherent-deformation-not-capacity-diagnosing-and-mitigating-overfitting-in-dynamic-gaussian-splatting) | [2604.16747](https://arxiv.org/abs/2604.16747) | 诊断动态 3DGS 过拟合，弹性正则化+稀疏化降阈值（v2） |
| 2026-04-27 | [MERID-GS](3dgs_2026-04.md#1-light-em-up-enabling-few-shot-low-light-3d-gaussian-splatting-with-multi-scale-explicit-retinex-illumination-decoupling-merid-gs) | [2604.24053](https://arxiv.org/abs/2604.24053) | Retinex 光照-反射解耦，少样本低光 3DGS 新视角合成 |
| 2026-04-23 | [YOGO](3dgs_2026-04.md#2-you-only-gaussian-once-yogo-controllable-3d-gaussian-splatting-for-ultra-densely-sampled-scenes) | [2604.21400](https://arxiv.org/abs/2604.21400) | 确定性预算均衡框架，超密集室内场景可控 3DGS |
| 2026-04-22 | [Init vs Densification](3dgs_2026-04.md#8-the-role-and-relationship-of-initialization-and-densification-in-3d-gaussian-splatting) | [2603.20714](https://arxiv.org/abs/2603.20714) | 系统研究 3DGS 初始化与加密的关系（v2） |
| 2026-04-21 | [Gaussians on a Diet](3dgs_2026-04.md#1-gaussians-on-a-diet-high-quality-memory-bounded-3d-gaussian-splatting-training) | [2604.20046](https://arxiv.org/abs/2604.20046) | 内存有界训练框架，边缘设备 80% 峰值显存降低 |
| 2026-04-14 | [SSD-GS](3dgs_2026-04.md#2-ssd-gs-scattering-and-shadow-decomposition-for-relightable-3d-gaussian-splatting) | [2604.13333](https://arxiv.org/abs/2604.13333) | 散射阴影分解可重光照（ICLR'26） |
| 2026-04-13 | [Naka-GS](3dgs_2026-04.md#6-naka-gs-a-bionics-inspired-dual-branch-naka-correction-and-progressive-point-pruning-for-low-light-3dgs) | [2604.11142](https://arxiv.org/abs/2604.11142) | 仿生双分支低光照 3DGS，Naka 色度校正 |
| 2026-04-11 | [3DGS Survey](3dgs_2026-04.md#3-a-survey-on-3d-gaussian-splatting-applications-segmentation-editing-and-generation) | [2508.09977](https://arxiv.org/abs/2508.09977) | 3DGS 应用综述：分割、编辑、生成 |
| 2026-04-09 | [A Survey on 3D Gaussian Splatting](3dgs_2026-04.md#6-a-survey-on-3d-gaussian-splatting) | [2401.03890](https://arxiv.org/abs/2401.03890) | 本文提供了3D高斯溅射领域首个系统性综述。 |
| 2026-04-07 | [In Depth We Trust](3dgs_2026-04.md#4-in-depth-we-trust-reliable-monocular-depth-supervision-for-gaussian-splatting) | [2604.05715](https://arxiv.org/abs/2604.05715) | 针对单目深度估计存在尺度模糊和多视图不一致等问题， |
| 2026-04-03 | [SpectralSplat](3dgs_2026-04.md#1-spectralsplat-appearance-disentangled-feed-forward-gaussian-splatting-for-driving-scenes) | [2604.03462](https://arxiv.org/abs/2604.03462) | 针对前馈3DGS方法中将场景几何与光照、天气等外观属性耦合导致无法重光照的问题， |
| 2026-04-02 | [Fourier Splatting](3dgs_2026-04.md#8-fourier-splatting-generalized-fourier-encoded-primitives-for-scalable-radiance-fields) | [2603.19834](https://arxiv.org/abs/2603.19834) | 针对现有3DGS方法将视觉保真度与图元数量严格绑定的问题， |

**概要**: 改进 3DGS 基础优化过程，包括优化器设计、密度控制、基元分裂/裁剪策略、初始化与加密关系、光照解耦、多模态表示等。

---

## 二、渲染加速与压缩 {#cat-render-accel}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-30 | ★ **[VkSplat](3dgs_2026-04.md#1-vksplat-high-performance-3dgs-training-in-vulkan-compute)** | [2605.00219](https://arxiv.org/abs/2605.00219) | 全 Vulkan 管线 3DGS 训练，速度提升 3.3x，显存降 33%（Eu |
| 2026-04-29 | [MesonGS++](3dgs_2026-04.md#2-mesongs-plus-plus-post-training-compression-of-3d-gaussian-splatting-with-hyperparameter-searching) | [2604.26799](https://arxiv.org/abs/2604.26799) | 剪枝+八叉树+量化联合压缩，34x 压缩保真度无损 |
| 2026-04-28 | [C3G](3dgs_2026-04.md#5-c3g-learning-compact-3d-representations-with-2k-gaussians) | [2512.04021](https://arxiv.org/abs/2512.04021) | 紧凑 3DGS 仅 2K 高斯实现高效场景重建（v2） |
| 2026-04-21 | ★ **[AdaGScale](3dgs_2026-04.md#9-adagscale-viewpoint-adaptive-gaussian-scaling-in-3d-gaussian-splatting-to-reduce-gaussian-tile-pairs)** | [2604.18980](https://arxiv.org/abs/2604.18980) | 视角自适应高斯缩放，tile 交集测试提速 13.8x（DAC'26） |
| 2026-04-20 | [NVGS](3dgs_2026-04.md#2-nvgs-neural-visibility-for-occlusion-culling-in-3d-gaussian-splatting) | [2511.19202](https://arxiv.org/abs/2511.19202) | 神经可见性遮挡剔除，实例共享 MLP+自定义光栅化 |
| 2026-04-17 | [GlobalSplat](3dgs_2026-04.md#4-globalsplat-efficient-feed-forward-3d-gaussian-splatting-via-global-scene-tokens) | [2604.15284](https://arxiv.org/abs/2604.15284) | 全局场景 token 前向 3DGS，16K 高斯/4MB |
| 2026-04-16 | [TokenGS](3dgs_2026-04.md#1-tokengs-decoupling-3d-gaussian-prediction-from-pixels-with-learnable-tokens) | [2604.15239](https://arxiv.org/abs/2604.15239) | 可学习 token 解耦高斯预测，NVIDIA SOTA |
| 2026-04-13 | [IterGS](3dgs_2026-04.md#4-unfolding-3d-gaussian-splatting-via-iterative-gaussian-synopsis) | [2604.11685](https://arxiv.org/abs/2604.11685) | 迭代高斯综述，自顶向下 LOD 层次压缩 |
| 2026-04-11 | [129FPS 3DGS Accelerator](3dgs_2026-04.md#2-a-129fps-full-hd-real-time-accelerator-for-3d-gaussian-splatting) | [2604.10223](https://arxiv.org/abs/2604.10223) | 129FPS 全 HD 3DGS 硬件加速器，0.219W |
| 2026-04-10 | [PointSplat](3dgs_2026-04.md#1-pointsplat-efficient-geometry-driven-pruning-and-transformer-refinement-for-3d-gaussian-splatting) | [2604.09903](https://arxiv.org/abs/2604.09903) | 针对3DGS需要数百万高斯点导致存储开销大的问题，本文提出PointSplat框 |
| 2026-04-08 | [Splats under Pressure](3dgs_2026-04.md#2-splats-under-pressure-exploring-performance-energy-trade-offs-in-real-time-3d-gaussian-splatting-und) | [2604.07177](https://arxiv.org/abs/2604.07177) | 本文研究了在边缘客户端上实时3DGS光栅化的可行性。 |
| 2026-04-07 | [SparseOIT](3dgs_2026-04.md#1-sparseoit-improving-order-independent-transparency-3dgs-via-active-set-method) | [2605.13855](https://arxiv.org/abs/2605.13855) | 针对3D高斯溅射在处理透明和非朗伯材质时的局限性，本文提出SparseOIT方法 |
| 2026-04-06 | [3DTurboQuant](3dgs_2026-04.md#2-3dturboquant-training-free-near-optimal-quantization-for-3d-reconstruction-models) | [2604.05366](https://arxiv.org/abs/2604.05366) | 针对现有3D模型压缩方法需要每场景微调学习数据依赖编码库的问题， |
| 2026-04-06 | ★ **[GEMM-GS](3dgs_2026-04.md#7-gemm-gs-accelerating-3d-gaussian-splatting-on-tensor-cores-with-gemm-compatible-blending)** | [2604.02120](https://arxiv.org/abs/2604.02120) | 针对现有3DGS加速方法忽视了现代GPU的Tensor Cores的问题，（DA |
| 2026-04-02 | [GS^2](3dgs_2026-04.md#4-gs2-graph-based-spatial-distribution-optimization-for-compact-3d-gaussian-splatting) | [2604.01884](https://arxiv.org/abs/2604.01884) | 针对3DGS因大量高斯点导致高内存成本且裁剪方法常损害空间一致性的问题，本文提出 |
| 2026-04-01 | [LG-HCC](3dgs_2026-04.md#8-lg-hcc-local-geometry-aware-hierarchical-context-compression-for-3d-gaussian-splatting) | [2603.28431](https://arxiv.org/abs/2603.28431) | 针对现有3DGS压缩方案忽视几何依赖导致结构退化的问题，本文提出LG-HCC框架 |
| 2026-04-01 | ★ **[CLoD-GS](3dgs_2026-04.md#11-clod-gs-continuous-level-of-detail-via-3d-gaussian-splatting)** | [2510.09997](https://arxiv.org/abs/2510.09997) | 针对传统离散LOD需要存储多份模型副本且在切换时产生视觉跳变伪影的问题，（ICL |

**概要**: 提升 3DGS 渲染性能或降低存储开销，包括硬件加速、Vulkan/CUDA 优化、剪枝量化、紧凑表示、LOD 管理等。

---

## 三、新视角合成 {#cat-nvs}

### 3.1 可泛化 / 前向 {#cat-nvs-gg}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-30 | [SDDF](3dgs_2026-04.md#1-sddf-learning-scene-level-signed-directional-distance-function-with-ellipsoidal-priors-and-neural-residuals) | [2503.20066](https://arxiv.org/abs/2503.20066) | 符号方向距离函数+椭球先验，高效几何重建（v2） |
| 2026-04-27 | [Genie Sim PanoRecon](3dgs_2026-04.md#8-genie-sim-panorecon-fast-immersive-scene-generation-from-single-view-panorama) | [2604.07105](https://arxiv.org/abs/2604.07105) | 前馈 3DGS 快速从全景图生成 3D 场景（v2） |
| 2026-04-23 | [WildSplatter](3dgs_2026-04.md#3-wildsplatter-feed-forward-3d-gaussian-splatting-with-appearance-control-from-unconstrained-images) | [2604.21182](https://arxiv.org/abs/2604.21182) | 前向 3DGS 外观控制，1 秒内无约束照片重建 |
| 2026-04-14 | [DAV-GSWT](3dgs_2026-04.md#9-dav-gswt-diffusion-active-view-sampling-for-data-efficient-gaussian-splatting-wang-tiles) | [2602.15355](https://arxiv.org/abs/2602.15355) | 扩散主动视图采样，数据高效 Wang Tiles |
| 2026-04-09 | ★ **[AnchorSplat](3dgs_2026-04.md#4-anchorsplat-feed-forward-3d-gaussian-splatting-with-3d-geometric-priors)** | [2604.07053](https://arxiv.org/abs/2604.07053) | 针对现有前馈高斯重建模型将高斯表示与输入图像紧密耦合的问题，（CVPR'26） |
| 2026-04-03 | [SparseSplat](3dgs_2026-04.md#3-sparsesplat-towards-applicable-feed-forward-3d-gaussian-splatting-with-pixel-unaligned-prediction) | [2604.03069](https://arxiv.org/abs/2604.03069) | 针对前馈3DGS方法生成的空间均匀且冗余度高的高斯图限制了下游任务集成的问题， |
| 2026-04-03 | ★ **[NavCrafter](3dgs_2026-04.md#5-navcrafter-exploring-3d-scenes-from-a-single-image)** | [2604.02828](https://arxiv.org/abs/2604.02828) | 针对从单张图像创建灵活3D场景的需求，本文提出NavCrafter框架。（ICR |
| 2026-04-01 | [Diff3R](3dgs_2026-04.md#3-diff3r-feed-forward-3d-gaussian-splatting-with-uncertainty-aware-differentiable-optimization) | [2604.01030](https://arxiv.org/abs/2604.01030) | 为结合前馈模型快速推理和每场景优化高质量渲染的优势，本文提出Diff3R框架。 |

### 3.2 稀疏视角 {#cat-nvs-sparse}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-21 | [BALTIC](3dgs_2026-04.md#7-baltic-a-benchmark-and-cross-domain-strategy-for-3d-reconstruction-across-air-and-underwater-domains-under-varying-illumination) | [2604.19133](https://arxiv.org/abs/2604.19133) | 13 数据集跨空气/水下基准，白平衡校正 3DGS 匹配专用方法（v2 4/28 |
| 2026-04-30 | [Sparse-View in the Wild](3dgs_2026-04.md#8-sparse-view-3d-gaussian-splatting-in-the-wild) | [2604.27422](https://arxiv.org/abs/2604.27422) | 扩散引导伪视图+稀疏感知复制，野生稀疏视角合成 |
| 2026-04-27 | [SPAGS](3dgs_2026-04.md#7-spags-sparse-view-articulated-object-reconstruction-from-single-state-via-planar-gaussian-splatting) | [2511.17092](https://arxiv.org/abs/2511.17092) | 平面高斯稀疏重建少视角可变形物体（v2） |
| 2026-04-26 | [MarineSTD-GS](3dgs_2026-04.md#2-marinestd-gs-spatiotemporal-degradation-aware-3d-gaussian-splatting-for-realistic-underwater-scene-reconstruction) | [2604.23551](https://arxiv.org/abs/2604.23551) | 配对准退化高斯对，时空退化感知水下场景重建 |
| 2026-04-23 | ★ **[DualSplat](3dgs_2026-04.md#1-dualsplat-robust-3d-gaussian-splatting-via-pseudo-mask-bootstrapping-from-reconstruction-failures)** | [2604.21631](https://arxiv.org/abs/2604.21631) | 失败到先验框架，伪掩码引导瞬态场景重建（CVPR'26） |
| 2026-04-22 | [GSCompleter](3dgs_2026-04.md#1-gscompleter-a-distillation-free-plugin-for-metric-aware-3d-gaussian-splatting-completion-in-seconds) | [2604.20155](https://arxiv.org/abs/2604.20155) | "先生成后配准"工作流，秒级稀疏视角 3DGS 补全 |
| 2026-04-22 | [Dehaze-then-Splat](3dgs_2026-04.md#1-dehaze-then-splat-generative-dehazing-with-physics-informed-3d-gaussian-splatting-for-smoke-free-novel-view-synthesis) | [2604.13589](https://arxiv.org/abs/2604.13589) | 生成去雾+物理引导 3DGS 实现无烟新视角合成（v2） |
| 2026-04-22 | [3D Smoke Reconstruction](3dgs_2026-04.md#4-3d-smoke-scene-reconstruction-guided-by-vision-priors-from-multimodal-large-language-models) | [2604.05687](https://arxiv.org/abs/2604.05687) | 多模态视觉先验引导烟雾 3DGS 重建（v2） |
| 2026-04-21 | [SmokeGS-R](3dgs_2026-04.md#5-smokegs-r-physics-guided-pseudo-clean-3dgs-for-real-world-multi-view-smoke-restoration) | [2604.05301](https://arxiv.org/abs/2604.05301) | 物理引导伪清洁 3DGS 真实世界多视角烟雾恢复（v2） |
| 2026-04-21 | [SWAGSplatting](3dgs_2026-04.md#9-semantic-guided-gaussian-splatting-for-high-fidelity-underwater-scene-reconstruction) | [2509.00800](https://arxiv.org/abs/2509.00800) | 语义引导+自适应重分配，高保真水下 3DGS（v2） |
| 2026-04-15 | ★ **[PDF-GS](3dgs_2026-04.md#3-pdf-gs-progressive-distractor-filtering-for-robust-3d-gaussian-splatting)** | [2604.12580](https://arxiv.org/abs/2604.12580) | 渐进干扰过滤鲁棒重建（CVPR Findings'26） |
| 2026-04-09 | [SurfelSplat](3dgs_2026-04.md#2-surfelsplat-learning-efficient-and-generalizable-gaussian-surfel-representations-for-sparse-view-sur) | [2604.08370](https://arxiv.org/abs/2604.08370) | 针对现有3DGS表面重建方法需要密集输入视图和大量每场景优化的问题， |
| 2026-04-08 | [From Blobs to Spokes](3dgs_2026-04.md#1-from-blobs-to-spokes-high-fidelity-surface-reconstruction-via-oriented-gaussians) | [2604.07337](https://arxiv.org/abs/2604.07337) | 针对3DGS缺乏全局几何场导致表面提取困难的根本问题， |
| 2026-04-08 | [DOC-GS](3dgs_2026-04.md#3-doc-gs-dual-domain-observation-and-calibration-for-reliable-sparse-view-gaussian-splatting) | [2604.06739](https://arxiv.org/abs/2604.06739) | 针对稀疏视图3DGS重建中因几何监督不足导致的过拟合和伪影问题， |
| 2026-04-08 | [Physically Plausible Human-Object Rendering from Sparse V...](3dgs_2026-04.md#8-physically-plausible-human-object-rendering-from-sparse-views-via-3d-gaussian-splatting) | [2503.09640](https://arxiv.org/abs/2503.09640) | 针对稀疏视图下人物体交互渲染难以同时实现高质量、物理合理性和计算效率的问题， |
| 2026-04-08 | [Part$^{2}$GS](3dgs_2026-04.md#7-part2gs-part-aware-modeling-of-articulated-objects-using-3d-gaussian-splatting) | [2506.17212](https://arxiv.org/abs/2506.17212) | 针对铰接物体建模中结构和运动同时捕捉的挑战，本文提出Part^2GS框架。 |
| 2026-04-05 | [GA-GS](3dgs_2026-04.md#1-ga-gs-generation-assisted-gaussian-splatting-for-static-scene-reconstruction) | [2604.04331](https://arxiv.org/abs/2604.04331) | 针对含动态物体的单目视频中静态场景重建时遮挡区域难以恢复的问题，本文提出GA-G |
| 2026-04-03 | ★ **[ReWeaver](3dgs_2026-04.md#8-reweaver-towards-simulation-ready-and-topology-accurate-garment-reconstruction)** | [2601.16672](https://arxiv.org/abs/2601.16672) | 针对现有服装重建方法依赖非结构化表示难以提供准确服装拓扑和缝纫结构的问题，（CV |
| 2026-04-02 | [Learning Fine-Grained Geometry for Sparse-View Splatting ...](3dgs_2026-04.md#10-learning-fine-grained-geometry-for-sparse-view-splatting-via-cascade-depth-loss) | [2505.22279](https://arxiv.org/abs/2505.22279) | 针对稀疏视图条件下新视角合成质量急剧下降的问题，本文引入层次深度引导溅射框架HD |
| 2026-04-01 | ★ **[DirectFisheye-GS](3dgs_2026-04.md#6-directfisheye-gs-enabling-native-fisheye-input-in-gaussian-splatting-with-cross-view-joint-optimizat)** | [2604.00648](https://arxiv.org/abs/2604.00648) | 针对现有鱼眼相机3DGS方法先畸变校正再训练导致信息丢失和细节稀释的问题，（CV |

**概要**: 无需逐场景优化即可合成新视角（可泛化/前向方法），或从极少输入视角重建场景（稀疏视角方法）。

---

## 四、动态场景与 4D {#cat-dynamic-4d}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-30 | ★ **[FieryGS](3dgs_2026-04.md#2-fierygs-in-the-wild-fire-synthesis-with-physics-integrated-gaussian-splatting)** | [2605.00177](https://arxiv.org/abs/2605.00177) | 燃烧物理仿真与 3DGS 结合，逼真火焰合成（ICLR'26） |
| 2026-04-29 | [Color-Encoded Illumination](3dgs_2026-04.md#5-color-encoded-illumination-for-high-speed-volumetric-scene-reconstruction) | [2604.26920](https://arxiv.org/abs/2604.26920) | 颜色编码照明+动态 3DGS，首次实现多视角高速体场景重建 |
| 2026-04-28 | [Splatent](3dgs_2026-04.md#4-splatent-splatting-diffusion-latents-for-novel-view-synthesis) | [2512.09923](https://arxiv.org/abs/2512.09923) | VAE 隐空间 3DGS+扩散模型提升细节恢复（v2） |
| 2026-04-26 | ★ **[Egocentric Dynamic 3DGS](3dgs_2026-04.md#1-bringing-a-personal-point-of-view-evaluating-dynamic-3d-gaussian-splatting-for-egocentric-scene-reconstruction)** | [2604.23803](https://arxiv.org/abs/2604.23803) | 自视角动态 3DGS 质量评估，静态内容重建是瓶颈（CVPR'26 Worksh |
| 2026-04-26 | [D3DR](3dgs_2026-04.md#11-diffusion-models-are-secretly-zero-shot-3dgs-harmonizers) | [2503.06740](https://arxiv.org/abs/2503.06740) | 扩散模型隐式理解光照，零样本 3DGS 物体融合（v2） |
| 2026-04-25 | [ODE-GS](3dgs_2026-04.md#10-ode-gs-latent-odes-for-dynamic-scene-extrapolation-with-3d-gaussian-splatting) | [2506.05480](https://arxiv.org/abs/2506.05480) | 隐空间 ODEs 驱动 3DGS 实现动态场景未来外推（v2） |
| 2026-04-20 | [PhysMorph-GS](3dgs_2026-04.md#3-physmorph-gs-render-guided-volumetric-morphing-with-differentiable-physics) | [2511.16988](https://arxiv.org/abs/2511.16988) | 可微物理渲染引导体素形变，梯度注入变形梯度 |
| 2026-04-20 | [SemMorph3D](3dgs_2026-04.md#4-semmorph3d-unsupervised-semantic-aware-3d-morphing-via-mesh-guided-gaussians) | [2510.02034](https://arxiv.org/abs/2510.02034) | 无监督语义感知 3D 形变，网格引导+双流优化 |
| 2026-04-15 | ★ **[ClipGStream](3dgs_2026-04.md#2-clipgstream-clip-stream-gaussian-splatting-for-any-length-and-any-motion-multi-view-dynamic-scene-reconstruction)** | [2604.13746](https://arxiv.org/abs/2604.13746) | 混合流动态场景重建，任意长度视频（CVPR'26） |
| 2026-04-13 | [ArtifactWorld](3dgs_2026-04.md#1-artifactworld-scaling-3d-gaussian-splatting-artifact-restoration-via-video-generation-models) | [2604.12251](https://arxiv.org/abs/2604.12251) | 视频生成模型扩展 3DGS 伪影修复 |
| 2026-04-13 | ★ **[LumiMotion](3dgs_2026-04.md#8-lumimotion-improving-gaussian-relighting-with-scene-dynamics)** | [2604.10994](https://arxiv.org/abs/2604.10994) | 场景动态改进高斯重光照（CVPR'26） |
| 2026-04-13 | [STGV](3dgs_2026-04.md#10-stgv-spatio-temporal-hash-encoding-for-gaussian-based-video-representation) | [2604.10910](https://arxiv.org/abs/2604.10910) | 时空哈希编码高斯视频表示 |
| 2026-04-10 | [DynFOA](3dgs_2026-04.md#8-dynfoa-generating-first-order-ambisonics-with-conditional-diffusion-for-dynamic-and-acoustically-com) | [2604.02781](https://arxiv.org/abs/2604.02781) | 针对360度视频缺乏空间音频的问题，本文提出DynFOA框架， |
| 2026-04-06 | ★ **[PhysGaia](3dgs_2026-04.md#9-physgaia-a-physics-aware-benchmark-with-multi-body-interactions-for-dynamic-novel-view-synthesis)** | [2506.02794](https://arxiv.org/abs/2506.02794) | 针对动态新视角合成领域缺乏物理感知基准的问题，本文引入PhysGaia基准。（C |
| 2026-04-02 | [TrackerSplat](3dgs_2026-04.md#2-trackersplat-exploiting-point-tracking-for-fast-and-robust-dynamic-3d-gaussians-reconstruction) | [2604.02586](https://arxiv.org/abs/2604.02586) | 针对动态场景3DGS重建中大帧间位移导致伪影和时间不一致性的问题， |
| 2026-04-02 | [Resonance4D](3dgs_2026-04.md#3-resonance4d-frequency-domain-motion-supervision-for-preset-free-physical-parameter-learning-in-4d-dy) | [2604.01994](https://arxiv.org/abs/2604.01994) | 针对物理驱动的4D动态仿真中可靠的运动监督计算成本超过仿真器本身的问题， |

**概要**: 处理随时间变化的动态场景，包括 4D 高斯表示、动态表面重建、时序一致性、物理仿真、火焰合成、视频表示等。

---

## 五、语义分割与场景理解 {#cat-seg-understand}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-29 | ★ **[Semantic Foam](3dgs_2026-04.md#3-semantic-foam-unifying-spatial-and-semantic-scene-decomposition)** | [2604.26262](https://arxiv.org/abs/2604.26262) | Voronoi 网格语义分解，超越 Gaussian Grouping（CVPR |
| 2026-04-24 | [NRGS](3dgs_2026-04.md#3-nrgs-neural-regularization-for-robust-3d-semantic-gaussian-splatting) | [2604.22439](https://arxiv.org/abs/2604.22439) | 方差感知 MLP 校正 3D 语义场噪声，鲁棒 3D 语义高斯重建 |
| 2026-04-21 | [E3VS-Bench](3dgs_2026-04.md#8-e3vs-bench-a-benchmark-for-viewpoint-dependent-active-perception-in-3d-gaussian-splatting-scenes) | [2604.17969](https://arxiv.org/abs/2604.17969) | 99 个 3DGS 场景的 5-DoF  embodied 视觉搜索基准 |
| 2026-04-21 | [MAGICIAN](3dgs_2026-04.md#7-magician-efficient-long-term-planning-with-imagined-gaussians-for-active-mapping) | [2603.22650](https://arxiv.org/abs/2603.22650) | 想象高斯+树搜索实现主动建图长期规划（v2） |
| 2026-04-18 | [Instant Colorization](3dgs_2026-04.md#1-instant-colorization-of-gaussian-splats) | [2604.17155](https://arxiv.org/abs/2604.17155) | 最小二乘逆向颜色映射，实时光照变换和语义分割 |
| 2026-04-16 | ★ **[NG-GS](3dgs_2026-04.md#3-ng-gs-nerf-guided-3d-gaussian-splatting-segmentation)** | [2604.14706](https://arxiv.org/abs/2604.14706) | NeRF 边界引导 3DGS 分割（CVPR'26 Highlight） |
| 2026-04-14 | [BLaDA](3dgs_2026-04.md#8-blada-bridging-language-to-functional-dexterous-actions-within-3dgs-fields) | [2604.08410](https://arxiv.org/abs/2604.08410) | 语言到灵巧动作 3DGS 场桥梁，零样本功能操作 |
| 2026-04-13 | [GS4City](3dgs_2026-04.md#5-gs4city-hierarchical-semantic-gaussian-splatting-via-city-model-priors) | [2604.11401](https://arxiv.org/abs/2604.11401) | 城市语义高斯溅射，CityGML 先验融合 |
| 2026-04-13 | [ViserDex](3dgs_2026-04.md#7-viserdex-visual-sim-to-real-for-robust-dexterous-in-hand-reorientation) | [2604.11138](https://arxiv.org/abs/2604.11138) | 视觉 sim-to-real 灵巧手物体重定向 |
| 2026-04-12 | [Fast-SegSim](3dgs_2026-04.md#1-fast-segsim-real-time-open-vocabulary-segmentation-for-robotics-in-simulation) | [2604.10951](https://arxiv.org/abs/2604.10951) | 40FPS 实时开放词汇分割（ICRA'26） |
| 2026-04-10 | [Scene-Agnostic Object-Centric Representation Learning for...](3dgs_2026-04.md#4-scene-agnostic-object-centric-representation-learning-for-3d-gaussian-splatting) | [2604.09045](https://arxiv.org/abs/2604.09045) | 现有3D场景理解方法依赖2D视觉基础模型的掩码监督， |
| 2026-04-06 | [Indoor Asset Detection in Large Scale 360° Drone-Captured...](3dgs_2026-04.md#3-indoor-asset-detection-in-large-scale-360-drone-captured-imagery-via-3d-gaussian-splatting) | [2604.05316](https://arxiv.org/abs/2604.05316) | 针对大规模360度无人机图像中室内资产检测问题，本文提出基于3DGS的方法。 |
| 2026-04-05 | [FLEG](3dgs_2026-04.md#2-fleg-feed-forward-language-embedded-gaussian-splatting-from-any-views-via-compact-semantic-represent) | [2512.17541](https://arxiv.org/abs/2512.17541) | 针对现有前馈语言嵌入高斯重建方法受限于固定输入视图数量且每高斯附加语义嵌入导致冗 |
| 2026-04-01 | [LESV](3dgs_2026-04.md#2-lesv-language-embedded-sparse-voxel-fusion-for-open-vocabulary-3d-scene-understanding) | [2604.01388](https://arxiv.org/abs/2604.01388) | 针对基于3DGS的开放词汇3D场景理解方法中空间歧义和多层语义歧义的局限， |

**概要**: 3DGS 上的语义分割、开放词汇场景理解、语言 grounding、物体级提取、功能理解等。

---

## 六、视觉定位与安全 {#cat-visloc}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-17 | [Splats in Splats++](3dgs_2026-04.md#3-splats-in-splats-plus-plus-robust-and-generalizable-3d-gaussian-splatting-steganography) | [2604.15862](https://arxiv.org/abs/2604.15862) | SH 加密 3DGS 隐写术，3x 渲染加速 |
| 2026-04-14 | [DF3DV-1K](3dgs_2026-04.md#1-df3dv-1k-a-large-scale-dataset-and-benchmark-for-distractor-free-novel-view-synthesis) | [2604.13416](https://arxiv.org/abs/2604.13416) | 1048 场景干扰-free 新视角合成数据集 |
| 2026-04-14 | [PatchPoison](3dgs_2026-04.md#3-patchpoison-poisoning-multi-view-datasets-to-degrade-3d-reconstruction) | [2604.13153](https://arxiv.org/abs/2604.13153) | 高频对抗补丁破坏 3D 重建（CVPR Workshop'26） |
| 2026-04-09 | [RDSplat](3dgs_2026-04.md#5-rdsplat-robust-watermarking-for-3d-gaussian-splatting-against-2d-and-3d-diffusion-editing) | [2512.06774](https://arxiv.org/abs/2512.06774) | 针对现有3DGS水印方法在扩散编辑下失效的问题，本文提出RDSplat， |
| 2026-04-06 | [LSGS-Loc](3dgs_2026-04.md#1-lsgs-loc-towards-robust-3dgs-based-visual-localization-for-large-scale-uav-scenarios) | [2604.05402](https://arxiv.org/abs/2604.05402) | 针对大规模UAV场景下视觉定位中姿态初始化和渲染伪影敏感性的问题， |
| 2026-04-06 | ★ **[PR-IQA](3dgs_2026-04.md#6-pr-iqa-partial-reference-image-quality-assessment-for-diffusion-based-novel-view-synthesis)** | [2604.04576](https://arxiv.org/abs/2604.04576) | 针对扩散模型生成的稀疏视图新视角图像常存在光度与几何不一致性从而损害3D重建的问 |
| 2026-04-05 | ★ **[Can Protective Watermarking Safeguard the Copyright of 3D...](3dgs_2026-04.md#3-can-protective-watermarking-safeguard-the-copyright-of-3d-gaussian-splatting)** | [2511.22262](https://arxiv.org/abs/2511.22262) | 本文首次系统探索并验证了3DGS水印框架的可能脆弱性。（AAAI'26） |
| 2026-04-02 | [Satellite-Free Training for Drone-View Geo-Localization](3dgs_2026-04.md#6-satellite-free-training-for-drone-view-geo-localization) | [2604.01581](https://arxiv.org/abs/2604.01581) | 针对无人机地理定位方法依赖卫星图像训练导致卫星数据不可用时无法部署的问题， |

**概要**: 基于 3DGS 的视觉定位、图像质量评估、安全与水印、对抗攻击与隐写术等。

---

## 七、几何与表面重建 {#cat-geo-recon}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-30 | [Residual GS for CBCT](3dgs_2026-04.md#6-residual-gaussian-splatting-for-ultra-sparse-view-cbct-reconstruction) | [2604.27552](https://arxiv.org/abs/2604.27552) | 小波多分辨率+3DGS，超稀疏视角锥形束 CT 重建 |
| 2026-04-26 | [CryoSplat](3dgs_2026-04.md#10-cryosplat-gaussian-splatting-for-cryo-em-homogeneous-reconstruction) | [2508.04929](https://arxiv.org/abs/2508.04929) | 3DGS 适配冷冻电镜成像物理，高效同源重建（v2） |
| 2026-04-24 | [EvFlow-GS](3dgs_2026-04.md#2-evflow-gs-event-enhanced-motion-deblurring-with-optical-flow-for-3d-gaussian-splatting) | [2604.22183](https://arxiv.org/abs/2604.22183) | 事件流+光流联合优化运动去模糊（ICME'26） |
| 2026-04-23 | [PAGaS](3dgs_2026-04.md#4-pagas-pixel-aligned-1dof-gaussian-splatting-for-depth-refinement) | [2604.22129](https://arxiv.org/abs/2604.22129) | 单自由度像素对齐高斯，深度作为唯一优化自由度，提升多视图深度精度 |
| 2026-04-22 | [Confidence Mesh](3dgs_2026-04.md#6-confidence-based-mesh-extraction-from-3d-gaussians) | [2603.24725](https://arxiv.org/abs/2603.24725) | 自监督置信度框架动态平衡光度与几何监督（v2） |
| 2026-04-21 | [OT-UVGS](3dgs_2026-04.md#6-ot-uvgs-revisiting-uv-mapping-for-gaussian-splatting-as-a-capacity-allocation-problem) | [2604.19127](https://arxiv.org/abs/2604.19127) | 最优传输 UV 映射替代确定性球面投影，提升 UVGS 容量利用率 |
| 2026-04-17 | ★ **[Neural Gabor Splatting](3dgs_2026-04.md#2-neural-gabor-splatting-enhanced-gaussian-splatting-with-neural-gabor-for-high-frequency-surface-reconstruction)** | [2604.15941](https://arxiv.org/abs/2604.15941) | 神经 Gabor 增强高频表面重建（CVPR'26） |
| 2026-04-14 | [MSGS](3dgs_2026-04.md#4-msgs-multispectral-3d-gaussian-splatting) | [2604.13340](https://arxiv.org/abs/2604.13340) | 多光谱 3DGS，per-band 球面谐波（ISMAR'25 Adjunct） |
| 2026-04-14 | [MedGS](3dgs_2026-04.md#10-medgs-gaussian-splatting-for-multi-modal-3d-medical-imaging) | [2509.16806](https://arxiv.org/abs/2509.16806) | 多模态 3D 医学成像高斯溅射 |
| 2026-04-13 | [VVGT](3dgs_2026-04.md#2-vvgt-visual-volume-grounded-transformer) | [2604.12217](https://arxiv.org/abs/2604.12217) | 视觉体素 Transformer，体数据直接到 3DGS |
| 2026-04-13 | [Dark-EvGS](3dgs_2026-04.md#11-dark-evgs-event-camera-as-an-eye-for-radiance-field-in-the-dark) | [2507.11931](https://arxiv.org/abs/2507.11931) | 事件相机暗光辐射场重建 |
| 2026-04-10 | [MASS](3dgs_2026-04.md#6-mass-mesh-inellipse-aligned-deformable-surfel-splatting-for-hand-reconstruction-and-rendering-from-e) | [2604.08943](https://arxiv.org/abs/2604.08943) | 针对以自我为中心的视角下从单目视频重建高保真3D手部的挑战，本文提出MASS方法 |
| 2026-04-08 | [4D Vessel Reconstruction for Benchtop Thrombectomy Analysis](3dgs_2026-04.md#4-4d-vessel-reconstruction-for-benchtop-thrombectomy-analysis) | [2604.06671](https://arxiv.org/abs/2604.06671) | 针对桌面血栓切除术研究中缺乏时间分辨的全场3D血管运动测量的问题， |
| 2026-04-08 | [Neural Harmonic Textures for High-Quality Primitive Based...](3dgs_2026-04.md#5-neural-harmonic-textures-for-high-quality-primitive-based-neural-reconstruction) | [2604.01204](https://arxiv.org/abs/2604.01204) | 针对3DGS等基于图元的方法中单个图元表达能力有限导致高频细节建模困难的问题， |
| 2026-04-08 | ★ **[BrepGaussian](3dgs_2026-04.md#6-brepgaussian-cad-reconstruction-from-multi-view-images-with-gaussian-splatting)** | [2602.21105](https://arxiv.org/abs/2602.21105) | 针对从不规则数据恢复边界表示（B-Rep）的挑战性任务，（CVPR'26） |
| 2026-04-06 | [3D Gaussian Splatting for Annular Dark Field Scanning Tra...](3dgs_2026-04.md#5-3d-gaussian-splatting-for-annular-dark-field-scanning-transmission-electron-microscopy-tomography-re) | [2604.04693](https://arxiv.org/abs/2604.04693) | 针对ADF-STEM层析成像中稀疏视图下常规方法退化严重的问题， |
| 2026-04-04 | [2D Triangle Splatting for Direct Differentiable Mesh Trai...](3dgs_2026-04.md#3-2d-triangle-splatting-for-direct-differentiable-mesh-training) | [2506.18575](https://arxiv.org/abs/2506.18575) | 针对3DGS在渲染速度和高级渲染效果（如重光照和阴影）方面不如基于网格模型的问题 |
| 2026-04-04 | ★ **[CGHair](3dgs_2026-04.md#2-cghair-compact-gaussian-hair-reconstruction-with-card-clustering)** | [2604.03716](https://arxiv.org/abs/2604.03716) | 针对3DGS头发重建需要数百万图元导致存储和渲染成本高昂的问题，（CVPR'26 |
| 2026-04-02 | [GVGS](3dgs_2026-04.md#9-gvgs-gaussian-visibility-aware-multi-view-geometry-for-accurate-surface-reconstruction) | [2601.20331](https://arxiv.org/abs/2601.20331) | 针对3DGS表面重建中可见性估计需要准确深度而深度监督本身又条件于可见性的循环依 |
| 2026-04-01 | [Geometric-Photometric Event-based 3D Gaussian Ray Tracing](3dgs_2026-04.md#10-geometric-photometric-event-based-3d-gaussian-ray-tracing) | [2512.18640](https://arxiv.org/abs/2512.18640) | 针对事件相机3DGS方法如何有效利用稀疏事件细粒度时间信息的问题，本文提出GPE |

**概要**: 从图像重建几何准确的表面、网格或点云，包括表面光栅化、高频细节恢复、CAD 重建、医学/科学成像等。

---

## 八、生成式模型 {#cat-generative}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-21 | [TransSplat](3dgs_2026-04.md#3-transsplat-unbalanced-semantic-transport-for-language-driven-3dgs-editing) | [2604.19571](https://arxiv.org/abs/2604.19571) | 语言驱动编辑建模为非平衡语义传输，跨视角一致性（v2 4/29） |
| 2026-04-25 | [ConsDreamer](3dgs_2026-04.md#11-consdreamer-advancing-multi-view-consistency-for-zero-shot-text-to-3d-generation) | [2504.02316](https://arxiv.org/abs/2504.02316) | 视角解耦+一致性损失，零样本文本 3D 生成（v2） |
| 2026-04-21 | [FluSplat](3dgs_2026-04.md#2-flusplat-sparse-view-3d-editing-without-test-time-optimization) | [2604.20038](https://arxiv.org/abs/2604.20038) | 前向 3D 场景编辑，跨视角正则化消除逐场景优化 |
| 2026-04-19 | [R3D2](3dgs_2026-04.md#1-r3d2-realistic-3d-asset-insertion-via-diffusion-for-autonomous-driving-simulation) | [2506.07826](https://arxiv.org/abs/2506.07826) | 扩散模型逼真 3D 资产插入，跨场景阴影生成 |
| 2026-04-15 | [HY-World 2.0](3dgs_2026-04.md#1-hy-world-2-0-a-multi-modal-world-model-for-reconstructing-generating-and-simulating-3d-worlds) | [2604.14268](https://arxiv.org/abs/2604.14268) | 腾讯多模态世界模型，文本/图像/视频到 3D |
| 2026-04-14 | [Rein3D](3dgs_2026-04.md#7-rein3d-reinforced-3d-indoor-scene-generation-with-panoramic-video-diffusion-models) | [2604.10578](https://arxiv.org/abs/2604.10578) | 全景视频扩散强化 3D 室内生成 |
| 2026-04-12 | [FreeScale](3dgs_2026-04.md#3-freescale-scaling-3d-scenes-via-certainty-aware-free-view-generation) | [2604.10512](https://arxiv.org/abs/2604.10512) | 确定性感知自由视图生成扩展 3D 场景（CVPR'26） |
| 2026-04-09 | [SIC3D](3dgs_2026-04.md#1-sic3d-style-image-conditioned-text-to-3d-gaussian-splatting-generation) | [2604.08760](https://arxiv.org/abs/2604.08760) | 针对文本到3D生成方法受限于文本模态导致可控性差和纹理模糊的问题，本文提出SIC |
| 2026-04-07 | ★ **[GaussianGrow](3dgs_2026-04.md#3-gaussiangrow-geometry-aware-gaussian-growing-from-3d-point-clouds-with-text-guidance)** | [2604.05721](https://arxiv.org/abs/2604.05721) | 针对3D高斯生成中几何先验不足的问题，本文提出GaussianGrow方法，（C |
| 2026-04-06 | [DreamLifting](3dgs_2026-04.md#8-dreamlifting-a-plug-in-module-lifting-mv-diffusion-models-for-3d-asset-generation) | [2509.07435](https://arxiv.org/abs/2509.07435) | 针对现有3D生成方法多关注几何建模而将纹理合成留给后处理的问题， |
| 2026-04-01 | [ARGS](3dgs_2026-04.md#7-args-auto-regressive-gaussian-splatting-via-parallel-progressive-next-scale-prediction) | [2604.00494](https://arxiv.org/abs/2604.00494) | 将2D图像的自回归下一尺度预测范式扩展到3D物体生成领域，本文提出ARGS框架。 |

**概要**: 使用扩散模型、自回归模型等生成式方法生成或编辑 3DGS 场景，包括文本到 3D、图像到 3D、3D 编辑等。

---

## 九、流媒体与编码 {#cat-streaming}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-29 | [URF-GS](3dgs_2026-04.md#3-bridging-visual-and-wireless-sensing-via-a-unified-radiation-field-for-3d-radio-map-construction) | [2601.19216](https://arxiv.org/abs/2601.19216) | 统一辐射场 3DGS 构建 3D 无线电地图（v2） |
| 2026-04-28 | [Semantic Coding for 3DGS](3dgs_2026-04.md#2-generalizable-3d-gaussian-splatting-enabled-semantic-coding-for-real-time-immersive-video-communications) | [2604.25330](https://arxiv.org/abs/2604.25330) | 可泛化 3DGS 与语义编码统一，实时沉浸式视频通信 |
| 2026-04-27 | [GSpaRC](3dgs_2026-04.md#6-gsparc-gaussian-splatting-for-real-time-reconstruction-of-rf-channels) | [2511.22793](https://arxiv.org/abs/2511.22793) | 3DGS 实现毫秒级射频信道实时重建（v2） |
| 2026-04-22 | [Aerial Transceiver](3dgs_2026-04.md#3-efficient-transceiver-design-for-aerial-image-transmission-and-large-scale-scene-reconstruction) | [2604.11098](https://arxiv.org/abs/2604.11098) | 端到端收发机+3DGS 联合优化空中影像传输（v2） |
| 2026-04-17 | [BiSplat-WRF](3dgs_2026-04.md#1-bisplat-wrf-planar-gaussian-splatting-with-bilinear-spatial-transformer-for-wireless-radiance-field-reconstruction) | [2604.25945](https://arxiv.org/abs/2604.25945) | 平面高斯无线辐射场重建（IEEE ICC'26 Workshop） |
| 2026-04-10 | [AudioGS](3dgs_2026-04.md#5-audiogs-spectrogram-based-audio-gaussian-splatting-for-sound-field-reconstruction) | [2604.08967](https://arxiv.org/abs/2604.08967) | 针对稀疏观测下高保真双耳音频合成的挑战，本文提出AudioGS方法，灵感来源于3 |
| 2026-04-03 | [Streaming Real-Time Rendered Scenes as 3D Gaussians](3dgs_2026-04.md#4-streaming-real-time-rendered-scenes-as-3d-gaussians) | [2604.02851](https://arxiv.org/abs/2604.02851) | 针对云渲染系统通常将场景作为2D视频流传输导致内容与服务器渲染视角紧密耦合的问题 |

**概要**: 3DGS 场景或动态 3DGS 的视频编码、流式传输、带宽优化和无线传感融合。

---

## 十、SLAM 与建图 {#cat-slam}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-24 | [Flow4DGS-SLAM](3dgs_2026-04.md#1-flow4dgs-slam-optical-flow-guided-4d-gaussian-splatting-slam) | [2604.22339](https://arxiv.org/abs/2604.22339) | 光流引导动态 4DGS SLAM，动态/静态高斯分解 SOTA（v2 4/28） |
| 2026-04-21 | [RMGS-SLAM](3dgs_2026-04.md#2-rmgs-slam-real-time-multi-sensor-gaussian-splatting-slam) | [2604.12942](https://arxiv.org/abs/2604.12942) | 激光-惯性-视觉紧耦合 3DGS SLAM 实时稠密建图（v2） |
| 2026-04-14 | [GGD-SLAM](3dgs_2026-04.md#5-ggd-slam-monocular-3dgs-slam-powered-by-generalizable-motion-model-for-dynamic-environments) | [2604.12837](https://arxiv.org/abs/2604.12837) | 动态环境单目 3DGS SLAM（ICRA'26） |
| 2026-04-13 | [ReefMapGS](3dgs_2026-04.md#3-reefmapgs-enabling-large-scale-underwater-reconstruction-by-closing-the-loop-between-multimodal-slam-and-gaussian-splatting) | [2604.11992](https://arxiv.org/abs/2604.11992) | 多模态 SLAM 闭环大规模水下高斯重建 |
| 2026-04-13 | [Ψ-Map](3dgs_2026-04.md#9-map-panoptic-surface-integrated-mapping-enables-real2sim-transfer) | [2604.10982](https://arxiv.org/abs/2604.10982) | 全景表面集成映射，Real2Sim 迁移 |
| 2026-04-03 | [Flash-Mono](3dgs_2026-04.md#2-flash-mono-feed-forward-accelerated-gaussian-splatting-monocular-slam) | [2604.03092](https://arxiv.org/abs/2604.03092) | 针对单目3DGS SLAM在时间效率、几何精度和多视图一致性方面的限制， |
| 2026-04-02 | [VBGS-SLAM](3dgs_2026-04.md#1-vbgs-slam-variational-bayesian-gaussian-splatting-simultaneous-localization-and-mapping) | [2604.02696](https://arxiv.org/abs/2604.02696) | 针对现有3DGS SLAM变体对初始化敏感且随着地图演化容易灾难性遗忘的问题， |
| 2026-04-02 | [F3DGS](3dgs_2026-04.md#5-f3dgs-federated-3d-gaussian-splatting-for-decentralized-multi-agent-world-modeling) | [2604.01605](https://arxiv.org/abs/2604.01605) | 针对多智能体分布式场景中集中式3DGS管线的通信开销和几何不一致问题， |
| 2026-04-01 | [Compact Keyframe-Optimized Multi-Agent Gaussian Splatting...](3dgs_2026-04.md#5-compact-keyframe-optimized-multi-agent-gaussian-splatting-slam) | [2604.00804](https://arxiv.org/abs/2604.00804) | 针对多智能体SLAM中大规模高斯地图在受限带宽下共享成为瓶颈的问题， |

**概要**: 基于 3DGS 的 SLAM 系统、主动建图、多智能体建图、水下/城市场景大规模建图等。

---

## 十一、机器人与仿真 {#cat-robot-sim}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-30 | [GSDrive](3dgs_2026-04.md#3-gsdrive-reinforcing-driving-policies-by-multi-mode-future-trajectory-probing-with-3d-gaussian-splatting-environment) | [2604.28111](https://arxiv.org/abs/2604.28111) | 可微 3DGS 环境强化学习驾驶策略，循环 IL-RL 训练 |
| 2026-04-28 | ★ **[GS-Playground](3dgs_2026-04.md#1-gs-playground-a-high-throughput-photorealistic-simulator-for-vision-informed-robot-learning)** | [2604.25459](https://arxiv.org/abs/2604.25459) | 批量 3DGS 渲染万 FPS，机器人学习高吞吐仿真器（RSS'26） |
| 2026-04-21 | [Mobile Object-Centered Capture](3dgs_2026-04.md#4-an-object-centered-data-acquisition-method-for-3d-gaussian-splatting-using-mobile-phones) | [2604.19216](https://arxiv.org/abs/2604.19216) | 手机端以物为中心采集，实时球面覆盖引导用户运动 |
| 2026-04-18 | [LAGS](3dgs_2026-04.md#2-lags-low-altitude-gaussian-splatting-with-groupwise-heterogeneous-graph-learning) | [2604.16910](https://arxiv.org/abs/2604.16910) | 异构图神经网络低空资源分配，100x 延迟降低 |
| 2026-04-15 | [LIVE-GS](3dgs_2026-04.md#4-live-gs-llm-powers-interactive-vr-experience-with-physics-aware-gaussian-splatting) | [2412.09176](https://arxiv.org/abs/2412.09176) | LLM 驱动物理感知 VR 高斯资产创建 |
| 2026-04-14 | [Habitat-GS](3dgs_2026-04.md#6-habitat-gs-a-high-fidelity-navigation-simulator-with-dynamic-gaussian-splatting) | [2604.12626](https://arxiv.org/abs/2604.12626) | 高保真导航模拟器，动态高斯+可驱动头像 |
| 2026-04-06 | [GaussFly](3dgs_2026-04.md#4-gaussfly-contrastive-reinforcement-learning-for-visuomotor-policies-in-3d-gaussian-fields) | [2604.05062](https://arxiv.org/abs/2604.05062) | 针对自主飞行器仅依赖单目视觉的端到端策略学习中样本效率低和sim-to-real |

**概要**: 基于 3DGS 的机器人仿真器、导航规划、视觉-动作策略学习和高吞吐渲染。

---

## 十二、数字人与人体重建 {#cat-avatar-human}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-28 | [Generalizable Human GS](3dgs_2026-04.md#3-generalizable-human-gaussian-splatting-via-multi-view-semantic-consistency) | [2604.25466](https://arxiv.org/abs/2604.25466) | 跨视角注意力校正人体部位特征，稀疏视角可泛化人体高斯重建 |
| 2026-04-26 | [ISExplore](3dgs_2026-04.md#9-isexplore-informative-segment-selection-for-efficient-personalized-3d-talking-face-generation) | [2511.07940](https://arxiv.org/abs/2511.07940) | 自动选择最有价值参考片段，5 倍加速 3D 说人脸生成（v2） |
| 2026-04-21 | ★ **[SketchFaceGS](3dgs_2026-04.md#5-sketchfacegs-real-time-sketch-driven-face-editing-and-generation-with-gaussian-splatting)** | [2604.19202](https://arxiv.org/abs/2604.19202) | 草图驱动 3D 人脸生成与编辑，实时 UV 特征预测（CVPR'26 Highl |
| 2026-04-20 | [High-Fidelity 3D Human GS](3dgs_2026-04.md#1-high-fidelity-3d-gaussian-human-reconstruction-via-region-aware-initialization-and-geometric-priors) | [2604.21714](https://arxiv.org/abs/2604.21714) | SMPL-X 初始化+区域感知密度控制，高保真实时人体重建 |
| 2026-04-16 | [Compositional 3D Head Avatars](3dgs_2026-04.md#2-one-shot-compositional-3d-head-avatars-with-deformable-hair) | [2604.14782](https://arxiv.org/abs/2604.14782) | 单图 3D 人头，毛发-面部解耦+PBD 物理仿真 |
| 2026-04-11 | [Real-Time Human Animation](3dgs_2026-04.md#1-real-time-human-reconstruction-and-animation-using-feed-forward-gaussian-splatting) | [2604.10259](https://arxiv.org/abs/2604.10259) | 前馈高斯溅射实时人体重建与动画 |
| 2026-04-11 | [AvatarPointillist](3dgs_2026-04.md#4-avatarpointillist-autoregressive-4d-gaussian-avatarization) | [2604.04787](https://arxiv.org/abs/2604.04787) | 自回归 4D 高斯头像生成（CVPR'26） |
| 2026-04-10 | [F3G-Avatar](3dgs_2026-04.md#2-f3g-avatar-face-focused-full-body-gaussian-avatar) | [2604.09835](https://arxiv.org/abs/2604.09835) | 现有全身高斯数字人在面部细节重建上表现不佳，本文提出F3G-Avatar方法。 |
| 2026-04-10 | [Structure-Aware Fine-Grained Gaussian Splatting for Expre...](3dgs_2026-04.md#3-structure-aware-fine-grained-gaussian-splatting-for-expressive-avatar-reconstruction) | [2604.09324](https://arxiv.org/abs/2604.09324) | 针对单目视频重建人体数字人时手部动作和面部表情等细节难以精确建模的问题， |
| 2026-04-07 | ★ **[Rendering Multi-Human and Multi-Object with 3D Gaussian S...](3dgs_2026-04.md#5-rendering-multi-human-and-multi-object-with-3d-gaussian-splatting)** | [2604.02996](https://arxiv.org/abs/2604.02996) | 针对稀疏视图中多人与多物体交互场景重建的挑战，本文提出MM-GS层次化框架。（I |
| 2026-04-03 | [UNICA](3dgs_2026-04.md#6-unica-a-unified-neural-framework-for-controllable-3d-avatars) | [2604.02799](https://arxiv.org/abs/2604.02799) | 针对创建可控3D人体数字人需要冗长管线的痛点，本文提出UNICA， |
| 2026-04-02 | [Better Rigs, Not Bigger Networks](3dgs_2026-04.md#7-better-rigs-not-bigger-networks-a-body-model-ablation-for-gaussian-avatars) | [2604.01447](https://arxiv.org/abs/2604.01447) | 针对基于SMPL的3DGS数字人方法不断增加训练架构复杂度的趋势， |
| 2026-04-01 | [Autoregressive Appearance Prediction for 3D Gaussian Avatars](3dgs_2026-04.md#4-autoregressive-appearance-prediction-for-3d-gaussian-avatars) | [2604.00928](https://arxiv.org/abs/2604.00928) | 针对相似姿态对应不同外观导致数字人模型过拟合和产生不稳定外观变化的问题， |

**概要**: 3DGS 人体/头像重建、数字人生成与动画、手部重建、面部编辑等。

---

## 十三、风格迁移与编辑 {#cat-style-edit}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-09 | [ReconPhys](3dgs_2026-04.md#3-reconphys-reconstruct-appearance-and-physical-attributes-from-single-video) | [2604.07882](https://arxiv.org/abs/2604.07882) | 针对非刚性物体物理重建的挑战，本文提出ReconPhys， |
| 2026-04-04 | [M2StyleGS](3dgs_2026-04.md#1-m2stylegs-multi-modality-3d-style-transfer-with-gaussian-splatting) | [2604.03773](https://arxiv.org/abs/2604.03773) | 针对传统3D风格迁移方法依赖固定参考图像而缺乏灵活性的问题， |
| 2026-04-01 | [ColorGradedGaussians](3dgs_2026-04.md#1-colorgradedgaussians-palette-based-color-grading-for-3d-gaussian-splatting-via-view-space-sparse-dec) | [2604.01551](https://arxiv.org/abs/2604.01551) | 针对现有基于调色板的3DGS颜色编辑方法在图元级别分解导致像素级编辑影响非预期区 |
| 2026-04-01 | [Thinking Like Van Gogh](3dgs_2026-04.md#9-thinking-like-van-gogh-structure-aware-style-transfer-via-flow-guided-3d-gaussian-splatting) | [2601.10075](https://arxiv.org/abs/2601.10075) | 为真实再现后印象派风格化中放大结构形式同时抑制摄影细节的核心原则， |

**概要**: 3DGS 风格迁移、颜色编辑、3D 场景编辑和物理属性重建。

---

## 十四、领域应用 {#cat-domain-special}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-04-30 | [Fake3DGS](3dgs_2026-04.md#5-fake3dgs-a-benchmark-for-3d-manipulation-detection-in-neural-rendering) | [2604.27590](https://arxiv.org/abs/2604.27590) | 首个 3DGS 操控检测基准，3D 感知多视角一致性检测 |
| 2026-04-13 | [MetroGS](3dgs_2026-04.md#12-metrogs-efficient-and-stable-reconstruction-of-geometrically-accurate-high-fidelity-large-scale-scenes) | [2511.19172](https://arxiv.org/abs/2511.19172) | 高效稳定大规模城市场景重建（CVPR'26） |
| 2026-04-12 | [UniSplat](3dgs_2026-04.md#2-unisplat-learning-3d-representations-for-spatial-intelligence-from-unposed-multi-view-images) | [2604.10573](https://arxiv.org/abs/2604.10573) | 无位姿多视图 3D 表示学习（CVPR'26） |
| 2026-04-10 | [Generative 3D Gaussian Splatting for Arbitrary-Resolution...](3dgs_2026-04.md#7-generative-3d-gaussian-splatting-for-arbitrary-resolution-atmospheric-downscaling-and-forecasting) | [2604.07928](https://arxiv.org/abs/2604.07928) | 针对AI数值天气预报中高分辨率输出计算成本高的问题，本文提出GSSA-ViT框架 |
| 2026-04-10 | ★ **[ProDiG](3dgs_2026-04.md#9-prodig-progressive-diffusion-guided-gaussian-splatting-for-aerial-to-ground-reconstruction)** | [2604.02003](https://arxiv.org/abs/2604.02003) | 针对仅从航空图像生成地面级视图和连贯3D站点的极端视角变化挑战，本文提出ProD |
| 2026-04-10 | [LoBE-GS](3dgs_2026-04.md#10-lobe-gs-load-balanced-and-efficient-3d-gaussian-splatting-for-large-scale-scene-reconstruction) | [2510.01767](https://arxiv.org/abs/2510.01767) | 针对将3DGS扩展到城市街区级大规模场景时分区负载不平衡和粗到细管线效率低的问题 |
| 2026-04-07 | [GS-Surrogate](3dgs_2026-04.md#2-gs-surrogate-deformable-gaussian-splatting-for-parameter-space-exploration-of-ensemble-simulations) | [2604.06358](https://arxiv.org/abs/2604.06358) | 针对集合仿真参数空间探索中原始数据存储代价高昂的问题，本文提出GS-Surrog |
| 2026-04-03 | ★ **[Scene Grounding In the Wild](3dgs_2026-04.md#7-scene-grounding-in-the-wild)** | [2603.26584](https://arxiv.org/abs/2603.26584) | 针对从非结构化自然图像重建大规模真实世界场景时输入视图缺乏重叠导致全局对齐失败的 |

**概要**: 3DGS 在特定领域的应用，包括大气下推、城市级重建、大规模场景、伪造检测、科学仿真等。

---

## v2 版本更新论文

> 以下论文在 4 月期间发布了 v2 版本更新，已归入上方对应类别。此处按更新时间列出。

### 4/26-30 v2 更新 {#v2-426-30}

| 更新日期 | 论文 | arXiv | 说明 |
|------|------|-------|------|
| 2026-04-30 | [SDDF](3dgs_2026-04.md#1-sddf-learning-scene-level-signed-directional-distance-function-with-ellipsoidal-priors-and-neural-residuals) | [2503.20066v2](https://arxiv.org/abs/2503.20066) | 符号方向距离函数+椭球先验，高效几何重建（v2） |
| 2026-04-29 | [Deformation Overfitting](3dgs_2026-04.md#2-incoherent-deformation-not-capacity-diagnosing-and-mitigating-overfitting-in-dynamic-gaussian-splatting) | [2604.16747v2](https://arxiv.org/abs/2604.16747) | 诊断动态 3DGS 过拟合，弹性正则化+稀疏化降阈值（v2） |
| 2026-04-29 | [URF-GS](3dgs_2026-04.md#3-bridging-visual-and-wireless-sensing-via-a-unified-radiation-field-for-3d-radio-map-construction) | [2601.19216v2](https://arxiv.org/abs/2601.19216) | 统一辐射场 3DGS 构建 3D 无线电地图（v2） |
| 2026-04-28 | [Splatent](3dgs_2026-04.md#4-splatent-splatting-diffusion-latents-for-novel-view-synthesis) | [2512.09923v2](https://arxiv.org/abs/2512.09923) | VAE 隐空间 3DGS+扩散模型提升细节恢复（v2） |
| 2026-04-28 | [C3G](3dgs_2026-04.md#5-c3g-learning-compact-3d-representations-with-2k-gaussians) | [2512.04021v2](https://arxiv.org/abs/2512.04021) | 紧凑 3DGS 仅 2K 高斯实现高效场景重建（v2） |
| 2026-04-27 | [GSpaRC](3dgs_2026-04.md#6-gsparc-gaussian-splatting-for-real-time-reconstruction-of-rf-channels) | [2511.22793v2](https://arxiv.org/abs/2511.22793) | 3DGS 实现毫秒级射频信道实时重建（v2） |
| 2026-04-27 | [SPAGS](3dgs_2026-04.md#7-spags-sparse-view-articulated-object-reconstruction-from-single-state-via-planar-gaussian-splatting) | [2511.17092v2](https://arxiv.org/abs/2511.17092) | 平面高斯稀疏重建少视角可变形物体（v2） |
| 2026-04-27 | [Genie Sim PanoRecon](3dgs_2026-04.md#8-genie-sim-panorecon-fast-immersive-scene-generation-from-single-view-panorama) | [2604.07105v2](https://arxiv.org/abs/2604.07105) | 前馈 3DGS 快速从全景图生成 3D 场景（v2） |
| 2026-04-26 | [ISExplore](3dgs_2026-04.md#9-isexplore-informative-segment-selection-for-efficient-personalized-3d-talking-face-generation) | [2511.07940v2](https://arxiv.org/abs/2511.07940) | 自动选择最有价值参考片段，5 倍加速 3D 说人脸生成（v2） |
| 2026-04-26 | [CryoSplat](3dgs_2026-04.md#10-cryosplat-gaussian-splatting-for-cryo-em-homogeneous-reconstruction) | [2508.04929v2](https://arxiv.org/abs/2508.04929) | 3DGS 适配冷冻电镜成像物理，高效同源重建（v2） |
| 2026-04-26 | [D3DR](3dgs_2026-04.md#11-diffusion-models-are-secretly-zero-shot-3dgs-harmonizers) | [2503.06740v2](https://arxiv.org/abs/2503.06740) | 扩散模型隐式理解光照，零样本 3DGS 物体融合（v2） |

### 4/21-25 v2 更新 {#v2-421-25}

| 更新日期 | 论文 | arXiv | 说明 |
|------|------|-------|------|
| 2026-04-25 | [ODE-GS](3dgs_2026-04.md#10-ode-gs-latent-odes-for-dynamic-scene-extrapolation-with-3d-gaussian-splatting) | [2506.05480v2](https://arxiv.org/abs/2506.05480) | 隐空间 ODEs 驱动 3DGS 实现动态场景未来外推（v2） |
| 2026-04-25 | [ConsDreamer](3dgs_2026-04.md#11-consdreamer-advancing-multi-view-consistency-for-zero-shot-text-to-3d-generation) | [2504.02316v2](https://arxiv.org/abs/2504.02316) | 视角解耦+一致性损失，零样本文本 3D 生成（v2） |
| 2026-04-22 | [Dehaze-then-Splat](3dgs_2026-04.md#1-dehaze-then-splat-generative-dehazing-with-physics-informed-3d-gaussian-splatting-for-smoke-free-novel-view-synthesis) | [2604.13589v2](https://arxiv.org/abs/2604.13589) | 生成去雾+物理引导 3DGS 实现无烟新视角合成（v2） |
| 2026-04-22 | [Aerial Transceiver](3dgs_2026-04.md#3-efficient-transceiver-design-for-aerial-image-transmission-and-large-scale-scene-reconstruction) | [2604.11098v2](https://arxiv.org/abs/2604.11098) | 端到端收发机+3DGS 联合优化空中影像传输（v2） |
| 2026-04-22 | [3D Smoke Reconstruction](3dgs_2026-04.md#4-3d-smoke-scene-reconstruction-guided-by-vision-priors-from-multimodal-large-language-models) | [2604.05687v2](https://arxiv.org/abs/2604.05687) | 多模态视觉先验引导烟雾 3DGS 重建（v2） |
| 2026-04-22 | [Confidence Mesh](3dgs_2026-04.md#6-confidence-based-mesh-extraction-from-3d-gaussians) | [2603.24725v2](https://arxiv.org/abs/2603.24725) | 自监督置信度框架动态平衡光度与几何监督（v2） |
| 2026-04-22 | [Init vs Densification](3dgs_2026-04.md#8-the-role-and-relationship-of-initialization-and-densification-in-3d-gaussian-splatting) | [2603.20714v2](https://arxiv.org/abs/2603.20714) | 系统研究 3DGS 初始化与加密的关系（v2） |
| 2026-04-21 | [RMGS-SLAM](3dgs_2026-04.md#2-rmgs-slam-real-time-multi-sensor-gaussian-splatting-slam) | [2604.12942v2](https://arxiv.org/abs/2604.12942) | 激光-惯性-视觉紧耦合 3DGS SLAM 实时稠密建图（v2） |
| 2026-04-21 | [SmokeGS-R](3dgs_2026-04.md#5-smokegs-r-physics-guided-pseudo-clean-3dgs-for-real-world-multi-view-smoke-restoration) | [2604.05301v2](https://arxiv.org/abs/2604.05301) | 物理引导伪清洁 3DGS 真实世界多视角烟雾恢复（v2） |
| 2026-04-21 | [MAGICIAN](3dgs_2026-04.md#7-magician-efficient-long-term-planning-with-imagined-gaussians-for-active-mapping) | [2603.22650v2](https://arxiv.org/abs/2603.22650) | 想象高斯+树搜索实现主动建图长期规划（v2） |
| 2026-04-21 | [SWAGSplatting](3dgs_2026-04.md#9-semantic-guided-gaussian-splatting-for-high-fidelity-underwater-scene-reconstruction) | [2509.00800v2](https://arxiv.org/abs/2509.00800) | 语义引导+自适应重分配，高保真水下 3DGS（v2） |

---

## 统计概览

| 类别 | 论文数 |
|------|--------|
| 一、核心算法与优化 | 16 |
| 二、渲染加速与压缩 | 17 |
| 3.1 可泛化 / 前向 | 8 |
| 3.2 稀疏视角 | 20 |
| 四、动态场景与 4D | 16 |
| 五、语义分割与场景理解 | 14 |
| 六、视觉定位与安全 | 8 |
| 七、几何与表面重建 | 20 |
| 八、生成式模型 | 11 |
| 九、流媒体与编码 | 7 |
| 十、SLAM 与建图 | 9 |
| 十一、机器人与仿真 | 7 |
| 十二、数字人与人体重建 | 13 |
| 十三、风格迁移与编辑 | 4 |
| 十四、领域应用 | 8 |
| **合计** | **178** |
