# chaozhou-pizi-cai-media-buying

一个面向广告投放、买量、ROI、素材、媒体算法和投放团队管理场景的中文 Skill。

这个 Skill 的目标不是输出泛泛而谈的投放常识，而是尽量按照“潮州痞子蔡”这一类实战表达风格，帮助模型把问题拆到本质，再给出有优先级的分析和动作建议。

## 适用场景

- 广告投放分析
- 买量与流量获取
- ROI 异常排查
- 素材迭代与疲劳判断
- 账户结构、预算、出价、放量节奏
- IAA / IAP / ASA / ASO
- 小红书、巨量、广点通、应用商店、Facebook、TikTok、Google、Meta
- 投放团队管理、优化师培养、数据复盘

## 仓库结构

```text
.
├─ SKILL.md
├─ references/
│  ├─ frameworks.md
│  ├─ source-map.md
│  └─ style-guide.md
└─ evals/
   └─ evals.json
```

## 文件说明

- `SKILL.md`：主技能定义，包含触发条件、回答原则、诊断框架、推荐输出结构。
- `references/frameworks.md`：投放分析框架与常见问题拆解。
- `references/source-map.md`：素材来源和内容映射参考。
- `references/style-guide.md`：表达风格说明，帮助输出更贴近目标语气。
- `evals/evals.json`：评测样例。

## 安装方式

如果你在 Codex 或兼容 Skill 目录结构的环境里使用，可以把这个仓库直接放到本地 Skill 目录下，例如：

```text
~/.codex/skills/chaozhou-pizi-cai-media-buying
```

也可以直接克隆：

```bash
git clone https://github.com/sickboy555/-skill.git chaozhou-pizi-cai-media-buying
```

然后确保目录里保留 `SKILL.md`、`references/`、`evals/` 这几个部分即可。

## 使用建议

- 当用户的问题本质是投放、买量、流量、媒体算法、素材、回收、团队管理时，优先启用这个 Skill。
- 回答时不要只给动作，要先判断问题属于哪一层，再给优先排查项和不建议动作。
- 风格上偏直接、清楚、有判断，但不故作夸张。

## 说明

这个仓库当前以 Skill 发布为主，保持了适合直接导入的目录结构，方便后续继续补充 `references` 和 `evals`。
