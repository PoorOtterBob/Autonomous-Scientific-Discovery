# library_tree_secondary_recount_and_07_tertiary_classification_2026-07-08

日期：`2026-07-08`

## 1. 范围

本文件记录基于原始图书馆学树的研究层统计与归位结果。

本轮继续明确忽略以下两份非原始树映射文件，不把它们当作分类依据：

- `Coverage_Check/secondary_class_redefinition_updated_mapping_after_batchI_03_04_06_07_multi_module_2026-07-07.tsv`
- `Coverage_Check/secondary_class_redefinition_no_bnd_mapping_after_batchM_03_04_06_07_multi_module_2026-07-08.tsv`

可用依据只包括：

- `review_scope_and_classification_policy.md`
- `domain_classification_rules.md`
- `science_domain_taxonomy.md`
- 当前结构化事实中的 `scientific_object_modules`、`primary_module_for_filing`、`legacy_secondary_class`、`remarks`
- 对应 note 与一手 PDF / HTML 证据

## 2. 二级类统计

口径：

- 多模块口径
- 只允许原始图书馆学二级类代码
- `07` 的最终二级类优先采用三级类回卷后的结果

### 2.1 `03` 化学科学

| 二级类代码 | 二级类名称 | 数量 |
|---|---|---:|
| `03.01` | 化学总论与化学方法 | 6 |
| `03.02` | 基础化学 | 6 |
| `03.03` | 合成、反应与催化 | 36 |
| `03.04` | 分子设计与化学空间探索 | 42 |
| 合计 |  | 90 |

### 2.2 `04` 材料科学

| 二级类代码 | 二级类名称 | 数量 |
|---|---|---:|
| `04.01` | 材料基础 | 18 |
| `04.02` | 结构材料与无机材料 | 3 |
| `04.03` | 软物质与功能材料 | 22 |
| `04.04` | 能源、电子与器件材料 | 74 |
| 合计 |  | 117 |

### 2.3 `06` 生命科学

当前最新二级类统计已经纳入 `06 / 07` 二级类 round1 与 round2 closeout 的结果。

| 二级类代码 | 二级类名称 | 数量 |
|---|---|---:|
| `06.01` | 生物学基础 | 17 |
| `06.02` | 生物类群科学 | 3 |
| `06.03` | 生物技术相关科学 | 58 |
| 合计 |  | 78 |

### 2.4 `07` 医学与健康科学

当前 `07` 二级类以三级类回卷后的结果为准。

| 二级类代码 | 二级类名称 | 数量 |
|---|---|---:|
| `07.01` | 医学基础 | 10 |
| `07.02` | 临床医学 | 8 |
| `07.03` | 公共卫生与健康科学 | 21 |
| `07.04` | 药学与生物医药 | 41 |
| 合计 |  | 80 |

## 3. `07` 三级类统计

### 3.1 使用规则

`07` 三级类继续只使用原始 taxonomy 树中的正式代码：

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

### 3.2 最新三级类统计

当前统计已经纳入：

- `library_tree_07_tertiary_reaudit_round1_closeout_2026-07-08.md`
- `library_tree_07_tertiary_reaudit_round2_closeout_2026-07-08.md`

| 三级类代码 | 三级类名称 | 数量 |
|---|---|---:|
| `07.01.04` | 病理学 | 3 |
| `07.01.06` | 药理学 | 1 |
| `07.01.07` | 毒理学 | 1 |
| `07.01.08` | 医学遗传学 | 4 |
| `07.01.09` | 医学免疫学 | 1 |
| `07.02.05` | 肿瘤学 | 6 |
| `07.02.06` | 神经病学 | 2 |
| `07.03.08` | 医学信息学 | 21 |
| `07.04.01` | 药物发现 | 37 |
| `07.04.05` | 生物制药 | 4 |
| 合计 |  | 80 |

### 3.3 三级类回卷到二级类

由当前三级类直接回卷得到：

- `07.01 = 10`
- `07.02 = 8`
- `07.03 = 21`
- `07.04 = 41`

这组数字是当前更值得优先保留的 `07` 研究层基线。

## 4. 当前残留压力点

到当前阶段为止：

- `07` 三级类 `medium queue` 已清空
- `06 / 07` 最关键的一组二级类边界样本已大幅压缩

当前剩余 residuals 主要位于：

- `06 secondary` 中的 general-system / equation-discovery / workflow pressure 样本
- `03 / 04` 中的 molecule-vs-material、atomistic-harness、equation-discovery pressure 样本

因此，这份文件中的 `07` 三级类结果现在可以作为当前研究层高置信度 baseline 使用；更新后的残留清单以：

- `Coverage_Check/library_tree_confidence_medium_queue_03_04_06_07_and_07_tertiary_2026-07-08.tsv`

为准。

## 5. 产出文件

- 本说明文件：
  - `Coverage_Check/library_tree_secondary_recount_and_07_tertiary_classification_2026-07-08.md`
- `07` 逐篇三级类归位表：
  - `Coverage_Check/library_tree_07_tertiary_classification_multi_module_2026-07-08.tsv`
