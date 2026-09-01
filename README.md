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

> 个人级 Agent 工程：让 Agent 长期跑得对，比演示它能干什么更难。
