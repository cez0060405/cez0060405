# cez0060405

### I run a personal AI agent like a production system

我在 Windows 上长期跑一个个人 AI 助手（Hermes Agent），像运维生产系统一样维护它，已经跑了好几个月。所有东西都是真跑过、踩坑踩出来的，不是演示。

**📌 实战资产**

- 🧪 **[personal-agent-ops](https://github.com/cez0060405/personal-agent-ops)** —— 决策回归测试（125 道选择题，换模型后准确率 91%→97%）、模型偷换检测器、断流看门狗、技能工程样例
- 🗣️ **[communication-protocol-setup](https://github.com/cez0060405/communication-protocol-setup)** —— 让任何 AI 助手学会怎么跟你沟通。交互式问答配置，不是静态文档；支持多工具同步、指标验证、重新校准
- 🧠 **[hermes-lcm](https://github.com/cez0060405/hermes-lcm)** —— Hermes 的无损上下文管理插件
- 📋 **[kanban-comment-delegation](https://github.com/cez0060405/kanban-comment-delegation)** —— 多 agent 看板的评论驱动任务委派
- 🚦 **[kanban-concurrency-gate](https://github.com/cez0060405/kanban-concurrency-gate)** —— 多 agent 看板的 AIMD 动态并发闸门

**🔧 开源贡献**

- 🏆 **[NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent)** —— 24.1 万 star 项目，我是**第 2821 位贡献者**（[graphs/contributors](https://github.com/NousResearch/hermes-agent/graphs/contributors)）
- ✅ **已合并：启动不再卡死** —— 修复 Windows 上启动时孤儿进程清理过慢导致的黑屏/卡 5 分钟（[#101929](https://github.com/NousResearch/hermes-agent/pull/101929)）。我的 [#100774](https://github.com/NousResearch/hermes-agent/pull/100774) 因没带测试被关闭，但维护者**认可代码价值，专门抢救（salvage）cherry-pick 合并**，补测试后**全绿通过**，作者身份保留
- 还有 2 个桌面端修复在等合并：
  - **"问一次答三次"** —— 工具调用过程中 AI 的中间过程不再和最终答案长得一样，加了"Working"标签区分（[#100777](https://github.com/NousResearch/hermes-agent/pull/100777)）
  - **断连诊断** —— 给 WebSocket 断连加了心跳计数和静默时长日志，方便排查周期性掉线（[#100779](https://github.com/NousResearch/hermes-agent/pull/100779)）

> 个人级 Agent 工程：让 Agent 长期跑得对，比演示它能干什么更难。
