# Benchmarking Psychological Dynamics in Generative Agents

**论文信息**

- ID：ASD-0921
- 标题：Benchmarking Psychological Dynamics in Generative Agents
- 作者：Vaid, Sumer S.; Whillans, Ashley V.
- 年份：2026
- 来源 / venue：arXiv preprint
- DOI / arXiv / URL：https://arxiv.org/abs/2610.04246
- 一手阅读来源：https://arxiv.org/abs/2610.04246
- 来源层级：全文
- 阅读版本：对应缓存来源版本，参见Evidence Log
- 阅读版本题名：Benchmarking Psychological Dynamics in Generative Agents
- 原始全文缓存：C:/Users/20683/Desktop/综述/.tmp_asd_pdfs/source_F/2610.04246.pdf
- PDF / 本地文件路径：Reference_PDF/11_Social_Behavioral_Economic_and_Knowledge_System_Sciences/Vaid_2026_Psychological_Dynamics.pdf
- 当前状态：background_only
- 阅读日期：2026-10-22
- 笔记作者：Codex（读者证据包经主控审核整合）

## Evidence Log

| 判断项 | 结论 / 原文概括 | 证据位置 | 可信度 |
|---|---|---|---|
| 纵向设计 | 固定身份persona经历逐步变化的事件，以多个时间点状态形成轨迹。 | §3 Creating the Benchmark | high |
| 数据生成 | event model一次性生成叙事；全部评测模型读取相同文本并打心理状态分。 | §3.2；§4 Experimental Setup | high |
| 样本 | 使用300个synthetic employees，测量六个离散心理状态时间点。 | §4 Experimental Setup | high |
| 效度指标 | 内部效度测重复测量结构，外部效度测已知心理关系方向。 | §3.3 Two Dimensions of Psychological Realism | high |
| 结果 | 方向一致率84.3%，34项方差结构中26项复现，但个体内相关及分布仍较差。 | Abstract；§5 | high |
| 时间限制 | 六天轨迹不足以识别个体内自回归关系。 | §5 Results；§6 Discussion | high |
| Agent判断 | 评测模型只处理固定叙事并输出评分；无计划、工具调用或自主行动决策。 | §3–4 protocol | high |

## 0. 摘要翻译

本文提出心理动态benchmark：基于公开心理学norm构造300个synthetic employees，由固定模型生成统一的连续日常叙事，再让36个模型在六个时间点给心理状态评分。多数模型能够恢复已有心理关系方向，但较难复现个体内相关和分布结构。所谓generative agents是被模拟persona；评测模型没有执行多步社会行动。

## 1. 是否纳入本综述

### 1.1 Agent 判定

- 当前判断：background_only；读者建议：background_only。
全文流程是模型读取同一批固定叙事并输出心理评分；没有计划生成、工具使用、自主行动选择或环境反馈策略循环。纵向事件序列本身不足以满足多步Agent行动标准，因此列background_only。

### 1.2 排除风险检查

若作为心理学背景可展示于11.04；但不能作为核心Agent文献，因为被测LLM只读固定叙事并评分，没有多步Agent行动循环。不能仅凭标题Generative Agents纳入。
完整闭环不是纳入门槛；科研目标、多步行动、至少一项Agent能力及明确科研角色须同时成立。

## 2. 科学领域归类

### 2.1 科学对象模块归类

- 科学对象模块：11
- 覆盖模式：single_module
- 独立01.04存放区：none
- Primary module for filing：11（仅归档，不替代多模块事实）
- 模块内分类路径：11.04
- 分类深度：03/04使用二级；06/07使用固定三级；其余沿用现有树。
- 分类状态：原文证据复核

### 2.2 对象优先判定

对象为工作场景心理动态与计算人格模拟。样本为300个synthetic employees、36个模型及六个状态时间点。指标包括内部效度统计结构、外部关系方向一致性。摘要报告方向一致率84.3%，34项方差结构中26项复现；within-person相关和分布结构仍不足。全文指出六天轨迹不足以估计个体内自回归。

### 2.3 容易混淆的边界

若作为心理学背景可展示于11.04；但不能作为核心Agent文献，因为被测LLM只读固定叙事并评分，没有多步Agent行动循环。不能仅凭标题Generative Agents纳入。

## 3. Agent 系统与科研流程角色

全文流程是模型读取同一批固定叙事并输出心理评分；没有计划生成、工具使用、自主行动选择或环境反馈策略循环。纵向事件序列本身不足以满足多步Agent行动标准，因此列background_only。

科研流程与自主能力以本文实际行动和工具调用为依据：

根据人类规范初始化synthetic population；event model一次性生成身份描述和连续叙事；各待测模型在相同叙事的六个时间点预测心理状态；计算重复测量结构与心理关系方向一致性。

## 4. 方法设计

### 4.1 方法动机与设计

提出以纵向心理测量而非单次问卷检验synthetic persona真实性，并揭示模型难以保持个体内动态。

### 4.2 系统流程与组件

根据人类规范初始化synthetic population；event model一次性生成身份描述和连续叙事；各待测模型在相同叙事的六个时间点预测心理状态；计算重复测量结构与心理关系方向一致性。

## 5. 实验与验证

### 5.1 验证方式、对象及任务

对象为工作场景心理动态与计算人格模拟。样本为300个synthetic employees、36个模型及六个状态时间点。指标包括内部效度统计结构、外部关系方向一致性。摘要报告方向一致率84.3%，34项方差结构中26项复现；within-person相关和分布结构仍不足。全文指出六天轨迹不足以估计个体内自回归。

### 5.2 基线、指标与结果

对象为工作场景心理动态与计算人格模拟。样本为300个synthetic employees、36个模型及六个状态时间点。指标包括内部效度统计结构、外部关系方向一致性。摘要报告方向一致率84.3%，34项方差结构中26项复现；within-person相关和分布结构仍不足。全文指出六天轨迹不足以估计个体内自回归。

### 5.3 科学贡献与证据强度

提出以纵向心理测量而非单次问卷检验synthetic persona真实性，并揭示模型难以保持个体内动态。

证据层级：原始全文支持；作者报告结果不等于独立复现。

## 6. 与已有工作的关系

连接computational replicas、心理测量和synthetic population/LLM模拟评估。

## 7. 局限性与风险

序列只有六天，个体内自回归关系不可识别；部分效度目标仍是文献占位关系。评估对象是模型评分能力，不是Agent自主行动。

## 8. 对综述写作的价值

可用作synthetic persona纵向真实性的背景材料及Agent纳入边界反例。

推荐引用强度：背景引用。

## 9. 总结

### 9.1 一句话概括

评测模型生成的心理动态

### 9.2 速记版 pipeline

根据人类规范初始化synthetic population；event model一次性生成身份描述和连续叙事；各待测模型在相同叙事的六个时间点预测心理状态；计算重复测量结构与心理关系方向一致性。

### 9.3 标注字段汇总

```text
paper_id=ASD-0921
inclusion_status=background_only
scientific_object_modules=11
object_coverage_mode=single_module
general_method_bucket=none
primary_module_for_filing=11
module_taxonomy_codes=11.04
source_level=fulltext
fulltext_followup_required=false
```

### 全文后续要求

本轮已读原始全文并完成对象分类；无需为纳入/分类另做全文补读。具体引用时仍需回查相应原文位置。
