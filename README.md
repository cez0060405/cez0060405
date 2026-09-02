# cez0060405

### I run a personal AI agent like a production system

我在 Windows 上长期跑一个个人 AI 助手（Hermes Agent），像运维生产系统一样维护它，已经跑了好几个月。

**📌 实战资产：[personal-agent-ops](https://github.com/cez0060405/personal-agent-ops)**

都是真跑过、踩坑踩出来的东西：

- 🧪 **决策回归测试** —— 给 AI 助手出 125 道"选择题"，看它每次选得对不对。换模型后准确率从 91% 提到 97%
- 🔍 **模型偷换检测器** —— 有些订阅服务会悄悄用便宜模型冒充贵的，我写了个工具专门抓这个
- 🛡️ **断流看门狗** —— AI 助手跑着跑着突然断线，它自动检测并续上，全程留记录
- 🧩 **技能工程样例** —— 符合 Agent Skills 开放标准的技能写法

**🔧 开源贡献**

- [NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent) —— 给配置命令提过脚本化支持的建议（#96764），修过 Windows 文件路径问题（#80946）
- 最近提交了 3 个桌面端修复：
  - **启动不再卡死** —— 修复 Windows 上启动时孤儿进程清理过慢导致的黑屏/卡 5 分钟（[#100774](https://github.com/NousResearch/hermes-agent/pull/100774)）
  - **"问一次答三次"** —— 工具调用过程中 AI 的中间过程不再和最终答案长得一样，加了"Working"标签区分（[#100777](https://github.com/NousResearch/hermes-agent/pull/100777)）
  - **断连诊断** —— 给 WebSocket 断连加了心跳计数和静默时长日志，方便排查周期性掉线（[#100779](https://github.com/NousResearch/hermes-agent/pull/100779)）

> 个人级 Agent 工程：让 Agent 长期跑得对，比演示它能干什么更难。
