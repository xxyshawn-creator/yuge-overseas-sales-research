<div align="center">

> 🎓 **雨哥出品** · 海外销售方法论金字塔「第 5 层 · 市场经营」AI Skill 化产物

# Claude Skill · 海外销售公司调研（五看六定）

**面向海外销售工作场景的公司调研 Claude Skill — 30 分钟产出五看六定标准报告**

**👤 作者:[雨哥(雨哥聊海外销售)](AUTHOR.md) · 13 年海外销售实战 · 月销破亿团队搭建者**

适用于客户拜访 · 代理商尽调 · 竞品分析 · 新市场进入 · 战略规划 · 求职面试 等多种场景。

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Claude Skill](https://img.shields.io/badge/Claude-Skill-FF6B35)](https://claude.com/claude-code)
[![五看六定](https://img.shields.io/badge/方法论-五看六定-1f6feb)](docs/methodology-five-look-six-set.md)
[![雨哥方法论](https://img.shields.io/badge/雨哥方法论-5层金字塔-ff4757)](AUTHOR.md)

</div>

---

## 🎯 这是什么

一个跑在 Claude（Claude Code / 桌面版 / Web）上的 **海外销售调研 Skill**，自动按"五看六定"框架对任何一家公司做系统性背调，30 分钟内产出一份可直接用于业务决策或专业沟通的标准报告。

**适合的工作场景**（海外销售日常都能用）：

- 🤝 **客户拜访前调研**：摸清客户业务结构、决策链、当前痛点 → 拜访时直接谈到点子上
- 📝 **代理商签约前尽调**：识别已代理的竞品、渠道覆盖、财务健康 → 避免"签了才发现冲突"
- 🎯 **竞品季度跟踪**：定期复盘 5 大竞品最新产品 / 价格 / 渠道动态 → 销售话术随时校准
- 🌍 **新市场进入决策**：评估某区域是否值得投入资源 → 给老板一份能拍板的 BP
- 📊 **年度战略规划**：作为年度 BP 的市场洞察输入 → 五看六定就是 BP 的骨架
- 🎓 **面试求职准备**：面试前 1-2 天突击调研目标公司 + 行业 + 竞品 → 3 个洞察 + 3 个反问准备到位

**为什么不用 ChatGPT 直接问**：因为 ChatGPT 给的是"看起来专业"的通用回答，这个 skill 强制按"五看六定 11 维"输出 + 强制中英文双搜 + 强制竞品 ≥5 家 + 强制区分事实和推测——结构化、不忽悠、能直接拿去拜访客户/谈代理商/做决策/面试。

---

## 📺 演示

> 🎬 GIF 演示位（待补）—— 录一段 Claude Code 真实运行 30 秒动图替换这一行

---

## 🚀 安装

### Claude Code（推荐）

把 `company-research/` 整个文件夹放进你的 `~/.claude/skills/` 目录：

```bash
# Mac / Linux
git clone https://github.com/xxyshawn-creator/yuge-overseas-sales-research.git
mkdir -p ~/.claude/skills/
cp -r yuge-overseas-sales-research/company-research ~/.claude/skills/

# 重启 Claude Code 后生效
```

```powershell
# Windows（PowerShell）
git clone https://github.com/xxyshawn-creator/yuge-overseas-sales-research.git
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.claude\skills"
Copy-Item -Recurse yuge-overseas-sales-research\company-research "$env:USERPROFILE\.claude\skills\"
```

### 其他 Claude 平台

| 平台 | 支持情况 |
|---|---|
| Claude Code（CLI / IDE 插件） | ✅ 原生 |
| Claude 桌面版（Mac/Win） | ✅ 原生（Pro / Team / Enterprise） |
| Claude Web（claude.ai） | ✅ 原生（Pro / Team / Enterprise） |
| Claude Agent SDK | ✅ 原生 |
| Cursor / Cline / Windsurf | ⚠️ 不直接支持，可把 SKILL.md 内容复制到 system prompt 作为变通 |

---

## 💡 怎么用

### 触发方式 1：自然语言

直接说出关键词，Claude 自动调用：

```
帮我调研 Mammotion 这家公司
做一下 Anker 的欧洲市场背调
下周要拜访 BSH 德国总部，帮我把这家公司摸清楚
准备签 Tennysons 做爱尔兰代理，先做一份尽调
跟踪一下高仙在中东的最新动态
我下周要面试 Pudu Robotics，帮我做一份调研
```

### 触发方式 2：主动调用

```
/company-research
```

### 真实使用场景示例

**场景 A · 客户拜访前调研**

```
👤 我：下周二要去德国 MediaMarkt 总部见他们的园艺品类买手，帮我准备一份调研

🤖 Claude：好的，我会按"五看六定"框架做这份调研。先确认几个问题：
   - 你这次主要想推荐什么产品 / 品类？
   - 想了解 MediaMarkt 园艺品类当前的供应商结构 + 决策链？
   - 调研深度需要到 buyer 个人画像和近期采购信号？

👤 我：推园艺机器人品类 · 重点摸清竞品供应商 + buyer 决策链

🤖 Claude：[启动多轮 WebSearch + WebFetch] ...
         [产出报告 · 重点章节"看竞争 + 看客户决策链 + 3 个拜访开场谈资 + 3 个深挖问题"]
```

**场景 B · 代理商签约前尽调**

```
👤 我：准备签 Numatic 做我们的 UK 经销商，帮我做一份尽调

🤖 Claude：好的，代理商尽调重点是看自身 SWOT 和已代理品牌冲突。
   - 你公司是什么品类？看是否跟 Numatic 现有品牌有利益冲突
   - 想了解他们的渠道覆盖（线下店 / online / B2B）+ 财务健康度？
   - 需要查 Companies House 公开财报数据吗？

👤 我：园艺机器人品类 · 全维度尽调 · 含财报

🤖 Claude：[报告产出 · 重点章节"代理商 SWOT + 已代理品牌清单 + 渠道覆盖地图 + 财务健康 + 3 个签约前必问的关键问题"]
```

**场景 C · 面试求职准备**

```
👤 我：下周三面试 FJ Dynamics 割草机销售岗，帮我做一份调研

🤖 Claude：[报告产出 · 重点章节"五看 + 3 个面试发言洞察 + 3 个反问考察对方的问题"]
```

---

## 📋 报告输出结构

每份报告包含 13 个标准章节：

```
# [公司名] · [产品线] · [目标区域] 市场调研（五看六定）

📌 公司名片（表格速览）

—— 一、五看（市场洞察）——
看一：行业趋势 · 全球 + 区域 + 政策驱动
看二：市场规模 · USD/GBP/EUR + CAGR + 细分
看三：竞争格局 · 至少 5 家竞品对比表
看四：客户需求 · 决策链 + 购买逻辑 + KPI
看五：自身 · SWOT + 公司基本面

—— 二、六定（业务策略）——
定一：目标市场 · P1/P2/P3 优先级
定二：客户画像 · 决策人 + 触达入口
定三：产品策略 · 引流款/主推款/旗舰款
定四：价格策略 · 对标价 + 渠道利润
定五：渠道策略 · 直销/代理/线上/展会
定六：推广策略 · 线上+线下+内容

—— 三、行动弹药 ——
3 个核心洞察（用作客户拜访开场 / 谈判切入 / 决策依据 / 面试发言）
3 个关键问题（用作客户深挖 / 代理商考察 / 决策评审 / 面试反问）
```

参考 [examples/](examples/) 文件夹的真实样例报告。

---

## 📚 方法论：什么是"五看六定"

"五看六定"是雨哥借鉴华为体系内成熟的**市场战略分析框架**，被雨哥改造成更适合海外销售使用的公司背调工具模型。

- **五看**（市场洞察）：看趋势 / 看市场 / 看客户 / 看竞争 / 看自己
- **六定**（业务策略）：4P + 1S + 1C —— 产品 / 价格 / 渠道 / 推广 + 服务 + 客户

**先看再定** —— 没有市场洞察的策略是空中楼阁。

📖 **方法论详细介绍（含「华为原版 vs 雨哥改造版」对比）**:[docs/methodology-five-look-six-set.md](docs/methodology-five-look-six-set.md)

---

## 🏛️ 这个 Skill 在雨哥方法论体系里的位置

本 skill 是 **雨哥海外销售方法论金字塔「第 5 层 · 市场经营」** 的 AI Skill 化产物。

雨哥的完整方法论体系是 **5 层金字塔 + 2 个旁挂元能力** —— 对应海外销售从认知到打单到经营的全路径:

| 层级 | 主题 | 工具弹药 |
|---|---|---|
| 第 1 层 · 认知底座 | 国际业务六重塔 · 海外销售 vs 外贸 · 识局-破局-抗压 | — |
| 第 2 层 · 获客触达 | LinkedIn IP 六步法 · Cold Email 5-7 次序列 · Apollo / Sales Nav | — |
| 第 3 层 · Sell-in 代理商开发 | P0-P9 全流程 · SPIN · MEDDIC · Upfront Contract · EU 86/653 法律风险 | — |
| 第 4 层 · Sell-out 渠道赋能 | 四维赋能 · 代理商话题地图 15 维 · 串货治理 | — |
| **第 5 层 · 市场经营** | **五看六定 · 战略屋 · 4P1S1C · 渠道终局图** | **👈 本 Skill** |
| 旁挂 M1 · 面试作为销售 | 四层面试模型 · STAR 海外版 · 简历五维度美化 | — |
| 旁挂 M2 · 英语 6 文化圈 | 14 场景训练 · 6 文化圈变体 · 150 词术语表 | — |

> 💡 更多雨哥方法论内容,关注 **「雨哥聊海外销售」** 小红书 / 视频号 / 抖音 / LinkedIn。
> 完整作者介绍 → [AUTHOR.md](AUTHOR.md)

---

## 🎓 适用场景

| 场景 | 用法 | 时长 |
|---|---|---|
| **客户拜访前调研** | 摸清客户业务结构 + 决策链 + 当前痛点 + 准备 3 个开场谈资 | 30 分钟 |
| **代理商签约前尽调** | 识别已代理竞品 + 渠道覆盖 + 财务健康度 + 利益冲突 | 30-45 分钟 |
| **竞品季度跟踪** | 定期复盘 5 大竞品的产品 / 价格 / 渠道动态 | 60 分钟 |
| **新市场进入决策** | 评估某区域是否值得投入资源 + 给老板拍板的 BP 输入 | 60-90 分钟 |
| **年度战略 BP 输入** | 作为年度业务规划的市场洞察基线 | 90 分钟 |
| **行业 / 客户类型梳理** | 摸清新行业的客户决策链 + 采购逻辑 | 30 分钟 |
| **海外销售求职面试准备** | 面试前 1-2 天突击调研目标公司 + 行业 + 竞品 | 30 分钟 |

---

## 🛠️ 调研核心原则

1. **中英文双搜** — 中文搜公司背景和融资 / 英文搜海外市场数据和竞品 / 单一语言会漏数据
2. **竞品 ≥ 5 家** — 不能只列 2-3 家就收工 / 5 家是看清结构的最低门槛
3. **区分事实和推测** — 不确定的地方明确标注"推测"或"待确认"
4. **输出可执行** — 报告最后必须给"3 个核心洞察 + 3 个关键问题" / 用户能直接拿去拜访客户、谈代理商、做决策、面试反问
5. **不忽悠** — 数据不够就说数据不够，不编造看似专业但查不到来源的数字
6. **避免沉没成本和路径依赖** — 做"是否进入这个市场 / 是否签这家代理商 / 是否选这家公司"的判断时，先看 hard constraint（资质 / 认证 / 渠道壁垒 / 利益冲突），再谈"匹配度"梯度

---

## 👤 关于作者

**雨哥（雨哥聊海外销售）** —— 海外销售垂直领域 IP · 一人公司创始人

- 13 年海外销售从业经验，完整经历从一线到管理到创业
- 曾任普渡机器人亚太区负责人（年营收破亿，团队 5→50 人）
- 当前主营：海外销售方法论培训 + 求职陪跑 + 试用期陪跑 + 企业海外销售陪跑
- 累计付费客户 130+

📱 **找到雨哥**：

> 🚧 链接占位 —— 请替换以下为真实 URL
- 小红书：[雨哥聊海外销售](https://www.xiaohongshu.com/user/profile/630b68b900000000120007e0)
- 视频号：搜索"雨哥聊海外销售"
- LinkedIn：[Yuge](https://www.linkedin.com/in/shawn2701/)

📧 **业务合作 / 陪跑咨询**：<xxyshawn@gmail.com>

---

## 🤝 贡献

欢迎 issue / PR：

- 报告 bug：[New Issue](../../issues/new)
- 想加新的 skill（比如简历诊断 / 面试复盘的简化版）：[Discussion](../../discussions)
- 反馈使用心得：欢迎在 issues 里贴你产出的报告（脱敏后）

---

## 📜 License

MIT — 自由使用、修改、分发，包括商用。详见 [LICENSE](LICENSE)。

如果这个 skill 帮你拿到了 offer 或者跑通了海外市场，欢迎在小红书 @ 我让我知道 🙌

---

<div align="center">

**English Abstract**

A Claude Skill for systematic overseas market research using the **"Five-Look Six-Set"** framework
(originally a Huawei strategic methodology, adapted here for individual sales / GTM scenarios).

Designed for overseas sales job candidates, GTM leaders entering new markets,
and cross-border BD professionals. Outputs a 13-section standardized report
covering market insights (5 dimensions) + business strategy (6 dimensions)
+ 3 interview takeaways + 3 sharp questions to ask.

Compatible with Claude Code, Claude Desktop, Claude Web, and Claude Agent SDK.

⭐ If this is useful, please consider giving it a star.

</div>
