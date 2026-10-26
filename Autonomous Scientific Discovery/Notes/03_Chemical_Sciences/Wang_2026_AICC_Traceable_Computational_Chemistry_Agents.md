# A modular skill and orchestration framework for traceable agentic computational chemistry

**论文信息**

- ID：ASD-0890
- 标题：A modular skill and orchestration framework for traceable agentic computational chemistry
- 作者：Ruixing Wang; Jinhua Cai; Jin-Cheng Liu
- 年份：2026
- 来源 / venue：ChemRxiv
- DOI / arXiv / URL：https://doi.org/10.26434/chemrxiv.15005810/v1
- 一手阅读来源：https://doi.org/10.26434/chemrxiv.15005810/v1
- 来源层级：仅摘要/官方页面，尚未完成全文阅读
- 阅读版本：对应缓存来源版本，参见Evidence Log
- 阅读版本题名：A modular skill and orchestration framework for traceable agentic computational chemistry
- 原始全文缓存：未取得
- PDF / 本地文件路径：未归档PDF
- 当前状态：needs_review
- 阅读日期：2026-10-22
- 笔记作者：Codex（读者证据包经主控审核整合）

## Evidence Log

| 判断项 | 结论 / 原文概括 | 证据位置 | 可信度 |
|---|---|---|---|
| Framework description | AICC provides domain knowledge, per-code operational skills and orchestration procedures for general-purpose agents. | Crossref registered abstract, DOI 10.26434/chemrxiv.15005810/v1 | high |
| Evaluation task | Comparison uses real referee requests from Nature Communications papers and published computational-content extracts. | Crossref registered abstract | high |
| Evaluation setup | Two LLM evaluators apply a fixed document-level rubric to autonomous, reference-informed and published-extract outputs. | Crossref registered abstract | high |
| Reported scores | Autonomous GPT-5.5 means 64.8 and 65.5/100; after one human follow-up round 69.8 and 72.2; published extracts 72.6 and 54.7. | Crossref registered abstract | high |
| Unresolved object/action evidence | Abstract describes reports on reviewer requests but does not name concrete molecules or confirm actual execution of computational chemistry calculations. | Crossref registered abstract; inaccessible ChemRxiv full-text/PDF endpoints | high |
| Source access limit | Official routes returned HTTP 403 challenge HTML, not article text or PDF. | ChemRxiv full/PDF routes tested 2026-10-22 | high |

## 0. 摘要翻译

Crossref注册摘要称，AICC以通用化学知识、针对不同计算代码的操作技能和机器可读编排面，装备通用Agent开展计算研究。作者用Nature Communications论文审稿请求比较自主GPT-5.5 Agent、参考信息辅助后的Agent和已发表计算内容摘录；两个LLM评估者分别给自主Agent均分64.8和65.5/100，人类引导一轮后为69.8和72.2。摘要称执行报告与透明度较好，但理解审稿意图和选取计算规模仍是弱项。摘要未指明实际执行的具体化学对象或计算任务。

## 1. 是否纳入本综述

### 1.1 Agent 判定

- 当前判断：needs_review；读者建议：needs_review。
摘要支持工具技能、编排和受审稿请求驱动的多步计算工作角色，但未明确说明实验中是否运行了计算化学程序、完成具体分子/材料计算，还是仅重组与评价已发表计算内容，因此具体对象实验覆盖和核心Agent行动证据仍需全文确认。

### 1.2 排除风险检查

暂不硬化对象模块。若原文显示对具体分子/反应/催化对象执行计算并报告结果，可依对象归03.xx；若仅提供通用计算技能/Agent基准而无具体对象实验或案例，应进入01.04 general-method bucket。当前分类风险高于证据支持范围。 主控：03.01仅沿用现有暂存编目位置，不代表已确认化学对象覆盖。摘要不足以证明有具体对象，也不足以证明完全没有对象，故本轮不强行移入01.04；保持needs_review，不生成DCA/PMTA核心映射。
完整闭环不是纳入门槛；科研目标、多步行动、至少一项Agent能力及明确科研角色须同时成立。

## 2. 科学领域归类

### 2.1 科学对象模块归类

- 科学对象模块：03
- 覆盖模式：single_module
- 独立01.04存放区：none
- Primary module for filing：03（仅归档，不替代多模块事实）
- 模块内分类路径：03.01
- 分类深度：03/04使用二级；06/07使用固定三级；其余沿用现有树。
- 分类状态：来源受限，暂定

### 2.2 对象优先判定

