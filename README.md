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

## 专家库完整列表（271位）

> 共 14 个领域，271 位专家，覆盖营销、技术、电商、写作、游戏、学术等场景。

### 营销与内容（14位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| marketing-xiaohongshu-operator | 小红书运营专家 | 种草笔记、达人合作、爆款公式 |
| marketing-paid-ads-manager | 付费广告经理 | Meta/Google广告、ROAS优化 |
| marketing-brand-storyteller | 品牌故事讲述者 | 品牌叙事、情感共鸣、内容策略 |
| marketing-community-manager | 社区运营经理 | 私域运营、用户增长、活跃度 |
| marketing-content-strategist | 内容策略专家 | 内容矩阵、SEO、多平台分发 |
| marketing-conversion-optimizer | 转化率优化师 | 落地页、A/B测试、漏斗分析 |
| marketing-email-marketer | 邮件营销专家 | 自动化序列、细分、打开率 |
| marketing-go-to-market-strategist | 市场进入策略师 | GTM策略、产品发布、定位 |
| marketing-influencer-strategist | 网红营销策略师 | KOL/KOC合作、影响力营销 |
| marketing-market-researcher | 市场调研专家 | 用户洞察、竞品分析、数据 |
| marketing-performance-marketer | 效果营销专家 | 数据驱动、归因分析、ROI |
| marketing-product-marketer | 产品营销经理 | 产品定位、竞争分析、发布 |
| marketing-seo-specialist | SEO专家 | 关键词策略、技术SEO、排名 |
| marketing-social-media-manager | 社交媒体经理 | 多平台运营、内容日历 |

### 付费广告（10位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| paid-ads-amazon-ppc-specialist | 亚马逊PPC专家 | 亚马逊广告、竞价、ACOS |
| paid-ads-creative-strategist | 创意策略师 | 广告素材、测试框架 |
| paid-ads-cross-channel-media-buyer | 跨渠道媒介购买师 | 多平台投放、预算分配 |
| paid-ads-data-analyst | 广告数据分析师 | 数据分析、归因、报告 |
| paid-ads-google-ads-specialist | Google广告专家 | SEM、展示广告、再营销 |
| paid-ads-landing-page-optimizer | 落地页优化师 | CRO、UX、转化测试 |
| paid-ads-meta-ads-specialist | Meta广告专家 | FB/IG广告、受众定向 |
| paid-ads-programmatic-trader | 程序化广告交易师 | DSP、RTB、受众数据 |
| paid-ads-retention-specialist | 留存专家 | 再营销、LTV、流失挽回 |
| paid-ads-tiktok-ads-specialist | TikTok广告专家 | TikTok投放、内容广告 |

### 电商与销售（17位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| ecommerce-amazon-listing-specialist | 亚马逊Listing专家 | 标题优化、A+页面、排名 |
| ecommerce-customer-experience-manager | 客户体验经理 | NPS、客服、体验设计 |
| ecommerce-marketplace-manager | 电商平台运营经理 | 多平台管理、活动策划 |
| ecommerce-merchandising-manager | 商品运营经理 | 选品、陈列、促销策划 |
| ecommerce-mobile-commerce-specialist | 移动电商专家 | App购物、移动端转化 |
| ecommerce-pricing-strategist | 定价策略师 | 动态定价、竞价分析 |
| ecommerce-product-launch-manager | 产品发布经理 | 新品上市、预热、爆发 |
| ecommerce-subscription-specialist | 订阅制专家 | 订阅模式、续费率、LTV |
| sales-account-executive | 销售客户经理 | B2B销售、大客户管理 |
| sales-b2b-strategist | B2B销售策略师 | 企业销售、解决方案销售 |
| sales-business-development-rep | 商务拓展代表 | 线索开发、陌拜、破冰 |
| sales-channel-partner-manager | 渠道合作经理 | 分销体系、合作伙伴 |
| sales-customer-success-manager | 客户成功经理 | 续约、增购、满意度 |
| sales-outbound-specialist | 外呼销售专家 | 电话销售、话术设计 |
| sales-revenue-operations | 营收运营专家 | 销售流程、CRM、预测 |
| sales-solution-engineer | 解决方案工程师 | 技术销售、POC、提案 |
| specialized-pricing-optimizer | 定价优化专家 | 价格模型、弹性分析 |

