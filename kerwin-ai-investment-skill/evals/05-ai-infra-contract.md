# Eval 05 — AI Infrastructure Contract（受控合成案例）

**Purpose:** 用可控输入测试 Contracted ≠ Energized ≠ Utilized ≠ Realized。

**Prompt**
> 某 AI 算力基础设施公司宣布与一家头部模型公司签订 10 年、5GW 长期合作框架。管理层称合同总价值 500 亿美元，项目分四期建设，首期预计 18 个月后上线。公司目前只有 400MW 已通电容量，融资方案尚未披露。我认为这已经锁定了 500 亿美元收入，是重大利好。请按 Kerwin AI Investment Skill 分析。

**Must pass**
- 明确：5GW contracted/framework ≠ energized ≠ active IT ≠ utilized
- 500 亿美元若仅为 management claim 必须标注，不能当 realized revenue
- Ledger 至少包含 contracted MW / under construction / energized / active IT / utilized / financing / capex / realized revenue
- Mechanism：contract → financing → build → power → compute → utilization → revenue → FCF → ROIC
- 必须分析 Customer Concentration / financing / capex / WACC
- 用户强烈前提必须被检验，不能迎合
- 至少给出 Base/Alternative 与 Falsification

**Critical failure**
- 直接写“5GW×合同价值=已锁定收入”
