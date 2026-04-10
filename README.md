# 🎯 /expert — 智能专家匹配 Skill

> 一句话描述需求，自动从 271 位专家中找到最合适的那个，然后开始深度协作。

[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blue?logo=anthropic)](https://claude.ai/code)
[![Agents](https://img.shields.io/badge/专家库-271位-orange)](https://github.com/bruceluo123/expert-skill)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Language](https://img.shields.io/badge/语言-中文-red)](README.md)

---

## 是什么

`/expert` 是一个 Claude Code Skill，充当你和 271 位 AI 专家之间的**智能调度台**。

你不需要记住每个专家的名字，只需要描述你的需求——系统会自动匹配最合适的专家，问你几个关键问题细化需求，然后以专家身份开始深度工作。

```
你：/expert 我的小红书账号涨粉很慢，想做爆款内容

Claude：🎯 为你匹配到以下专家：

【最佳匹配】
小红书运营专家（marketing-xiaohongshu-operator）
→ 深耕小红书平台，精通种草笔记公式、达人合作策略、算法逻辑

📋 接下来请告诉我：
1. 你的账号定位是什么？（美妆/母婴/数码/生活方式？）
2. 目前发了多少篇内容，互动数据大概怎样？
3. 是个人账号还是品牌账号？
```

---

## 专家库覆盖范围（271位）

| 领域 | 专家数 | 代表专家 |
|------|--------|---------|
| 营销与内容 | 14 | 小红书运营、SEO、邮件营销、内容策略 |
| 付费广告 | 10 | Meta广告、Google广告、TikTok广告、亚马逊PPC |
| 电商与销售 | 17 | 亚马逊Listing、定价策略、B2B销售、客户成功 |
| 供应链与运营 | 10 | 库存预测、物流优化、海关合规、供应商评估 |
| 工程技术 | 11 | 软件架构师、安全审查、代码审查、区块链审计 |
| 测试与质量 | 10 | TDD向导、性能测试、无障碍审计、API测试 |
| 写作与内容创作 | 16 | 爆款标题设计、去AI味、主编审稿、选题生成 |
| HR / 法务 / 财务 | 11 | 招聘专家、法律合规、财务分析、客服响应 |
| 游戏开发 | 8 | Unity架构师、Unreal引擎、着色器、多人游戏 |
| XR与空间计算 | 4 | visionOS、VR/AR开发、空间UI |
| 学术与教育 | 8 | 人类学家、历史学家、学习规划、留学顾问 |
| 专项工具 | 8 | 定价优化、风险评估、Salesforce架构、深度研究 |
| 设计与创意 | 3 | 技术美术、字体设计、画布设计 |
| 产品与项目 | 5 | 幕僚长、合规审计、自动化架构 |

---

## 安装

### 前提条件
- [Claude Code](https://claude.ai/code) CLI 已安装

### 方法一：手动安装

```bash
# 克隆到 Claude skills 目录
git clone https://github.com/bruceluo123/expert-skill ~/.claude/skills/expert
```

### 方法二：直接复制 SKILL.md

```bash
mkdir -p ~/.claude/skills/expert
curl -o ~/.claude/skills/expert/SKILL.md \
  https://raw.githubusercontent.com/bruceluo123/expert-skill/main/SKILL.md
```

安装完成后，在 Claude Code 中输入 `/expert` 即可使用。

---

## 使用示例

### 营销场景
```
/expert 我想在小红书上推广我的护肤品牌
/expert 我的 Facebook 广告 ROAS 只有 1.2，怎么优化
/expert 帮我做一个内容营销计划
```

### 技术场景
```
/expert 我需要设计一个高并发的微服务架构
/expert 帮我做代码安全审查
/expert 我的 CI/CD 构建失败了
```

### 电商场景
```
/expert 我在亚马逊开店，Listing 排名很低
/expert 帮我做竞品定价分析
/expert 我的订阅产品续费率很低
```

### 内容创作
```
/expert 帮我写一篇爆款文章，但不要有 AI 味道
/expert 给我设计 10 个吸引人的标题
/expert 帮我审稿，看看哪里可以改进
```

---

## 工作原理

```
用户输入需求
     ↓
解析关键词（平台/任务类型/业务场景）
     ↓
从271位专家中匹配1-3位最合适的
     ↓
展示匹配结果 + 推荐理由
     ↓
提出3个关键问题细化需求
     ↓
用户确认后，切换到专家身份深度工作
```

### 匹配逻辑优先级

1. **平台关键词**：小红书 → 小红书运营专家；亚马逊 → PPC/Listing专家
2. **任务类型**：写作/内容 → 写作系列；代码/开发 → 工程技术系列
3. **业务场景**：电商 → 电商系列；B2B → 销售系列
4. **职能领域**：HR → 招聘专家；财务 → 财务专家
5. **模糊需求**：推荐「深度研究员」先帮你厘清方向

---

## 配套资源

这个 skill 基于 [agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh) 的 208 个中文商业 Agent，结合 Claude Code 内置专家，共 271 位。

如果你想单独使用某位专家，也可以直接在 Claude Code 对话中 `@` 对应的 agent：

```
# 直接调用小红书运营专家
使用 marketing-xiaohongshu-operator agent 帮我...
```

---

## 贡献

欢迎提 PR 添加新的专家匹配规则，或者改进匹配算法。

---

## License

MIT © bruceluo123