### 供应链与运营（10位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| supply-chain-inventory-forecaster | 库存预测专家 | 需求预测、安全库存 |
| supply-chain-route-optimizer | 物流路径优化师 | 配送优化、成本控制 |
| supply-chain-vendor-evaluator | 供应商评估专家 | 供应商筛选、谈判 |
| carrier-relationship-management | 承运商关系管理 | 运费谈判、KPI管理 |
| customs-trade-compliance | 海关合规专家 | 进出口报关、HS编码 |
| energy-procurement | 能源采购专家 | 电力/天然气采购 |
| logistics-exception-management | 物流异常管理 | 延误处理、索赔 |
| production-scheduling | 生产排程专家 | 排产计划、产能优化 |
| quality-nonconformance | 质量不合格品处理 | NCR流程、纠正措施 |
| returns-reverse-logistics | 退货逆向物流 | 退换货管理、处置 |

### 工程技术（11位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| architect | 软件架构师 | 系统设计、技术选型 |
| code-architect | 代码架构师 | 代码结构、模块设计 |
| code-reviewer | 代码审查员 | 代码质量、最佳实践 |
| security-reviewer | 安全审查员 | 漏洞扫描、安全加固 |
| build-error-resolver | 构建错误修复师 | CI/CD、依赖问题 |
| backend-architect-with-memory | 后端架构师 | API设计、数据库、微服务 |
| blockchain-security-auditor | 区块链安全审计师 | 智能合约、DeFi安全 |
| blender-addon-engineer | Blender插件工程师 | 3D工具、Python插件 |
| cpp-build-resolver | C++构建解决师 | CMake、编译问题 |
| terminal-integration-specialist | 终端集成专家 | CLI工具、Shell脚本 |
| typescript-reviewer | TypeScript审查员 | TS类型、代码规范 |

### 测试与质量（10位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| tdd-guide | TDD向导 | 测试驱动开发、红绿重构 |
| testing-accessibility-auditor | 无障碍审计师 | A11y测试、WCAG合规 |
| testing-api-tester | API测试工程师 | 接口测试、自动化 |
| testing-embedded-qa-engineer | 嵌入式QA工程师 | 硬件测试、固件验证 |
| testing-evidence-collector | 测试证据收集师 | 测试报告、缺陷追踪 |
| testing-performance-benchmarker | 性能基准测试师 | 压测、性能分析 |
| testing-reality-checker | 现实检验师 | 边界测试、异常场景 |
| testing-test-results-analyzer | 测试结果分析师 | 数据分析、趋势报告 |
| testing-tool-evaluator | 测试工具评估师 | 工具选型、ROI分析 |
| testing-workflow-optimizer | 测试流程优化师 | 流程改进、自动化策略 |

### 写作与内容创作（16位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| article-illustrator | 文章配图师 | AI配图、视觉风格设计 |
| concretizer | 具象化专家 | 抽象概念转化、类比 |
| edit-diff-learner | 写作复盘学习器 | 对比改稿、经验提炼 |
| editor-review | 主编审稿专家 | 全稿审查、AI味道检测 |
| empathy-designer | 共情点设计师 | 读者心理、情感节点 |
| humanizer | 去AI味专家 | 人性化写作、自然表达 |
| memory-loader | 记忆装载器 | 历史经验提取 |
| outline-architect | 大纲架构师 | 文章结构、逻辑框架 |
| pre-publish-review | 发布前评审专家 | 发布检查、红队挑刺 |
| research-expert | 调研资料专家 | 素材调研、案例收集 |
| title-designer | 标题设计师 | 爆款标题、钩子设计 |
| topic-generator | 选题生成器 | 热点选题、灵感发现 |
| topic-research | 选题调研专家 | 选题验证、热度评估 |
| toutiao-reader-test | 头条读者模拟器 | 读者反应模拟、测试 |
| writing-clarifier | 写作需求澄清专家 | 需求挖掘、要素确认 |
| writing-executor | 写作执行专家 | 初稿产出、执笔成文 |

### 支持职能 — HR / 法务 / 财务（11位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| support-recruitment-specialist | 招聘专家 | JD设计、面试、人才寻访 |
| support-legal-compliance-checker | 法律合规检查师 | 合同审查、法规合规 |
| support-finance-tracker | 财务追踪师 | 预算跟踪、财务分析 |
| support-supply-chain-strategist | 供应链策略师 | 端到端供应链规划 |
| support-infrastructure-maintainer | 基础设施维护师 | IT运维、系统稳定性 |
| support-support-responder | 客服响应专家 | 工单处理、客户沟通 |
| support-analytics-reporter | 分析报告专家 | 数据可视化、洞察 |
| support-executive-summary-generator | 高管摘要生成师 | 报告提炼、决策支持 |
| accounts-payable-agent | 应付账款专员 | 发票处理、供应商付款 |
| customer-billing-ops | 客户账单运营 | 计费系统、账单管理 |
| finance-billing-ops | 财务账单运营 | 财务流程、收款管理 |

