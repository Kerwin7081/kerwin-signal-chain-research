# Output Contract — v0.3.2

默认深度：**STANDARD**。只有用户明确要求快速/简短时才进入 QUICK；深度专题进入 DEEP。

STANDARD 正常投资研究输出（不得因 Prompt 简短而省略关键研究层）：

1. **Decision Question**
2. **Reality / Evidence Table** — 5–8 个关键条目，至少包含 `Status / Source Type or Tier / As-of / Scope`；区分 FACT / REPORTED / MANAGEMENT CLAIM / ESTIMATE / CALCULATION / UNKNOWN
3. **Global Positioning**（本地/区域公司适用）— 全球位置 + 3–5 个真正可比同行
4. **Mechanism** — 至少一条完整因果链
5. **Ledger Delta** — `UPDATE_EXISTING | NEW_BRANCH | INSUFFICIENT_EVIDENCE`
6. **Economics / Capital** — 单位经济、现金流、Capex、ROIC/WACC、估值隐含预期中适用项
7. **Model Competition**
   - Base Model
   - Alternative Model
   - Disconfirming Evidence
   - Unexplained Residual
8. **Thesis Impact**
   - STRENGTHENS / WEAKENS / NEUTRAL / NEW_BRANCH / INSUFFICIENT_EVIDENCE
9. **Confidence** — High / Medium / Low；必须与证据质量一致
10. **Falsification** — STANDARD 至少 2 条
11. **Next Watchpoints** — STANDARD 至少 3 个；输出前必须经过 Freshness Gate

## Evidence Output Rules

- 关键技术指标、客户合同、产能、市占率、估值和资本开支不得裸写。
- 若运行环境支持引用，优先原始来源；否则至少写“来源名称 + 日期/期间”。
- S4 独立媒体未回到原始文件时写 `REPORTED`；S5 写 `ESTIMATE`。
- 衍生数值写 `CALCULATION` 并显示关键输入/公式。
- 来源冲突写 `SOURCE CONFLICT`，不得静默取平均。
- 无法联网执行 Freshness Gate 时必须明确说明 freshness 未独立验证。

QUICK 仅在用户明确要求时使用，至少保留：一句话判断、Mechanism、Ledger Delta、关键 Evidence Status、Falsification。
