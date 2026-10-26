# ChemMate: an autonomous research mate for the full computational chemistry research lifecycle, from ideation to manuscript

**论文信息**

- ID：ASD-0891
- 标题：ChemMate: an autonomous research mate for the full computational chemistry research lifecycle, from ideation to manuscript
- 作者：Guangsheng Liu; Leshen Zhang; Xiao Ma; I-Shan Tsai; Jinyi Zhang; Wan-Lu Li
- 年份：2026
- 来源 / venue：ChemRxiv
- DOI / arXiv / URL：https://doi.org/10.26434/chemrxiv.15006055/v1
- 一手阅读来源：https://doi.org/10.26434/chemrxiv.15006055/v1
- 来源层级：仅摘要/官方页面，尚未完成全文阅读
- 阅读版本：对应缓存来源版本，参见Evidence Log
- 阅读版本题名：ChemMate: an autonomous research mate for the full computational chemistry research lifecycle, from ideation to manuscript
- 原始全文缓存：未取得
- PDF / 本地文件路径：未归档PDF
- 当前状态：needs_review
- 阅读日期：2026-10-22
- 笔记作者：Codex（读者证据包经主控审核整合）

## Evidence Log

| 判断项 | 结论 / 原文概括 | 证据位置 | 可信度 |
|---|---|---|---|
| Agent workflow | About 200 expert-protocol skills, idea pipeline, research knowledge graph and native multi-cluster orchestration combine across the research lifecycle. | Crossref registered abstract | high |
| Human oversight | Structure-check and job-submission gates require researcher inspection/correction/approval. | Crossref registered abstract | high |
| Catalysis objects | Electrocatalysis, non-thermal plasma catalysis, homogeneous asymmetric catalysis and isolated-Pd CO-reduction mechanism are reported. | Crossref registered abstract, campaign results | high |
| Drug-discovery object | Protease virtual screen returned 100 interference-clean hits at 16.5-fold enrichment. | Crossref registered abstract, virtual-screen result | high |
| Potential materials boundary | Machine-learned DFT Hamiltonian band-structure error decreased 491 to 101 meV, but abstract omits the concrete material/composition; this alone does not establish module 04. | Crossref registered abstract, first campaign result | high |
| Source access limit | Official full-text and PDF routes returned HTTP 403 challenge HTML, not article content. | ChemRxiv full/PDF routes tested 2026-10-22 | high |

## 0. 摘要翻译

Crossref注册摘要描述ChemMate：约200个专家协议技能、应用/方法/理论创意管线、类型化研究知识图与多集群计算编排，支持从构想到论文的计算化学研究。结构检查和作业提交由研究者批准。五个campaign涉及电催化、非热等离子体催化、均相不对称催化及生物分子药物发现。摘要给出：Agent调整指标后将band-structure error由491降至101 meV；等离子体动力学模型复现实测乙烯/乙炔比；不对称催化选择性预测与晶体学assignment一致且超过99% ee；蛋白酶虚拟筛选获得100个低干扰hits、16.5倍enrichment；并重建孤立Pd CO还原质子供应机理。

## 1. 是否纳入本综述

### 1.1 Agent 判定

- 当前判断：needs_review；读者建议：included。
摘要明确多步骤研究构想、技能编排、计算引擎和跨集群工具执行，并展示多个实际计算化学campaign及结果；人工审批门限定自主性，但不否定Agent角色。

### 1.2 排除风险检查

03.03由电/等离子体/均相催化与CO还原机制结果支持；蛋白酶虚拟药筛选有具体药物发现结果，支持07.04.01。04仅为待核边界：band-structure error属材料电子结构常见指标，但摘要未标明被研究的具体材料对象或独立材料campaign，故本证据包不将04作为已确认模块。若全文给出具体晶体/材料计算对象，可增补04.xx。
完整闭环不是纳入门槛；科研目标、多步行动、至少一项Agent能力及明确科研角色须同时成立。

## 2. 科学领域归类

### 2.1 科学对象模块归类

- 科学对象模块：03;07
- 覆盖模式：multi_module
- 独立01.04存放区：none
- Primary module for filing：03（仅归档，不替代多模块事实）
- 模块内分类路径：03.03; 07.04.01
- 分类深度：03/04使用二级；06/07使用固定三级；其余沿用现有树。
- 分类状态：来源受限，暂定

### 2.2 对象优先判定

摘要给出五项结果：电催化DFT哈密顿量中将band-structure error从491降到101 meV；非热等离子体模型复现测量乙烯/乙炔比；均相不对称催化对映选择性预测与晶体学指认相符且>99% ee；蛋白酶虚拟筛选100个低干扰hits、16.5-fold enrichment；孤立Pd CO还原机理多尺度重建。没有提供误差定义、基线和campaign拆解。

