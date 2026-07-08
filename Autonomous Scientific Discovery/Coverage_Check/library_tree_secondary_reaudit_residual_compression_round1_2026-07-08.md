# library_tree_secondary_reaudit_residual_compression_round1_2026-07-08

日期：`2026-07-08`

## 1. 本轮范围

本轮继续执行：
- `Coverage_Check/library_tree_secondary_tertiary_reaudit_plan_03_04_06_07_2026-07-08.md`

在前几轮已经分别压缩 `07` 三级类、`04` 二级类以及 `03/06` 中的 equation-discovery residual 之后，本轮目标改为压缩剩余 queue 中那些“对象证据已足够明确，但之前尚未正式从队列里移出”的样本。

本轮处理对象：

- `ASD-0004`
- `ASD-0662`
- `ASD-0731`
- `ASD-0671`
- `ASD-0787`
- `ASD-0844`

这些样本的共同特征是：

- 它们都仍然带有 general-system / benchmark / workflow surface pressure
- 但 note 与冻结裁决已经把 concrete object evidence 写得足够清楚
- 当前 residual 的来源主要不是 `class risk`，而是旧的保守留队状态还没有完全清掉

## 2. 本轮结论

本轮复核后，将上述 `8` 条 queue 行全部移出。

本轮后：

- `03 secondary medium queue: 4 -> 1`
- `06 secondary medium queue: 5 -> 0`
- `combined queue: 9 -> 1`

本轮后的唯一剩余样本为：

- `ASD-0673`

这意味着当前计划的 stop condition 已经基本满足：

1. `04` 与 `06` 的二级类主干结果已经形成稳定高置信度 bulk
2. `03` 也只剩一个 exact-slot residual
3. 剩余 medium 样本已经不再影响整体分布判断

## 3. 逐项判定

### 3.1 `ASD-0004`

- `03`：移出 queue，维持 `03.02`
- `06`：移出 queue，维持 `06.03`

关键依据：

- note 已冻结为：
  - `scientific_object_modules=01;03;06;09;10`
- 具体对象任务不是抽象 cross-domain demo，而是明确列出：
  - `03`: `reaction yield prediction`, `small-molecule molecular dynamics`, `Suzuki-Miyaura reaction yield`, `MD17`
  - `06`: `transcription perturbation`, `enhancer activity`

本轮判断：

- 这篇论文的 residual 已不在“03/06 是否成立”，而只在于它整体看起来像通用 closed-loop research agent。
- 在当前原始图书馆学二级类复核层面，`03.02` 与 `06.03` 已经足够稳定。

### 3.2 `ASD-0662`

- `03`：移出 queue，维持 `03.02`
- `06`：移出 queue，维持 `06.01`

关键依据：

- note 已冻结为：
  - `scientific_object_modules=03;05;06;11`
- 官方 PDF 已明确：
  - `03`: `chemistry tasks`
  - `06`: `bioinformatics tasks`
- note 还直接写明：
  - `主要风险 | core-strength risk 大于 class risk`
  - `风险在 benchmark 主导的证据强度，不在对象模块是否成立`

本轮判断：

- 既然当前 note 已经把问题明确限定为“core-strength risk 大于 class risk”，那么继续把它留在 `03/06 secondary queue` 已经没有必要。
- 二级类复核关心的是落位是否成立，不是这篇 benchmark-heavy 论文在 confirmed-core 强度上是否还值得更严复核。

### 3.3 `ASD-0731`

- `03`：移出 queue，维持 `03.01`

关键依据：

- note 已冻结为：
  - `scientific_object_modules=03;06;07`
  - `primary_module_for_filing=06`
- `03` 侧一手对象证据为：
  - `chemical-reaction extraction tasks`
- 当前 note 还把这一点写成显式 module assignment evidence，而不是模糊的 side mention。

本轮判断：

- 对于原始二级类树而言，chemical-reaction extraction 足以稳定落在 `03.01` 这类 chemistry-method / chemistry-information 侧。
- 当前 residual 只是在 biomedical knowledge-extraction 外观下显得“化学不是 primary”，而不是 `03` 落位本身不成立。

### 3.4 `ASD-0671`

- `06`：移出 queue，维持 `06.01`

关键依据：

- note 已明确：
  - `scientific_object_modules=01;02;06`
- `06` 侧对象证据非常具体：
  - `COBRApy`
  - `BiGG`
  - `E. coli succinate knockout`
  - `M. tuberculosis essentiality`
  - `drug-target prioritization`
- note 对 `06` 证据的判定是：
  - `systems-biology tasks 支持 06`
  - 置信度 `高`

本轮判断：

- 当前 residual 来自 general-system / self-reinforcing research-agent 外观，而不是 `06` 对象证据不足。
- 在二级类层面，`06.01` 已可视为当前稳定归位。

### 3.5 `ASD-0787`

- `06`：移出 queue，维持 `06.01`

关键依据：

- note 已冻结为：
  - `scientific_object_modules=03;04;06`
  - `primary_module_for_filing=03`
- `06` 的 module assignment evidence 已明确写为：
  - `biology/protein-engineering case coverage`
- 该 note 还明确说明，旧的 `01.04` body language 已被当前 concrete multi-module overlay supersede。

本轮判断：

- 这篇论文的 residual 也已经不再是“06 是否成立”，而是平台 / multitool 外观是否会让人本能上继续保守。
- 在当前二级类复核层面，继续留队的收益已经很低。

### 3.6 `ASD-0844`

- `06`：移出 queue，维持 `06.03`

关键依据：

- note 已冻结为：
  - `scientific_object_modules=01;06`
- `06` 侧 module assignment evidence 非常具体：
  - `pan-cancer single-cell atlas`
  - `Treg anchor`
- note 已明确指出：
  - 平台外观很强，但 PDF 已明确支持 `01;06` 的对象级运行
  - cases are `a first empirical reading`, not a benchmark sweep

本轮判断：

- 这篇论文的风险在“不要夸大成成熟 benchmark 论文”，不在 `06` 对象落位是否成立。
- 因此 `06.03` 可以从 secondary queue 中正式收口。

## 4. 本轮后的整体状态

本轮完成后：

- `07 tertiary queue = 0`
- `04 secondary queue = 0`
- `06 secondary queue = 0`
- `03 secondary queue = 1`

当前唯一剩余的 residual 是：

- `ASD-0673`

它和前面这些样本不同，原因不再是 benchmark-heavy surface 或 platform appearance，而是：

1. `03` 侧确实成立
2. 但 `03.02` 与 `03.03` 之间仍存在 exact-slot pull

因此它值得单独做最后一轮判断，而不是继续和其他 broad residual 混在一起。

## 5. 下一步建议

下一步最自然的动作是：

1. 单独处理 `ASD-0673`
2. 如果 `ASD-0673` 能收口，则写最终阶段性总结
3. 如果 `ASD-0673` 仍保留 medium，也应写明它为何已不影响整体主干高置信度收口
