# library_tree_03_04_secondary_reaudit_round1_closeout_2026-07-08

日期：`2026-07-08`

## 1. 本轮范围

本轮正式进入：

- `Coverage_Check/library_tree_secondary_tertiary_reaudit_plan_03_04_06_07_2026-07-08.md`
  中的第三优先批次 `03 / 04` 边界样本

本轮优先处理最容易形成稳定二级类落点的一组高价值样本：

- `ASD-0060`
- `ASD-0660`
- `ASD-0866`
- `ASD-0871`

它们共同覆盖了：

- broad scientific system 外观下的真实 chemistry / materials slice
- molecule-vs-material 双侧对象
- virtual-screening / ChemBench / MatSciBench / inorganic-materials cases
- cross-domain scientific-discovery system 中仍可稳定抽出的 `03` / `04` 对象

## 2. 本轮结论

本轮复核 `8` 条 queue 行：

- `03` 侧 `4` 条
- `04` 侧 `4` 条

这 `8` 条全部可以提升为当前可接受的高置信度二级类归位，并全部移出 `medium queue`。

本轮后：

- `03 secondary medium queue: 12 -> 8`
- `04 secondary medium queue: 12 -> 8`
- `combined queue: 32 -> 24`

## 3. 提升为高置信度的样本

### 3.1 `ASD-0060`

- `03`：维持 `03.04`
- `04`：维持 `04.04`

依据：

- `03` 侧来自 `ChEMBL molecule bio-activity / chemical-space optimization`
- `04` 侧来自 `nanohelix optimization` 与 `superconductor critical-temperature optimization`

虽然论文整体是 principle-aware cross-domain platform，但这两个对象侧都已足够具体，不再只是泛 demo。

### 3.2 `ASD-0660`

- `03`：维持 `03.04`
- `04`：维持 `04.01`

依据：

- `03` 侧来自 `ChemBench` 中分子性质与早期 virtual-screening slice
- `04` 侧来自 `MatSciBench` 与 `electrochemical-cell examples`

这篇的系统平台感很强，但 `03` / `04` 两个对象侧已经都有清楚 benchmark object coverage。

### 3.3 `ASD-0866`

- `03`：维持 `03.04`
- `04`：维持 `04.02`

依据：

- `03` 侧来自 `antibiotic molecular design`
- `04` 侧来自 `inorganic materials design`

这里的 `03` / `04` 不是弱附带标签，而是正文 main design applications 中明确列出的对象任务。

### 3.4 `ASD-0871`

- `03`：维持 `03.04`
- `04`：维持 `04.03`

依据：

- `03` 侧来自 `self-assembling peptides`
- `04` 侧来自 `functionalized graphene interfaces / confined water dynamics`

虽然 Denario 是极宽跨域系统，但这两个对象示例都已经足够具体，可作为稳定 research-layer secondary placement 使用。

## 4. 暂不出队的残留样本

本轮之后，`03 / 04` 里仍值得继续保留的压力样本主要是：

### 4.1 `03` 剩余 `8` 条

- `ASD-0004`
- `ASD-0539`
- `ASD-0662`
- `ASD-0673`
- `ASD-0731`
- `ASD-0857`
- `ASD-0869`
- `ASD-0870`

它们主要对应：

- general-system cross-domain pressure
- materials-primary with weak chemistry slice
- atomistic chemistry / catalysis exact落点不够唯一
- chemical-reaction extraction vs chemistry-centered discovery
- equation-discovery benchmark pressure

### 4.2 `04` 剩余 `8` 条

- `ASD-0062`
- `ASD-0085`
- `ASD-0511`
- `ASD-0673`
- `ASD-0787`
- `ASD-0857`
- `ASD-0869`
- `ASD-0870`

它们主要对应：

- workflow substrate / instrument-operation support
- 04 side weaker than 06 primary
- atomistic materials exact二级位仍有拉扯
- equation-discovery benchmark pressure

## 5. 本轮对计划推进的意义

到本轮为止：

1. `07` 三级类 `medium queue` 已清空
2. `06 / 07` 最关键边界样本已基本压完
3. `03 / 04` 中最容易稳定下来的高价值样本已完成首轮清理

因此，后续可以继续做：

- `03 / 04` 残留 `16` 条 pressure 样本的第二轮压缩

