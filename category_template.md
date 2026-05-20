# 3D Gaussian Splatting 论文分类索引 (YYYY-MM)

> 基于 `3dgs_YYYY-MM.md` 中收集的论文，按研究方向细分类。
> ★ 表示被顶会/顶刊录用。

## 目录

- [3D Gaussian Splatting 论文分类索引 (YYYY-MM)](#3d-gaussian-splatting-论文分类索引-yyyy-mm)
  - [目录](#目录)
  - [一、核心算法与优化 {#cat-core-opt}](#一核心算法与优化-cat-core-opt)
  - [二、渲染加速与压缩 {#cat-render-accel}](#二渲染加速与压缩-cat-render-accel)
  - [三、新视角合成 {#cat-nvs}](#三新视角合成-cat-nvs)
    - [3.1 可泛化 / 前向 {#cat-nvs-generalizable}](#31-可泛化--前向-cat-nvs-generalizable)
    - [3.2 稀疏视角 {#cat-nvs-sparse}](#32-稀疏视角-cat-nvs-sparse)
  - [四、动态场景与 4D {#cat-dynamic-4d}](#四动态场景与-4d-cat-dynamic-4d)
  - [五、语义分割与场景理解 {#cat-seg-understand}](#五语义分割与场景理解-cat-seg-understand)
  - [六、视觉定位 {#cat-visloc}](#六视觉定位-cat-visloc)
  - [七、几何与表面重建 {#cat-geo-recon}](#七几何与表面重建-cat-geo-recon)
  - [八、生成式模型 {#cat-generative}](#八生成式模型-cat-generative)
  - [九、流媒体与编码 {#cat-streaming}](#九流媒体与编码-cat-streaming)
  - [统计概览](#统计概览)

---

## 一、核心算法与优化 {#cat-core-opt}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-01 | [LeGS](#2-beyond-heuristics-learnable-density-control-for-3d-gaussian-splatting) | 2605.00408 | 强化学习密度控制 |

**概要**: 改进 3DGS 基础优化过程，包括优化器设计、密度控制、基元分裂/裁剪策略、基元分布模型等。

---

## 二、渲染加速与压缩 {#cat-render-accel}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-18 | [TensorGS](#2-accelerating-3d-gaussian-splatting-using-tensor-cores-tensorgs) | 2605.17855 | Tensor Core 张量化，1.65x 加速 |
| 2026-05-03 | [GETA-3DGS](#2-geta-3dgs-automatic-joint-structured-pruning-and-quantization-for-3d-gaussian-splatting) | 2605.02086 | 联合剪枝+量化，~5x 压缩 |

**概要**: 提升 3DGS 渲染性能或降低存储开销，包括硬件加速、包围盒裁剪、剪枝量化、后处理超采样等。

---

## 三、新视角合成 {#cat-nvs}

### 3.1 可泛化 / 前向 {#cat-nvs-generalizable}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-13 | ★ **[Z-Order Transformer for 3DGS](#5-z-order-transformer-for-feed-forward-gaussian-splatting)** | 2605.13465 | Z 序稀疏注意力，单次前向 (CVPR'26 Oral) |

### 3.2 稀疏视角 {#cat-nvs-sparse}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-12 | ★ **[GeoQuery](#8-geoquery-geometry-query-diffusion-for-sparse-view-reconstruction)** | 2605.12399 | 几何引导扩散修复伪像 (SIGGRAPH'26) |

**概要**: 无需逐场景优化即可合成新视角（可泛化/前向方法），或从极少输入视角重建场景（稀疏视角方法）。

---

## 四、动态场景与 4D {#cat-dynamic-4d}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-12 | ★ **[Retrospective Dynamic NVS](#3-3d-gaussian-splatting-for-efficient-retrospective-dynamic-scene-novel-view-synthesis-with-a-standardized-benchmark)** | 2605.12437 | 同步多视图回溯重建 (CVPR'26) |

**概要**: 处理随时间变化的动态场景，包括 4D 高斯表示、动态表面重建、时序一致性等。

---

## 五、语义分割与场景理解 {#cat-seg-understand}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-10 | ★ **[BEA-GS](#4-bea-gs-beyond-radiance-supervision-in-3dgs-for-precise-object-extraction)** | 2605.09662 | 超越辐射监督的精确物体提取 (CVPR'26 Highlight) |

**概要**: 3DGS 上的语义分割、开放词汇场景理解、语言 grounding 和物体级提取。

---

## 六、视觉定位 {#cat-visloc}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-06 | ★ **[ULF-Loc](#5-ulf-loc-unbiased-landmark-feature-for-robust-visual-localization-with-3d-gaussian-splatting)** | 2605.04730 | 无偏地标特征 (CVPR'26 Highlight) |

**概要**: 基于 3DGS 场景表示的视觉定位，包括紧凑场景表示、特征场、2D-3D 匹配消歧等。

---

## 七、几何与表面重建 {#cat-geo-recon}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-02 | ★ **[SplAttN](#1-splatttn-bridging-2d-and-3d-with-gaussian-soft-splatting-and-attention-for-point-cloud-completion)** | 2605.01466 | 高斯软光栅化，点云补全 (ICML'26 Spotlight) |

**概要**: 从图像重建几何准确的表面、网格或点云，包括表面光栅化、高频细节恢复、多传感器融合等。

---

## 八、生成式模型 {#cat-generative}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-08 | ★ **[DeG](#7-generative-3d-gaussians-with-learned-density-control)** | 2605.16355 | Octree+扩散模型，学习密度控制 (SIGGRAPH'26) |

**概要**: 使用扩散模型、自回归模型等生成式方法生成或编辑 3DGS 场景。

---

## 九、流媒体与编码 {#cat-streaming}

| 日期 | 论文 | arXiv | 关键词 |
|------|------|-------|--------|
| 2026-05-10 | ★ **[CAGS](#2-cags-color-adaptive-volumetric-video-streaming-with-dynamic-3d-gaussian-splatting)** | 2605.09279 | 矢量量化+颜色自适应，体视频流 (SIGGRAPH'26) |

**概要**: 3DGS 场景或动态 3DGS 的视频编码、流式传输和带宽优化。

---

## 统计概览

| 类别 | 论文数 |
|------|--------|
| 核心算法与优化 | 1 |
| 渲染加速与压缩 | 2 |
| 新视角合成 | 2 |
| 动态场景与 4D | 1 |
| 语义分割与场景理解 | 1 |
| 视觉定位 | 1 |
| 几何与表面重建 | 1 |
| 生成式模型 | 1 |
| 流媒体与编码 | 1 |
| **合计** | **11** |
