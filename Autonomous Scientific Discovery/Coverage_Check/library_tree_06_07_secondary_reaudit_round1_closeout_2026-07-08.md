# library_tree_06_07_secondary_reaudit_round1_closeout_2026-07-08

日期：`2026-07-08`

## 1. 本轮范围

本轮正式进入：

- `Coverage_Check/library_tree_secondary_tertiary_reaudit_plan_03_04_06_07_2026-07-08.md`
  中的第二优先批次 `06 / 07` 边界样本

本轮没有试图一次清空全部 `06 secondary medium queue`，而是先处理最值得优先压缩的一小批高价值边界样本：

- `ASD-0254`
- `ASD-0660`
- `ASD-0676`
- `ASD-0871`
- 并同步复核但暂不出队：
  - `ASD-0659`
  - `ASD-0663`
  - `ASD-0856`
  - `ASD-0866`

本轮继续遵守：

- 只按原始图书馆学二级类树
- 不修改 owner fact source
- 只更新研究层 `Coverage_Check` 结果与 queue

## 2. 本轮结论

本轮共复核 `8` 篇高优先 `06 / 07` 边界样本，其中：

- `4` 篇可提升为当前可接受的高置信度 `06` 二级类归位
- `4` 篇继续保留在 `medium queue`

本轮后：

- `06 secondary medium queue: 16 -> 12`
- 总 queue: `40 -> 36`

## 3. 提升为高置信度的样本

### 3.1 `ASD-0254` 维持 `06.03`

当前 `06` 侧证据主要来自：

- `transcriptomics`
- `RNA-seq`
- `single-cell sequencing`
- `gene-expression`

这组对象明显更贴近原始树里的：

- `06.03 生物技术相关科学`

而不是宽泛的 `06.01 生物学基础`。

同时，这篇论文虽然带有 biomedical workflow 外观，但 `06` 侧并不是虚弱 benchmark slice，而是明确的 omics / scRNA / gene-expression research objective。

因此：

- 维持 `06.03`
- 从 `medium queue` 移出

### 3.2 `ASD-0660` 维持 `06.03`

当前 `06` 侧证据主要来自：

- `GWAS`
- `Biomni-Eval / Biomni-Eval1`

在原始树口径下，`GWAS` 更适合被理解为：

- `06.03` 下的 genomics-facing object coverage

而 `07` 侧的 rare-disease diagnosis 则单独支撑医学模块，不会吞掉 `06` 侧。

因此：

- `06` 侧当前维持 `06.03`
- 可以从 `medium queue` 移出

### 3.3 `ASD-0676` 维持 `06.03`

当前 `06` 侧证据主要来自：

- `PTM-aware degrader target nomination`
- `15 POIs / 189 interface sites`
- `PTM perturbations`
- `protein / PTM biology`

这组对象更稳地落在：

- `06.03 生物技术相关科学`

尤其是 protein / structure / PTM 这一支，而不是仅仅停留在抽象生命科学对象。

因此：

- 维持 `06.03`
- 从 `medium queue` 移出

### 3.4 `ASD-0871` 维持 `06.03`

当前 `06` 侧证据主要来自：

- `malaria single-cell biology`
- `protein folding pathways`

在原始树口径下，这比 `06.01` 更自然地落在：

- `06.03`

因为它带有清楚的单细胞 / 蛋白对象切面，而不是普通 broad biology。

因此：

- 维持 `06.03`
- 从 `medium queue` 移出

## 4. 暂保留为 medium 的样本

### 4.1 `ASD-0659`

这篇的 `06` 侧真实存在，但现在的主要压力已经不是“有没有 `06` 证据”，而是：

- 它更像 `06.01` 的 broad biological foundation
- 还是更像 `06.03` 的 protein / peptide / structural-biology facing object

由于全文还是一个很强的 distributed scientific-discovery ecosystem，本轮暂不把它提升出队。

### 4.2 `ASD-0663`

`06` 侧证据同时来自：

- `ProteinGym`
- `protein engineering`
- `single-cell omics`

这使它在 `06.01` 与 `06.03` 之间同时受拉。

本轮结论不是 `06` 证据不足，而是：

- 当前 `06` 二级位还没有被唯一锁死

因此继续保留。

### 4.3 `ASD-0856`

`06` 侧证据同时来自：

- `DiscoveryBench freshwater-fish / biological datasets`
- `SEA-AD human-brain cellular atlas`

前者更像 broad biology，后者又带有 atlas / cell-level pressure，因此：

- `06.01` 与 `06.03` 都还有解释力

本轮继续保留。

### 4.4 `ASD-0866`

`06` 侧主要来自：

- `functional DNA sequences`

而整篇论文的主压力明显仍在 `07`。

因此目前的主要问题是：

- `06` 侧到底应理解为 `06.01` 的 molecular / genetic object
- 还是继续留在当前 `06.03`

本轮暂不提前冻结。

## 5. 本轮后的 queue 变化

本轮前：

- `03 secondary = 12`
- `04 secondary = 12`
- `06 secondary = 16`
- `07 tertiary = 0`
- `total = 40`

本轮后：

- `03 secondary = 12`
- `04 secondary = 12`
- `06 secondary = 12`
- `07 tertiary = 0`
- `total = 36`

## 6. 下一步建议

接下来有两条自然路径：

1. 继续把剩余 `06 secondary` 中真正属于 `06 / 07` 边界的样本压缩完
2. 然后再切到 `03 / 04` 边界样本

当前最值得继续看的 `06` 剩余边界样本是：

- `ASD-0659`
- `ASD-0663`
- `ASD-0856`
- `ASD-0866`

