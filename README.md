# Kerwin Signal-Chain Research

> 从一个被忽略的细节出发，顺藤摸瓜，按图索骥，把零散线索扩展为可验证、可跟踪的产业链研究。

**Kerwin Signal-Chain Research** 是一套面向投资研究、产业研究与AI辅助研究的公开方法论和任务流。它从财报电话会、客户案例、产品发布、监管文件或产业新闻中的一个高价值细节出发，依次完成实体核验、技术拆解、供应链扩展、投资映射、领先指标设计、网页发布和持续跟踪。

这不是一个自动给出股票结论的工具，而是一套用于提高研究深度、证据透明度和可复用性的研究框架。

## 核心链路

```text
细节发现
  → 实体核验
  → 证据分级
  → 技术架构拆解
  → 产业链扩展
  → 投资映射
  → 领先指标与证伪条件
  → 专题发布
  → 持续监测
```

## 为什么创建这个项目

这套方法起源于一次Alphabet财报电话会研究。管理层在大量财务与AI基础设施信息中提到了一家英国前沿实验室 **Ineffable Intelligence**。沿着这个名字继续追踪，我们连接起：

- David Silver与AlphaZero式强化学习；
- Agent之后的持续自主学习；
- Google Cloud A5X裸金属实例；
- NVIDIA Vera Rubin NVL72；
- Vera CPU、HBM4、网络、光互联、800V供电与存储分层；
- 从样机、测试到规模交付和收入确认的验证路径。

这体现了Kerwin一贯的研究方法：**电话会不仅用于核对收入与指引，更要从客户、产品和技术细节中发现新的产业线索。一个细节可以扩展为一条产业链，也可以转化为一组持续监测的领先指标。**

## 适用场景

- 财报电话会中出现陌生客户、合作方或产品名称；
- 新芯片、机柜、网络、电力或存储架构可能带来系统性升级；
- 单个客户案例可能代表更广泛的行业需求；
- 需要区分官方事实、公司自报、研究推断与网传材料；
- 需要把零散讨论整理为结构化专题和持续跟踪清单；
- 需要将研究过程交给AI Agent执行，同时保留人工判断边界。

## 仓库结构

```text
.
├── SKILL.md                         # 可直接复用的Skill规范
├── templates/
│   ├── evidence-ledger.md           # 证据分级与来源台账
│   └── research-output.md           # 标准研究输出模板
├── examples/
│   └── ineffable-rubin-a5x.md       # 从电话会细节扩展到产业链的案例
├── CONTRIBUTING.md                  # 贡献方式
├── SECURITY.md                      # 隐私与安全边界
└── LICENSE                          # CC BY 4.0
```

## 快速使用

将以下指令交给研究员或AI Agent：

```text
使用Kerwin Signal-Chain Research方法分析这个线索。
先定位原始出处并进行证据分级，再核验公司、人物和产品实体；
按照“应用需求—工作负载—芯片—机柜—网络—存储—电力—云平台”的顺序拆解；
区分已经确认、公司自报、研究推断和网传材料；
最后给出投资映射、领先指标、证伪条件和后续监测清单。
```

完整执行规范见 [`SKILL.md`](./SKILL.md)。

## 研究原则

1. **从细节出发，不从宏大结论出发。**
2. **先核验事实，再扩展产业链。**
3. **计划、样机、测试、Preview、GA和规模收入必须严格区分。**
4. **系统级性能不得偷换成单芯片性能。**
5. **技术受益、收入受益、利润受益和估值受益分别判断。**
6. **所有结论都应绑定下一步验证信号和证伪条件。**

## 隐私边界

本仓库是一个与其他研究仓库完全分离的公开项目，只包含：

- 公开方法论；
- 通用模板；
- 已公开案例；
- 不涉及客户身份和账户的数据。

本仓库不应提交：客户资料、持仓、交易记录、内部邮件、未公开财务数据、访问密钥、私人研究笔记或主站后台文件。详细规则见 [`SECURITY.md`](./SECURITY.md)。

## 项目属性

这是Kerwin第一次将个人研究方法整理为可公开复用的GitHub项目。它同时是：

- 一套投资研究Skill；
- 一个AI辅助研究工作流；
- 一个个人研究能力产品化的案例；
- 一个从使用AI到设计AI任务系统的实践样本。

## English summary

Kerwin Signal-Chain Research is an evidence-first workflow for expanding a small but meaningful disclosure into a structured industry-chain research project. It moves from signal discovery to entity verification, technical decomposition, supply-chain mapping, investment implications, falsification criteria, publication, and ongoing monitoring.

Keywords: `investment research`, `earnings calls`, `industry chain`, `AI infrastructure`, `evidence grading`, `agent workflow`, `continual learning`, `NVIDIA Rubin`, `Google Cloud A5X`.

## License

Licensed under [Creative Commons Attribution 4.0 International](./LICENSE). You may reuse and adapt the framework with attribution to **Kerwin Signal-Chain Research**.

---

**Author:** Kerwin  
**Method:** 顺藤摸瓜 · 按图索骥 · 先证据后结论
