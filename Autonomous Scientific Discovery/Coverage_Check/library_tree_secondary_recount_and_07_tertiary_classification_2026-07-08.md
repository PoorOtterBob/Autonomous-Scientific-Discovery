# library_tree_secondary_recount_and_07_tertiary_classification_2026-07-08

日期：`2026-07-08`

## 1. 本轮范围

本轮只按最早定义的图书馆学分类树执行 derived / research-layer 统计与归位，不修改 owner fact source。

本轮明确忽略以下两份研究层映射文件，不把它们当作本轮二级类或三级类依据：

- `Coverage_Check/secondary_class_redefinition_updated_mapping_after_batchI_03_04_06_07_multi_module_2026-07-07.tsv`
- `Coverage_Check/secondary_class_redefinition_no_bnd_mapping_after_batchM_03_04_06_07_multi_module_2026-07-08.tsv`

本轮使用的依据只有：

- `review_scope_and_classification_policy.md`
- `domain_classification_rules.md`
- `science_domain_taxonomy.md`
- 当前结构化事实层中的 `scientific_object_modules`、`primary_module_for_filing`、`legacy_secondary_class`、`remarks`
- 对应 paper notes 的标题与已冻结说明

## 2. 03 / 04 / 06 / 07 二级类统计

口径：

- 多模块口径
- 只允许原始图书馆学二级类代码
- native 行优先继承同模块 `legacy_secondary_class`
- 多模块展开后新增的外模块行，再按原始树对象定义重新归位

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

| 二级类代码 | 二级类名称 | 数量 |
|---|---|---:|
| `06.01` | 生物学基础 | 19 |
| `06.02` | 生物类群科学 | 3 |
| `06.03` | 生物技术相关科学 | 56 |
| 合计 |  | 78 |

### 2.4 `07` 医学与健康科学

这一步是二级类层面的初步 recount，尚未使用三级类细分回卷。

| 二级类代码 | 二级类名称 | 数量 |
|---|---|---:|
| `07.01` | 医学基础 | 10 |
| `07.02` | 临床医学 | 6 |
| `07.03` | 公共卫生与健康科学 | 12 |
| `07.04` | 药学与生物医药 | 52 |
| 合计 |  | 80 |

## 3. `07` 三级类分类

### 3.1 三级类使用规则

本轮 `07` 三级类继续只使用原始图书馆学树中的正式代码：

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

归位优先级：

1. 先看 `07` 模块证据来自什么具体医学对象。
2. 如果是药物设计、lead 优化、筛选、target / DTI / de novo design，优先落 `07.04.01`。
3. 如果是抗体、nanobody、CAR-T、生物治疗模态，优先落 `07.04.05`。
4. 如果是病理、肿瘤、神经影像、疾病队列等疾病对象，优先落对应临床 / 基础医学三级类。
5. 如果 `07` 侧主要体现为 biomedical workflow、translational bioinformatics、medical-research analysis、evidence screening、knowledge extraction，则优先落 `07.03.08`。

### 3.2 `07` 三级类统计

| 三级类代码 | 三级类名称 | 数量 |
|---|---|---:|
| `07.01.04` | 病理学 | 3 |
| `07.01.06` | 药理学 | 1 |
| `07.01.07` | 毒理学 | 1 |
| `07.01.08` | 医学遗传学 | 4 |
| `07.01.09` | 医学免疫学 | 1 |
| `07.02.05` | 肿瘤学 | 6 |
| `07.02.06` | 神经病学 | 2 |
| `07.03.08` | 医学信息学 | 22 |
| `07.04.01` | 药物发现 | 36 |
| `07.04.05` | 生物制药 | 4 |
| 合计 |  | 80 |

### 3.3 从三级类回卷得到的 `07` 二级类数量

如果直接按本轮三级类代码回卷到二级父类，则 `07` 的父类分布会变成：

| 二级类代码 | 二级类名称 | 数量 |
|---|---|---:|
| `07.01` | 医学基础 | 10 |
| `07.02` | 临床医学 | 8 |
| `07.03` | 公共卫生与健康科学 | 22 |
| `07.04` | 药学与生物医药 | 40 |
| 合计 |  | 80 |

这与上面的二级类初步 recount 不完全一致，说明：

- 二级类粗分时，若直接从原 `legacy_secondary_class` 与多模块 extra rows 进行对象级回填，容易把一部分 biomedical workflow / knowledge-extraction / translational-analysis 工作先放进 `07.04`
- 一旦继续细化到三级类，这些条目会更自然地滑入 `07.03.08`

因此，如果后续要把 `07` 的原始图书馆学树细化结果继续往前推进，本轮三级类回卷后的 `07.01 / 07.02 / 07.03 / 07.04 = 10 / 8 / 22 / 40` 更值得优先保留为研究层参考值。

## 4. 低置信度压力点

以下条目不是“无依据”，但属于强 general-system / cross-domain pressure 样本，后续如果要把 `07` 三级类写回更正式的派生表，建议优先二次复核：

- `ASD-0060`
- `ASD-0659`
- `ASD-0660`
- `ASD-0663`
- `ASD-0673`
- `ASD-0676`
- `ASD-0856`
- `ASD-0866`
- `ASD-0871`

这些论文的问题不是 `07` 证据不存在，而是它们的医学与健康侧证据通常来自：

- drug-discovery demos
- rare-disease / GWAS cases
- translational bioinformatics bundles
- digital-health / biomedical workflow demos
- general scientific systems 中的 biomedical benchmark slices

因此，它们适合保留在研究层三级类映射里，但不应误读为已经成为 owner fact source 中冻结好的正式三级类字段。

## 5. 产出文件

- 本说明文件：
  - `Coverage_Check/library_tree_secondary_recount_and_07_tertiary_classification_2026-07-08.md`
- `07` 逐篇三级类归位表：
  - `Coverage_Check/library_tree_07_tertiary_classification_multi_module_2026-07-08.tsv`
