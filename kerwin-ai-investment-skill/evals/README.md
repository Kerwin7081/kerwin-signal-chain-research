# Kerwin AI Investment Skill — Runtime Evals (current v0.3.3)

目标：验证当前 Skill v0.3.3 的 **Research Depth + Evidence Integrity**，包括新增的历史数据时点、现金到账状态、官方日期和业务范围口径检查；不是比较文风。以下是测试标准，**不代表所有 runtime 已经达到通过门槛**。

固定五例：
1. 长鑫科技 — A 股 Memory / Evidence & Freshness
2. 中际旭创 — A 股 Optical / Global Chain Mapping
3. 宇树科技 — Physical Agent / Missing Unit Economics
4. Snowflake — Enterprise Software / Earnings & Value Capture
5. 5GW AI Infrastructure Contract — Controlled synthetic contract test

当前 v0.3.3 使用 `RUNTIME-EVAL-RUBRIC-v0.3.3.md`，每例 20 分；`RUNTIME-EVAL-RUBRIC-v0.3.2.md` 仅供历史测试回溯。

## Release Gate

v0.3.3 → v0.4.0 前至少满足：
- 每个 runtime 五例平均 ≥ 16/20
- 无 Critical Failure
- Evidence Integrity 单项平均 ≥ 1.6/2
- 同一案例跨模型的 Thesis Direction 不出现无证据的反向漂移
- FACT / ESTIMATE / INFERENCE 分类错误率持续下降

v0.4.0 的重点才是 Cross-Model Consistency；本版本先锁证据纪律。

**版本与结果边界：** 本页只说明当前测评入口及晋级门槛。历史评测报告需按其实际 Skill、rubric、runtime 和测试日期解释，不能因为版本指向更新就追认旧结果为当前版本验证。正式晋级还须检查现有真实回归结果与 Critical Failure。
