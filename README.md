# SST-TOUFANG-SKILL

一个面向广告投放、买量、ROI、素材、归因、平台算法、IAA/IAP/混合变现和投放团队管理场景的中文 Skill。

收集互联网有关投放的文章2000篇，压缩成了一套结构化知识库，它现在覆盖的重点内容，主要有这些：

Meta / Facebook / Google / UAC / SAN / SKAN / MMP / AppsFlyer
华为 / vivo / oppo / 小米 / ASA / ASO / 应用商店投放
预算、出价、客群质量、放量节奏
素材系统、素材疲劳、素材复用、双端同素材冲突
IAA / IAP / 混合变现、回收周期、目标拆分
内容平台定位、互动信号、低粉高客单、审核与分发
团队管理、招聘负责人 / 投手、复盘、述职、数据体系
平台算法变化、自动化、AI 化趋势

## 适用场景

- 广告投放分析
- 买量与流量获取
- ROI 异常排查
- 素材迭代与疲劳判断
- 预算、出价、账户结构与放量节奏
- 归因窗口、MMP、AppsFlyer、SAN、SKAN、回传口径
- IAA / IAP / 混合变现
- 小红书、巨量、广点通、应用商店、Facebook、TikTok、Google、Meta
- 投放团队管理、复盘、述职与数据体系建设

## 仓库结构

```text
.
├─ SKILL.md
├─ references/
│  ├─ frameworks.md
│  ├─ problem-playbooks.md
│  ├─ source-map.md
│  └─ style-guide.md
├─ evals/
│  └─ evals.json
├─ agents/
│  └─ openai.yaml
└─ README.md
```

## 文件说明

- `SKILL.md`：主技能定义，包含触发范围、回答原则、默认诊断顺序、输出结构和专题要求。
- `references/frameworks.md`：底层分析框架与核心判断原则。
- `references/problem-playbooks.md`：高频问题作战卡，适合按场景快速拆题。
- `references/source-map.md`：语料来源与主题映射。
- `references/style-guide.md`：回答语气、节奏和表达习惯说明。
- `evals/evals.json`：评测样例。
- `agents/openai.yaml`：显式调用时的 OpenAI agent 元信息。

## 安装方式

如果你在 Codex 或兼容 Skill 目录结构的环境里使用，可以把这个仓库直接放到本地 Skill 目录下，例如：

```text
~/.codex/skills/SST-TOUFANG-SKILL
```

也可以直接克隆：

```bash
git clone https://github.com/sickboy555/-skill.git SST-TOUFANG-SKILL
```

然后确保目录里保留 `SKILL.md`、`references/`、`evals/` 这几个核心部分即可。

## 使用建议

- 当用户的问题本质是投放、买量、流量、素材、归因、回收、平台算法或团队管理时，优先启用这个 Skill。
- 显式唤醒时，优先使用 `$SST-TOUFANG-SKILL`。
- 回答时不要只给动作，先判断问题属于哪一层，再给优先排查项和不建议动作。
- 遇到平台后台、MMP、SAN、SKAN 数据不一致的问题，先对齐统计口径，再讨论优化动作。

## 说明

这个仓库当前以 Skill 发布为主，保持了适合直接导入的目录结构，方便后续继续补充 `references` 和 `evals`。

## 应该如何使用
最好把它当成“投放诊断和决策助手”，不是“泛泛投放百科”。

最好的问法不是：

广告该怎么投？
而是这种：

Meta 预算一加大，CPM 和 CPA 一起涨，这更像是流量池变了还是用户变差了？先看什么？
巨量 IAP 短剧前端 CPA 还行，但首日 ROI 不达标，先别给泛建议，按主因优先级帮我拆。
小红书想让粉丝和成交一起涨，先抓哪几个点？
vivo 应用商店关键词计划首日 ROI 不错，但留存不稳，这更像是哪层没拆开？
我们在招投放负责人，怎么分辨他是吃过红利，还是逻辑真的强？
平时提问时，建议顺手补这几类信息，答案会准很多：

平台：Meta / Google / 巨量 / 小红书 / 华为商店...
业务模型：IAA / IAP / 混合变现 / 短剧 / 工具 / 电商 / 金融...
当前症状：没量 / 有量但贵 / 前端还行但回收差 / 数据打架
时间范围：今天 / 最近3天 / 最近7天 / 放量后
关键指标：CPA / CPM / CTR / CVR / ROI / ROAS / 留存 / 付费率
团队分歧：现在内部有人想提价 / 复制 / 换素材 / 加预算
它默认会按这个思路回答你：

先说结论
再判断问题更像哪一层
再解释为什么
再告诉你先看什么
再告诉你现在最不建议乱做什么
最后给一个处理顺序
一句话理解
这套 skill 最擅长的不是教你“点哪个按钮”，而是先判断你的问题到底属于流量、素材、回收、归因、内容分发、应用商店，还是管理协同，再给你一个有优先级的处理路径。
