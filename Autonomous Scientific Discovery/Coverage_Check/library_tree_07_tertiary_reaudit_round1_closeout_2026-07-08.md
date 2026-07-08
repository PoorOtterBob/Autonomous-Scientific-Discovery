# library_tree_07_tertiary_reaudit_round1_closeout_2026-07-08

日期：`2026-07-08`

## 1. 本轮范围

本轮严格执行：

- `Coverage_Check/library_tree_secondary_tertiary_reaudit_plan_03_04_06_07_2026-07-08.md`

处理对象只限于：

- `Coverage_Check/library_tree_confidence_medium_queue_03_04_06_07_and_07_tertiary_2026-07-08.tsv`
  中的 `07` 三级类 `medium queue` `13` 篇

本轮继续遵守：

- 只按原始图书馆学树复核
- 不使用 `secondary_class_redefinition_updated_mapping_after_batchI_...tsv`
- 不使用 `secondary_class_redefinition_no_bnd_mapping_after_batchM_...tsv`
- 不修改 owner fact source

可用证据仍限于：

- `review_scope_and_classification_policy.md`
- `domain_classification_rules.md`
- `science_domain_taxonomy.md`
- `Paper_Lists/agent_master_paper_list.md`
- 对应 note
- 必要时的一手 PDF / HTML 证据

## 2. 本轮结论

本轮 `13` 篇里：

- `9` 篇提升为当前可接受的高置信度三级类归位
- `4` 篇继续保留在 `medium queue`
- 本轮未新增 `07` 三级类代码
- 本轮未改写 owner fact source

## 3. 逐篇复核结果

### 3.1 提升为高置信度

| paper_id | 当前三级类 | 结论 | 主要依据 | 处理 |
|---|---|---|---|---|
| `ASD-0060` | `07.04.01` | 维持并提升为高置信度 | note 与 remarks 已明确给出 `pChEMBL lead-compound / drug-discovery framing`，`07` 侧不是泛 biomedical 口号，而是可直接落到药物发现 | 移出 medium queue |
| `ASD-0093` | `07.04.01` | 维持并提升为高置信度 | local PDF 已确认 chemistry tools 同时覆盖 drug-discovery task coverage，`07` 侧是稳定药物发现 slice | 移出 medium queue |
| `ASD-0096` | `07.04.01` | 维持并提升为高置信度 | WDR5 target / ligand / inhibitor / drug-candidate docking design 直接指向药物发现 | 移出 medium queue |
| `ASD-0254` | `07.03.08` | 维持并提升为高置信度 | end-to-end biomedical research workflow 自动化、disease objective、diagnosis / prognosis / translational analysis 共同支持医学信息学 | 移出 medium queue |
| `ASD-0660` | `07.01.08` | 维持并提升为高置信度 | rare-disease diagnosis 与 GWAS example 让 `07` 侧最稳地落到医学遗传学 | 移出 medium queue |
| `ASD-0673` | `07.04.01` | 维持并提升为高置信度 | note 已明确 `drug-design virtual screening campaigns`，`07` 侧不是泛平台支持，而是药物设计 campaign | 移出 medium queue |
| `ASD-0676` | `07.04.01` | 维持并提升为高置信度 | PROTAC-STAN、DeepTernary、degrader target nomination、drug-discovery framing 共同把 `07` 锁定到药物发现 | 移出 medium queue |
| `ASD-0856` | `07.02.06` | 维持并提升为高置信度 | SEA-AD、Alzheimer's-spectrum donor cognition、neuropathology 直接支持神经病学 | 移出 medium queue |
| `ASD-0866` | `07.04.05` | 维持并提升为高置信度 | PD-L1 nanobody binders 与 biologic therapeutic modality 直接支持生物制药 | 移出 medium queue |

### 3.2 保留为 medium queue

| paper_id | 当前三级类 | 结论 | 保留原因 | 后续重点 |
|---|---|---|---|---|
| `ASD-0659` | `07.03.08` | 暂保留 medium | `07` 证据来自 `SSTR2 therapeutic receptor context` 与 peptide-design-for-discovery，说明 `07` 侧真实存在，但严格落点仍在 `07.03.08` 与 `07.04.01` 之间有拉力 | 专看该 investigation 段，确认是 medical-informatics support 还是 therapeutic-discovery 主导 |
| `ASD-0663` | `07.03.08` | 暂保留 medium | `07` 证据混合了 biomedical imaging 与 drug-discovery tasks，当前 `07.03.08` 尚可使用，但不是唯一稳定落点 | 需要再看 full-text task coverage，判断是否应转向 `07.04.01` |
| `ASD-0731` | `07.03.08` | 暂保留 medium | 论文主形态是 biomedical knowledge extraction / dataset construction，但 `07` 证据来自 BBB / oral bioavailability / LD50 等 pharmacological property tasks，`informatics` 与 `pharmacology-facing discovery support` 之间仍有张力 | 复核 task framing 是否以知识构建为主，还是更接近药学属性发现基础设施 |
| `ASD-0871` | `07.03.08` | 暂保留 medium | `07` 侧由 fertility outcomes 与 digital-health tasks 支撑，方向上更接近医学信息学，但它仍只是一个极宽跨域系统中的单个切片 | 需要再确认 `07` slice 的对象重心是否足够稳定地停在 `07.03.08` |

## 4. 本轮后的队列变化

本轮前：

- `03` 二级类 `12`
- `04` 二级类 `12`
- `06` 二级类 `16`
- `07` 三级类 `13`
- 合计 `53`

本轮后：

- `03` 二级类 `12`
- `04` 二级类 `12`
- `06` 二级类 `16`
- `07` 三级类 `4`
- 合计 `44`

也就是说，`07` 三级类 `medium queue` 已从 `13` 压缩到 `4`。

## 5. 对当前 07 三级类结构的影响

本轮没有新增三级类代码，也没有改写当前 `07` 三级类 TSV 中的归位代码。

本轮收敛的是：

- 哪些条目已经足以把当前三级类归位视为高置信度
- 哪些条目虽然已有可用落点，但还需要一轮 targeted reread 才能彻底锁死

因此，本轮更像是一次 `confidence compression`，而不是一次大规模重排。

## 6. 下一步建议

按原计划继续：

1. 先把剩余 `4` 篇 `07` 三级类 medium 样本做 targeted reread
2. 然后进入 `06 / 07` 边界样本
3. 最后再处理 `03 / 04` 边界样本

当前最值得优先继续看的就是：

- `ASD-0659`
- `ASD-0663`
- `ASD-0731`
- `ASD-0871`
