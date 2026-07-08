# library_tree_secondary_tertiary_reaudit_plan_03_04_06_07_2026-07-08

日期：`2026-07-08`

## 1. 计划目标

本计划用于继续提高以下结果的分类置信度：

- `03 / 04 / 06 / 07` 的原始图书馆学**二级类**归位
- `07` 的原始图书馆学**三级类**归位

本轮目标不是重新发明二级类 / 三级类体系，也不是继续扩展新类，而是把已经给出的原始树归位结果做成：

1. 高置信度主干结果
2. 可审计的中等置信度队列
3. 可逐轮清理的复核工作流

## 2. 口径锁定

本计划只允许使用最早定义的图书馆学原始树。

### 2.1 二级类树

只允许：

- `03.01` `03.02` `03.03` `03.04`
- `04.01` `04.02` `04.03` `04.04`
- `06.01` `06.02` `06.03`
- `07.01` `07.02` `07.03` `07.04`

### 2.2 `07` 三级类树

只允许 `science_domain_taxonomy.md` 中原始 `07.xx.xx` 代码。

当前已经实际使用的三级类包括：

- `07.01.04` 病理学
- `07.01.06` 药理学
- `07.01.07` 毒理学
- `07.01.08` 医学遗传学
- `07.01.09` 医学免疫学
- `07.02.05` 肿瘤学
- `07.02.06` 神经病学
- `07.03.08` 医学信息学
- `07.04.01` 药物发现
- `07.04.05` 生物制药

后续若新增 `07` 三级类，也必须先能在原始 taxonomy 树中找到正式代码。

### 2.3 明确不用作分类依据的文件

以下文件可作为历史研究轨迹参考，但**不得**作为本计划的分类判定依据：

- `Coverage_Check/secondary_class_redefinition_updated_mapping_after_batchI_03_04_06_07_multi_module_2026-07-07.tsv`
- `Coverage_Check/secondary_class_redefinition_no_bnd_mapping_after_batchM_03_04_06_07_multi_module_2026-07-08.tsv`

## 3. 事实源与允许证据

本计划仍然是研究层复核，不修改 owner fact source。

### 3.1 不修改

- `Paper_Lists/agent_master_paper_list.md`
- `Coverage_Check/multi_module_note_pdf_full_reaudit_progress_451_2026-06-21.md`
- `Data/discipline_code_assignments.jsonl`
- `Data/classification_code_index.json`

### 3.2 可用证据

允许作为复核依据的材料：

1. `review_scope_and_classification_policy.md`
2. `domain_classification_rules.md`
3. `science_domain_taxonomy.md`
4. `Data/papers.jsonl` / `Data/papers.sqlite`
5. 当前 `remarks`
6. 对应 note 的冻结说明、标题、证据摘要
7. 本地 PDF、publisher HTML、DOI landing page、supplementary、official project page

### 3.3 证据优先级

1. 本地 PDF 全文
2. 官方 HTML / DOI full text
3. publisher abstract / DOI landing page
4. note 中已冻结并可追溯到一手来源的说明

如果只有标题、旧 note 简述、或 benchmark 标签而缺少明确对象证据，不提升到高置信度。

## 4. 复核原则

### 4.1 二级类原则

- 先判定论文在该模块中的**直接科学对象**是什么。
- 不按系统外观、平台通用性、agent 架构、benchmark 名称归类。
- 多模块论文允许在不同模块下落到不同二级类，但每个模块内部只能落一个最稳的二级类。

### 4.2 `07` 三级类原则

- 先判定 `07` 侧的直接医学对象，而不是先看它是不是 “biomedical platform”。
- 药物设计、lead 优化、target discovery、DTI、drug response 优先落 `07.04.01`。
- nanobody、CAR-T、biologic modality 优先落 `07.04.05`。
- pathology / computational pathology / disease biomarker 优先落 `07.01.04` 或 `07.02.05`。
- neuroimaging / neurological disease 优先落 `07.02.06`。
- biomedical workflow、translational bioinformatics、medical research analysis、knowledge extraction 优先落 `07.03.08`。

### 4.3 置信度原则

高置信度：

- 对象明确
- 原始树内落点唯一或高度稳定
- `remarks` / note / 一手来源之间一致

中等置信度：

- 对象存在，但 general-system / benchmark / cross-domain 外观很强
- 原始树内可落位，但替代落位并非完全不可辩

低置信度：

- 证据不足
- 需要全文重看
- 当前连“本模块内是否应该落到这个类”都不够稳

本计划的目标是尽量把 low 消灭掉，把 medium 压缩成小队列。

## 5. 当前工作基线

当前已有研究层结果：

- `Coverage_Check/library_tree_secondary_recount_and_07_tertiary_classification_2026-07-08.md`
- `Coverage_Check/library_tree_07_tertiary_classification_multi_module_2026-07-08.tsv`
- `Coverage_Check/library_tree_confidence_audit_03_04_06_07_and_07_tertiary_2026-07-08.md`
- `Coverage_Check/library_tree_confidence_medium_queue_03_04_06_07_and_07_tertiary_2026-07-08.tsv`

当前 medium queue 规模：

- `03` 二级类：`12`
- `04` 二级类：`12`
- `06` 二级类：`16`
- `07` 三级类：`13`

合计：`53`

## 6. 批次顺序

### 6.1 第一优先批次：`07` 三级类 medium queue

原因：

- `07` 目前已经有完整三级类表
- 直接影响 `07` 的二级类回卷结果
- 规模最小，收益最高

本批目标：

- 尽量把 `13` 条 medium queue 中的一半以上提升为高置信度
- 明确保留的 medium 条目必须写清楚“为什么暂不提升”

### 6.2 第二优先批次：`06 / 07` 边界样本

重点看：

- omics / transcriptomics / perturbation / protein / biomarker / pathology / translational cases
- 这些样本既影响 `06` 二级类，也影响 `07` 三级类

### 6.3 第三优先批次：`03 / 04` 边界样本

重点看：

- molecule vs material
- catalyst vs catalyst material
- workflow / atomistic harness / equation discovery 在 `03` 或 `04` 侧到底是对象还是 support slice

## 7. 每轮执行步骤

每轮固定执行：

1. 从 medium queue 中选一小批
2. 逐篇看 `remarks`、note、必要时看 PDF / HTML
3. 给出：
   - 维持原归位
   - 调整归位
   - 暂保留 medium
4. 更新研究层 TSV / md 结果
5. 写一份 `Coverage_Check` closeout
6. git commit

## 8. 每篇论文的最小输出字段

每篇复核样本至少记录：

- `paper_id`
- 标题
- 当前二级类或三级类
- 建议维持 / 调整后的类
- 所属模块
- 主要对象证据
- 一手来源层级
- 置信度
- 是否仍留在 medium queue
- 理由

## 9. 产出物

本计划后续每轮至少产出：

1. 一份 `Coverage_Check/*.md` 中文 closeout
2. 必要时一份更新后的研究层 TSV
3. 一次 git commit

## 10. 停止条件

当满足以下条件时，可认为这条线阶段性收口：

1. `07` 三级类 medium queue 降到很小规模，且剩余条目理由明确
2. `03 / 04 / 06 / 07` 二级类主干结果已形成稳定高置信度 bulk
3. 剩余 medium 样本不再影响整体分布判断，只影响个别边界论文

## 11. 一句话定义

这份计划的任务不是“再造一套新分类”，而是把原始图书馆学树在 `03 / 04 / 06 / 07` 上真正压实到可长期复用的研究层高置信度结果。
