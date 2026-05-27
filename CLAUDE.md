# CLAUDE.md

## 仓库说明

本仓库用于跟踪 Arxiv 上的论文进展。各领域论文按子目录分类管理。

## 目录结构规则

```
论文跟踪/
├── tracking_sample.md             # 月度跟踪文件格式模板
├── category_template.md           # 分类文档模板
├── CLAUDE.md                      # 项目指令
├── README.md
├── <领域>/
│   ├── <领域>_<YYYY-MM>.md        # 月度跟踪文件
│   └── <领域>_category_<YYYY-MM>.md # 分类文档
├── <另一领域>/
│   └── ...
```

- 根目录下放置通用模板（`tracking_sample.md`、`category_template.md`）与项目说明（`CLAUDE.md`、`README.md`）
- 每个研究领域一个子目录，目录名为领域小写英文标识（如 `3dgs/`）
- 子目录内文件命名规则：
  - 月度跟踪文件：`<领域>_<YYYY-MM>.md`（如 `3dgs_2026-05.md`）
  - 分类文档：`<领域>_category_<YYYY-MM>.md`（如 `3dgs_category_2026-05.md`）
- 每月一个跟踪文件加一个分类文档，按月份独立建文件
- 新增领域时创建对应子目录，文件格式参考现有目录

## 工作流程

1. **搜索论文** — 使用 `arxiv-search` skill 按关键词和日期范围获取论文列表，输出为 JSON 文件
2. **生成月度文档和分类文档** — 使用 `arxiv-to-tracking` skill 处理 JSON 文件
   - LLM 处理阶段：对每篇论文完成摘要翻译、概述提取、亮点判断、分类、关键词生成
   - 月度文档生成阶段：将处理后的数据渲染为 `<领域>/<领域>_<YYYY-MM>.md`
   - 分类文档生成阶段：将论文按研究方向归类，生成 `<领域>/<领域>_category_<YYYY-MM>.md`
3. **校验** — 检查生成文档是否符合 [月度文档规范](.claude/rules/monthly-doc-rules.md) 和 [分类文档规范](.claude/rules/category-doc-rules.md)
4. **提交推送** — `git commit` 并 `git push`

### 论文版本处理

- **不要忽略 v2/v3 等版本更新的论文**。检索结果中带有 v2、v3 或更高版本标识的论文同样需要记录到文件中
- 在论文概述的 arXiv 编号或备注后标注版本号，如 `[2605.17916v3](https://arxiv.org/abs/2605.17916)`
- 若该论文已在本月文件中存在，更新其版本号并补充/更新摘要内容

详细规范请参见：
- [月度文档规范](.claude/rules/monthly-doc-rules.md) — 标题、表格、论文概述、亮点标记、排序规则等
- [分类文档规范](.claude/rules/category-doc-rules.md) — 格式、分类规则、锚点、统计概览等
