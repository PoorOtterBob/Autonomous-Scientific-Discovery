# library_tree_confidence_audit_03_04_06_07_and_07_tertiary_2026-07-08

日期：`2026-07-08`

## 1. 目标

本轮目标不是继续扩展二级类 / 三级类体系，而是提高以下结果的**分类置信度**：

- `03 / 04 / 06 / 07` 的原始图书馆学二级类归位
- `07` 的原始图书馆学三级类归位

本轮继续遵守：

- 不修改 owner fact source
- 不把 `secondary_class_redefinition_updated_mapping_after_batchI_...tsv`
- 不把 `secondary_class_redefinition_no_bnd_mapping_after_batchM_...tsv`

当作本轮分类依据

本轮只依赖：

- `review_scope_and_classification_policy.md`
- `domain_classification_rules.md`
- `science_domain_taxonomy.md`
- `papers.sqlite / papers.jsonl` 中当前 authoritative 事实
- `remarks`
- 对应 note 的已冻结说明与标题

## 2. 置信度工作法

本轮把样本分成两类：

### 2.1 高置信度

满足以下任一条件即可升到高置信度：

- 本模块 `primary_module_for_filing` 与 `legacy_secondary_class` 已稳定同向
- 多模块展开后虽然是 extra row，但 `remarks` 明确给出该模块的具体对象证据，而且该对象能直接落到原始图书馆学树
- `07` 三级类中，题目 / note / `remarks` 已明确指向药物发现、病理、肿瘤、神经影像、医学信息学、生物制药等稳定对象

### 2.2 中等置信度

保留为中等置信度的典型原因：

- general scientific system / workflow orchestration 外观很强
- 跨模块 benchmark / demo slice 存在，但该模块对象不是论文稳定主对象
- cross-domain harness / equation-discovery / multidisciplinary platform 压力仍大
- 在 `07` 中更像 biomedical workflow / translational analysis / digital-health support，而不是单一稳定疾病或单一药学对象

## 3. 本轮提高了哪些置信度

### 3.1 `07` 三级类

下列簇已经可以视为高置信度：

- `07.04.01 药物发现`
  - 大部分 drug discovery / lead optimization / DTI / de novo design / therapeutic reasoning / target discovery / combination screen 论文
- `07.04.05 生物制药`
  - nanobody、CAR-T、biologics、therapeutic modality 明确的论文
- `07.01.04 病理学`
  - cancer pathology / computational pathology / pathology biomarker 明确样本
- `07.02.05 肿瘤学`
  - 肿瘤病例、肿瘤空间组学、癌症 biomarker / prognosis 明确样本
- `07.02.06 神经病学`
  - neuroimaging / cognitive-neurology case 明确样本
- `07.03.08 医学信息学`
  - translational bioinformatics、medical research analysis、biomedical workflow automation、biomedical knowledge extraction 明确样本

因此，本轮推荐把 `07` 的父类分布优先改读为三级类回卷后的结果：

- `07.01 = 10`
- `07.02 = 8`
- `07.03 = 22`
- `07.04 = 40`

而不是更早那版二级类粗分的 `10 / 6 / 12 / 52`。

### 3.2 `03 / 04 / 06` 二级类

通过复核 `remarks` 与 note 冻结说明后，本轮已经把大量 extra-row 样本从“纯边界压力”提升为“可接受的高置信度研究层归位”。

例如：

- `03.03`
  - 反应优化、催化、自驱流动化学、实验闭环
- `03.04`
  - 分子设计、小分子优化、drug-like molecular discovery
- `04.04`
  - 电池、超材料、光电/器件材料、能源材料
- `06.03`
  - omics、single-cell、proteomics、protein / enzyme、biomolecular design

这些类的主干样本已经比较稳，不需要再把整类都视为低置信度。

## 4. 剩余中等置信度队列

本轮之后，建议保留为**中等置信度 / 下一轮优先点查**的，不是整类，而是少数压力样本。

详见：

- `Coverage_Check/library_tree_confidence_medium_queue_03_04_06_07_and_07_tertiary_2026-07-08.tsv`

### 4.1 `03` 二级类剩余中等置信度

主要是：

- general-scientific systems 被 relaxed object-coverage 牵引进 `03`
- equation-discovery / multidisciplinary systems 在 `03` 侧只有 benchmark slice
- 材料 / 医学主导论文在 `03` 侧只有 secondary chemistry evidence

### 4.2 `04` 二级类剩余中等置信度

主要是：

- workflow infrastructure / tool orchestration / atomistic harness 论文
- equation-discovery 和 general scientific system 在 `04` 侧只有 benchmark support
- `03 / 04` 之间 object pressure 仍较强的边界样本

### 4.3 `06` 二级类剩余中等置信度

主要是：

- biomedical workflow、general scientific system、distributed discovery ecosystem
- `06 / 07` 双压力样本
- `01.04 / 06` 旧 general-method 压力未完全消失的样本

### 4.4 `07` 三级类剩余中等置信度

主要是：

- biomedical workflow / translational analysis / knowledge-extraction 型条目
- multidisciplinary scientific systems 中切出来的 `07` evidence slice
- cross-domain atomistic / scientific-discovery frameworks 里只有一部分医学对象 demo 的条目

## 5. 当前建议结论

当前最稳的结论不是“这套结果已经 100% 最终冻结”，而是：

1. `03 / 04 / 06 / 07` 的原始图书馆学二级类已经可以分成“高置信度 bulk + 中等置信度小队列”。
2. `07` 的原始图书馆学三级类已经具备可用结构，尤其 `07.04.01`、`07.03.08`、`07.02.05` 这几个簇已明显成型。
3. 后续提高置信度的最高收益路线，不是重做全库，而是继续清理这份 medium queue。

## 6. 推荐下一步

优先顺序建议：

1. 先继续清理 `07` 三级类 medium queue
2. 再清理 `06 / 07` 边界样本
3. 再处理 `03 / 04` 中的 general-system / equation-discovery 压力样本

这样可以最快把“可用”推进到“更稳”。
