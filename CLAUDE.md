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

1. **搜索论文** — 使用 `arxiv-search` skill 按关键词和日期范围获取论文列表
2. **更新月度文件** — 将论文写入 `<领域>/<领域>_<YYYY-MM>.md`
   - 若该月文件不存在，参考 `tracking_sample.md` 创建
   - 按日期降序插入，注意表格行与正文区块同步（详见 [月度文档规范](.claude/rules/monthly-doc-rules.md)）
   - 若论文已存在，更新版本号及摘要内容
3. **更新分类文档** — 编辑 `<领域>/<领域>_category_<YYYY-MM>.md`
   - 若该月分类文档不存在，参考 `category_template.md` 创建
   - 从月度文件读取论文，按内容归入对应类别，一篇论文可归入多个类别（详见 [分类文档规范](.claude/rules/category-doc-rules.md)）
   - 更新底部统计概览
4. **提交推送** — `git commit` 并 `git push`

### 论文版本处理

- **不要忽略 v2/v3 等版本更新的论文**。检索结果中带有 v2、v3 或更高版本标识的论文同样需要记录到文件中
- 在论文简述的 arXiv 编号或备注后标注版本号，如 `[2605.17916v3](https://arxiv.org/abs/2605.17916)`
- 若该论文已在本月文件中存在，更新其版本号并补充/更新摘要内容

详细规范请参见：
- [月度文档规范](.claude/rules/monthly-doc-rules.md) — 标题、表格、论文简述、亮点标记、排序规则等
- [分类文档规范](.claude/rules/category-doc-rules.md) — 格式、分类规则、锚点、统计概览等
