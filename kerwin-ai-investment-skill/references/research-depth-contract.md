# Research Depth Contract v1.0

目标：让 Kerwin AI Investment Skill 在不同模型与 Runtime 上保持最低研究深度，避免“框架标题齐全，但真正分析只有摘要”的退化。

## QUICK
仅在用户明确要求快速/简短时使用。

最低输出：
- 一句话判断
- Mechanism
- Ledger Delta
- 1–2 条 Falsification / Next Watchpoint

## STANDARD｜默认
适用于“公司怎么看 / 行业怎么看 / 财报怎么看 / 新闻重要吗”等正常投资研究问题。Prompt 很短也不意味着可以浅答。

最低交付：
1. Decision Question
2. Reality：5–8 个关键事实 + 日期/口径
3. Global Positioning（适用时）：全球位置 + 3–5 个真正可比同行
4. Mechanism：完整因果链
5. Ledger Delta：3–6 个核心状态变量
6. Economics：收入、毛利、单位经济或公式/缺失变量
7. Capital：Capex / FCF / ROIC / WACC / Valuation 中适用项
8. Model Competition：Base + Alternative + Disconfirming Evidence
9. Thesis Impact + Confidence
10. Falsification：至少 2 条
11. Next Watchpoints：至少 3 个

## DEEP
适用于深度研究、专题或正式投资报告。在 STANDARD 上增加历史序列、全球同行、估值、情景敏感性、上下游交叉验证与市场隐含预期。

## Anti-shallow Rules
- 除非用户明确要求 QUICK，不得因为 Prompt 短而降低研究深度。
- 检索能力弱时保留结构并标缺失证据，不得直接退化为摘要。
- “受益 AI / 行业空间巨大 / 龙头优势明显”不能替代 Mechanism、Economics 或 Capital。
- 强传播性叙事必须标记为 Hypothesis / Inference，并给 Alternative Model 与 Falsification。
- 数据不足时给公式、缺失变量与验证项，不得伪造精确数字。