摘要报告两个评估者对自主Agent的均分64.8、65.5/100；论文摘录对照为72.6、54.7；一轮人工后续引导的Agent得分69.8、72.2。评估者间排序受文档完整度影响。未报告具体化学对象或科学计算结果。

### 2.3 容易混淆的边界

暂不硬化对象模块。若原文显示对具体分子/反应/催化对象执行计算并报告结果，可依对象归03.xx；若仅提供通用计算技能/Agent基准而无具体对象实验或案例，应进入01.04 general-method bucket。当前分类风险高于证据支持范围。 主控：03.01仅沿用现有暂存编目位置，不代表已确认化学对象覆盖。摘要不足以证明有具体对象，也不足以证明完全没有对象，故本轮不强行移入01.04；保持needs_review，不生成DCA/PMTA核心映射。

## 3. Agent 系统与科研流程角色

摘要支持工具技能、编排和受审稿请求驱动的多步计算工作角色，但未明确说明实验中是否运行了计算化学程序、完成具体分子/材料计算，还是仅重组与评价已发表计算内容，因此具体对象实验覆盖和核心Agent行动证据仍需全文确认。

科研流程与自主能力以本文实际行动和工具调用为依据：

Crossref沉积摘要描述：通用Agent配备tool-agnostic科学知识、按软件代码组织的操作技能以及编排程序；自主GPT-5.5、参考信息辅助版本和Nature Communications论文已发表计算内容摘录在文档级固定量表下比较，由两个LLM评估。实际工具调用序列和化学计算任务不可从摘要确定。

## 4. 方法设计

### 4.1 方法动机与设计

提出可追踪的技能与编排框架，并对Agent计算内容报告、透明度及与论文内容的比较进行初步评估；能否作为具体化学Agent研究尚待原文。

### 4.2 系统流程与组件

Crossref沉积摘要描述：通用Agent配备tool-agnostic科学知识、按软件代码组织的操作技能以及编排程序；自主GPT-5.5、参考信息辅助版本和Nature Communications论文已发表计算内容摘录在文档级固定量表下比较，由两个LLM评估。实际工具调用序列和化学计算任务不可从摘要确定。

## 5. 实验与验证

### 5.1 验证方式、对象及任务

摘要报告两个评估者对自主Agent的均分64.8、65.5/100；论文摘录对照为72.6、54.7；一轮人工后续引导的Agent得分69.8、72.2。评估者间排序受文档完整度影响。未报告具体化学对象或科学计算结果。

### 5.2 基线、指标与结果

摘要报告两个评估者对自主Agent的均分64.8、65.5/100；论文摘录对照为72.6、54.7；一轮人工后续引导的Agent得分69.8、72.2。评估者间排序受文档完整度影响。未报告具体化学对象或科学计算结果。

### 5.3 科学贡献与证据强度

提出可追踪的技能与编排框架，并对Agent计算内容报告、透明度及与论文内容的比较进行初步评估；能否作为具体化学Agent研究尚待原文。

证据层级：仅一手摘要支持，基线、消融与数值细节仍需全文核对。

## 6. 与已有工作的关系

与ASD-0022 ChemGraph、ASD-0061 xchemagents主题接近；目前没有证据确认作者/系统重复。

## 7. 局限性与风险

仅可访问Crossref注册摘要。ChemRxiv DOI全页和PDF端点返回403挑战页面；没有找到公开作者代码仓库。对象、所用计算代码、任务数、人工干预程度和评分协议未知。

## 8. 对综述写作的价值

检验学科专用Agent技能与通用科研Agent方法/评测桶的边界；在取得全文前不应作为已确认03类核心文献。

推荐引用强度：暂不作为核心结论证据，待核后引用。

## 9. 总结

### 9.1 一句话概括

构建可追溯计算化学Agent

### 9.2 速记版 pipeline

Crossref沉积摘要描述：通用Agent配备tool-agnostic科学知识、按软件代码组织的操作技能以及编排程序；自主GPT-5.5、参考信息辅助版本和Nature Communications论文已发表计算内容摘录在文档级固定量表下比较，由两个LLM评估。实际工具调用序列和化学计算任务不可从摘要确定。

### 9.3 标注字段汇总

```text
paper_id=ASD-0890
inclusion_status=needs_review
scientific_object_modules=03
object_coverage_mode=single_module
general_method_bucket=none
primary_module_for_filing=03
module_taxonomy_codes=03.01
source_level=abstract_only
fulltext_followup_required=true
```

### 全文后续要求

仍需取得/补读原始全文，核实方法、实验设置、数值结果及边界；本笔记不代表全文精读完成。