### 2.3 容易混淆的边界

03.03由电/等离子体/均相催化与CO还原机制结果支持；蛋白酶虚拟药筛选有具体药物发现结果，支持07.04.01。04仅为待核边界：band-structure error属材料电子结构常见指标，但摘要未标明被研究的具体材料对象或独立材料campaign，故本证据包不将04作为已确认模块。若全文给出具体晶体/材料计算对象，可增补04.xx。

## 3. Agent 系统与科研流程角色

摘要明确多步骤研究构想、技能编排、计算引擎和跨集群工具执行，并展示多个实际计算化学campaign及结果；人工审批门限定自主性，但不否定Agent角色。

科研流程与自主能力以本文实际行动和工具调用为依据：

摘要披露约200个专家协议技能受机器运行契约约束；Agent含应用/方法/理论创意流程、研究知识图和跨集群任务编排，每个作业保存机器/计算回执；结构检查及提交设人为审批门。各campaign的具体建模、工具和验证流程未由摘要充分说明。

## 4. 方法设计

### 4.1 方法动机与设计

把研究构想、专家协议技能、计算化学引擎和可追踪的多集群执行整合为生命周期Agent，并报告多个具体化学研究结果。

### 4.2 系统流程与组件

摘要披露约200个专家协议技能受机器运行契约约束；Agent含应用/方法/理论创意流程、研究知识图和跨集群任务编排，每个作业保存机器/计算回执；结构检查及提交设人为审批门。各campaign的具体建模、工具和验证流程未由摘要充分说明。

## 5. 实验与验证

### 5.1 验证方式、对象及任务

摘要给出五项结果：电催化DFT哈密顿量中将band-structure error从491降到101 meV；非热等离子体模型复现测量乙烯/乙炔比；均相不对称催化对映选择性预测与晶体学指认相符且>99% ee；蛋白酶虚拟筛选100个低干扰hits、16.5-fold enrichment；孤立Pd CO还原机理多尺度重建。没有提供误差定义、基线和campaign拆解。

### 5.2 基线、指标与结果

摘要给出五项结果：电催化DFT哈密顿量中将band-structure error从491降到101 meV；非热等离子体模型复现测量乙烯/乙炔比；均相不对称催化对映选择性预测与晶体学指认相符且>99% ee；蛋白酶虚拟筛选100个低干扰hits、16.5-fold enrichment；孤立Pd CO还原机理多尺度重建。没有提供误差定义、基线和campaign拆解。

### 5.3 科学贡献与证据强度

把研究构想、专家协议技能、计算化学引擎和可追踪的多集群执行整合为生命周期Agent，并报告多个具体化学研究结果。

证据层级：仅一手摘要支持，基线、消融与数值细节仍需全文核对。

## 6. 与已有工作的关系

与ASD-0010 El Agente、ASD-0022 ChemGraph、ASD-0061 xchemagents及ASD-0664自主计算催化相邻；ChemMate摘要强调多集群和跨campaign生命周期。

## 7. 局限性与风险

仅Crossref注册摘要可访问，ChemRxiv正式页面/PDF返回403挑战页面。安全关键输入与提交仍需研究者批准。各campaign方法、对照、基线和结果可复现性需全文确认。band-structure误差改进提示材料电子结构应用，但摘要未指明具体材料/器件对象，不能单凭误差项确定04。

## 8. 对综述写作的价值

有力压测计算化学Agent的多模块对象分类；同时提醒避免把DFT/band-structure方法结果自动当成具体材料对象覆盖。

推荐引用强度：暂不作为核心结论证据，待核后引用。

## 9. 总结

### 9.1 一句话概括

Agent执行计算化学研究任务

### 9.2 速记版 pipeline

摘要披露约200个专家协议技能受机器运行契约约束；Agent含应用/方法/理论创意流程、研究知识图和跨集群任务编排，每个作业保存机器/计算回执；结构检查及提交设人为审批门。各campaign的具体建模、工具和验证流程未由摘要充分说明。

### 9.3 标注字段汇总

```text
paper_id=ASD-0891
inclusion_status=needs_review
scientific_object_modules=03;07
object_coverage_mode=multi_module
general_method_bucket=none
primary_module_for_filing=03
module_taxonomy_codes=03.03; 07.04.01
source_level=abstract_only
fulltext_followup_required=true
```

### 全文后续要求

仍需取得/补读原始全文，核实方法、实验设置、数值结果及边界；本笔记不代表全文精读完成。