### 产品与项目管理（5位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| chief-of-staff | 幕僚长 | 战略执行、高层协调 |
| compliance-auditor | 合规审计师 | 法规遵从、审计流程 |
| corporate-training-designer | 企业培训设计师 | 课程设计、学习路径 |
| automation-governance-architect | 自动化治理架构师 | 流程自动化、治理框架 |
| agents-orchestrator | 代理编排师 | 多Agent协调、工作流 |

### 设计与创意（3位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| technical-artist | 技术美术师 | 着色器、渲染管线 |
| type-design-analyzer | 字体设计分析师 | 排版、字体选择 |
| canvas-design | 画布设计师 | 视觉设计、布局 |

### 游戏开发（8位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| unity-architect | Unity架构师 | Unity系统设计、模式 |
| unity-editor-tool-developer | Unity编辑器工具开发者 | 自定义工具、Editor脚本 |
| unity-multiplayer-engineer | Unity多人游戏工程师 | 网络同步、Netcode |
| unity-shader-graph-artist | Unity着色器图艺术家 | 视觉效果、着色器 |
| unreal-multiplayer-architect | Unreal多人架构师 | UE5网络、DS架构 |
| unreal-systems-engineer | Unreal系统工程师 | 游戏系统、C++/蓝图 |
| unreal-technical-artist | Unreal技术美术 | 材质、特效、优化 |
| unreal-world-builder | Unreal世界构建者 | 关卡设计、环境搭建 |

### XR与空间计算（4位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| visionos-spatial-engineer | visionOS空间工程师 | Apple Vision Pro开发 |
| xr-cockpit-interaction-specialist | XR座舱交互专家 | 工业XR、座舱UI |
| xr-immersive-developer | XR沉浸式开发者 | VR/AR应用开发 |
| xr-interface-architect | XR界面架构师 | 空间UI/UX设计 |

### 学术与教育（8位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| academic-anthropologist | 人类学家 | 文化体系、民族志 |
| academic-geographer | 地理学家 | 空间分析、地理信息 |
| academic-historian | 历史学家 | 史料考证、历史分析 |
| academic-narratologist | 叙事学家 | 故事结构、叙事分析 |
| academic-psychologist | 心理学家 | 行为分析、心理评估 |
| academic-study-planner | 学习规划师 | 学习路径、效率方法 |
| study-abroad-advisor | 留学顾问 | 院校申请、签证规划 |
| corporate-training-designer | 企业培训设计师 | 课程开发、教学设计 |

### 专项工具专家（7位）

| Agent 文件名 | 中文名 | 核心能力 |
|------------|--------|---------|
| specialized-risk-assessor | 风险评估专家 | 风险识别、应对策略 |
| specialized-salesforce-architect | Salesforce架构师 | CRM定制、集成开发 |
| specialized-workflow-architect | 工作流架构师 | 流程设计、自动化 |
| deep-research | 深度研究员 | 多源研究、综合分析 |
| market-research | 市场研究员 | 行业报告、竞品分析 |
| personal-data-harvester | 个人数据收集师 | 数据获取、整理分析 |
| zk-steward | 知识管理员 | 知识库构建、信息架构 |

---

## 安装

### 支持平台

| 平台 | 配置文件 | 调用方式 |
|------|---------|---------|
| **Claude Code** | `SKILL.md` | `/expert 需求描述` |
| **OpenClaw** | `openclaw.skill.json` | `/expert 需求描述` |
| **Codex** | `codex.yaml` | `codex run expert "需求描述"` |

---

### Claude Code 安装

```bash
# 方法一：克隆整个仓库
git clone https://github.com/bruceluo123/expert-skill ~/.claude/skills/expert

# 方法二：只复制 SKILL.md
mkdir -p ~/.claude/skills/expert
curl -o ~/.claude/skills/expert/SKILL.md \
  https://raw.githubusercontent.com/bruceluo123/expert-skill/main/SKILL.md
```

安装完成后，在 Claude Code 中输入 `/expert` 即可使用。

---

### OpenClaw 安装

```bash
# 克隆到 OpenClaw skills 目录
git clone https://github.com/bruceluo123/expert-skill ~/.openclaw/skills/expert

# 或者通过 ClawHub（如果已发布）
/install bruceluo123/expert
```

OpenClaw 会自动读取 `openclaw.skill.json`，然后用 `/expert` 调用。

---

### Codex 安装

```bash
# 克隆到 Codex skills 目录
git clone https://github.com/bruceluo123/expert-skill ~/.codex/skills/expert

# 或者在项目内使用
git clone https://github.com/bruceluo123/expert-skill .codex/skills/expert
```

安装后通过以下方式调用：

```bash
codex run expert "我想做小红书爆款内容"
# 或者在 Codex 对话中
/expert 我想做小红书爆款内容
```

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
