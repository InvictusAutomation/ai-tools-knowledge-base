# 🤖 Agent 技术与工具

> 追踪 AI Agent、多 Agent 协作框架和最佳实践

---

## 目录

1. [Agent 框架对比](./frameworks/)
2. [多 Agent 协作](./multi-agent/)
3. [Agent 技能](./skills/)
4. [调研能力](./research-capability/)

---

## Agent 核心能力评估

### 1. 调研能力 (最重要)

| 能力 | 说明 | 评估标准 |
|------|------|----------|
| **实时信息** | 搜索最新信息 | 工具: Perplexity, Kimi, web search |
| **最佳实践** | 代码细节、高质量教程 | 搜索质量 |
| **学术搜索** | 论文、期刊 | arXiv, NeurIPS, ICML |
| **闭源信息** | 产品文档、API | 来源可信度 |

### 2. 自主执行

| 能力 | 说明 |
|------|------|
| **任务规划** | 拆解复杂任务 |
| **代码执行** | 运行、调试 |
| **工具使用** | API、CLI 调用 |
| **学习积累** | Context Hub |

### 3. 多 Agent 协作

| 模式 | 说明 |
|------|------|
| **导演模式** | 一个 Agent 协调多个 |
| **流水线** | 串行处理不同任务 |
| **辩论模式** | Agent 之间的讨论 |
| **角色扮演** | 不同专家协作 |

---

## 当前最佳 Agent 实践

### 调研工作流

```
1. Perplexity / Kimi → 搜索信息
2. 筛选可信来源
3. 深度阅读最佳实践
4. 总结并应用到代码
```

### 多 Agent 协作

```
Leader (capi) → 任务拆解
  ├─→ Researcher (nova) → 信息收集
  ├─→ Coder (bolt) → 代码生成
  ├─→ Analyst (iris) → 数据分析
  └─→ Writer (echo) → 文档撰写
```

---

## Agent 工具对比

| 工具 | 特点 | 适用场景 |
|------|------|----------|
| **OpenClaw** | 多通道集成 | 复杂任务自动化 |
| **Claude Code** | 深度理解 | 复杂代码项目 |
| **Cursor** | AI-first IDE | 日常编程 |
| **Windsurf** | Flow State | 持续开发 |
| **Bolt.new** | 全栈生成 | 快速原型 |
| **Context Hub** | 知识管理 | 学习积累 |
| **InsForge** | 开源后端平台 | 全栈应用开发 |
| **jcode** | Rust 编码 Agent | 高性能项目 |
| **iFlyAgent** | 字节跳动 Agent | 电商/生产场景 |

---

## 2026 年 06 月新出现工具 (GitHub Trending) - 2026-06-29 更新

### 视频与媒体制作

| 工具 | 描述 | 特点 |
|------|------|------|
| **OpenMontage** | 世界首个开源 Agentic 视频制作系统 | 12 pipelines, 52 tools, 500+ skills |
| **voicebox** | 开源 AI 语音工作室 | 克隆、语音合成、创建 |

### 记忆与知识图谱

| 工具 | 描述 | 特点 |
|------|------|------|
| **codebase-memory-mcp** | 高性能代码知识图谱 MCP | 毫秒级索引，158 语言，单一二进制 |
| **cognee** | 开源 AI 记忆平台 | 图基记忆，长期对话一致性 |
| **Agent-Reach** | 互联网视觉 Agent | 读取 Twitter, Reddit, YouTube, Bilibili 等 |

### 框架与规范

| 工具 | 描述 | 来源 |
|------|------|------|
| **DESIGN.md** | 设计规范格式规范 | Google Labs |
| **page-agent** | 页面 GUI Agent | 阿里巴巴 |
| **deer-flow** | 开源长周期 SuperAgent | 字节跳动 |
| **agent-toolkit-for-aws** | AWS MCP 服务器 | AWS 官方 |

### Agent 性能优化

| 工具 | 描述 | 特点 |
|------|------|------|
| **harness** | Agent 性能优化系统 | Skills, instincts, memory, security |
| **headroom** | Token 压缩工具 | 60-95% 更少 token |
| **oh-my-pi** | 终端 AI 编码 Agent | hash-anchored edits |
| **SkillSpector** | Agent 技能安全扫描 | NVIDIA 出品, 检测恶意模式 |

### 记忆与知识

| 工具 | 描述 | 特点 |
|------|------|------|
| **supermemory** | 超快记忆引擎 | Memory API for AI |
| **fff** | 文件搜索工具 | 最快最准的 AI 文件搜索 |
| **codebase-memory-mcp** | 高性能代码知识图谱 | 毫秒级索引，158 语言 |

### 浏览器与自动化

| 工具 | 描述 | 特点 |
|------|------|------|
| **Agent-Reach** | 互联网视觉 Agent | 读取 Twitter, Reddit, YouTube 等 |
| **CloakBrowser** | 反检测 Chromium | 30/30 测试通过 |

### 技能库

| 工具 | 描述 | 来源 |
|------|------|------|
| **last30days-skill** | 30天内研究技能 | Reddit, X, YouTube, HN |
| **taste-skill** | AI 品味提升 | 避免生成无聊内容 |
| **compound-engineering-plugin** | 复合工程插件 | Claude Code / Codex / Cursor |
| **pm-skills** | PM 技能市场 | 100+ agentic skills |

### 视频与语音

| 工具 | 描述 | 特点 |
|------|------|------|
| **Open-LLM-VTuber** | 开源 VTuber | 免手语音交互 + Live2D |
| **MoneyPrinterTurbo** | 短视频生成 | 一键生成高清视频 |
| **OpenMontage** | 开源视频制作系统 | 12 pipelines, 52 tools, 500+ skills |

### Agent 编排

| 工具 | 描述 | 特点 |
|------|------|------|
| **hermes-agent** | 成长型 Agent | NousResearch |
| **revfactory/harness** | 元技能设计 | 定义专业 Agent 团队 |
| **goose** | 可扩展 AI Agent | 支持安装/执行/编辑/测试 |
| **DeepSeek-Reasonix** | DeepSeek 原生终端 Agent | prefix-cache 稳定性 |

### 专业工具

| 工具 | 描述 | 特点 |
|------|------|------|
| **apple/container** | Swift 容器 | Apple 芯片优化 |
| **markitdown** | 文档转换 | Office 转 Markdown |
| **supervision** | 计算机视觉工具 | Roboflow 出品 |

---

## 2026 年 05 月新出现工具

### Agent 编排框架

| 工具 | 描述 | GitHub 星标 |
|------|------|-------------|
| **ruflo** | 多 Agent 编排平台，支持 Claude Code/Codex | 新兴项目 |
| **TradingAgents** | 多 Agent 金融交易框架 | 新兴项目 |
| **local-deep-research** | 本地深度研究 (~95% SimpleQA) | 新兴项目 |
| **hermes-agent** | 可成长的 Agent 框架 | NousResearch |

### 编码 Agent

| 工具 | 描述 | 特点 |
|------|------|------|
| **jcode** | Rust 编码 Agent | 2,710 stars/week |
| **DeepSeek-TUI** | 终端 DeepSeek 客户端 | 终端应用 |
| **InsForge** | 开源后端平台 | 数据库/Auth/存储/计算 |
| **free-claude-code** | 免费 Claude Code 终端 | 开源替代 |

### 技能库 (重点更新)

| 工具 | 描述 | 来源 |
|------|------|------|
| **addyosmani/agent-skills** | 生产级工程技能 | Google Chrome 团队 |
| **mattpocock/skills** | 工程技能集合 | 独立开发者 |
| **ComposioHQ/awesome-codex-skills** | Codex 技能集 | 官方 |
| **zilliztech/claude-context** | 代码搜索 MCP | Milvus |
| **maigret** | 用户名 OSINT 工具 | 3000+ 站点 |

### 浏览器自动化

| 工具 | 描述 | 特点 |
|------|------|------|
| **CloakBrowser** | 反检测 Chromium | 30/30 测试通过 |
| **hyperframes** | HeyGen 视频生成框架 | Agent 专用 |

### 视频/媒体

| 工具 | 描述 | 特点 |
|------|------|------|
| **Pixelle-Video** | AI 全自动短视频引擎 | 全自动化 |
| **Open-Generative-AI** | 开源图像视频生成 | 200+ 模型 |

## 2026 年 05 月新兴工具 (Trending)

| 工具 | 描述 | 特点 |
|------|------|------|
| **codegraph** | Claude Code/Codex/Cursor 预索引代码知识图谱 | 减少 token 和工具调用，100%本地 |
| **CloakBrowser** | 反检测 Chromium (30/30 测试通过) | Playwright 替代品 |
| **agentmemory** | 编码 Agent 持久化内存 | 基于真实世界基准测试 |
| **awesome-codex-skills** | Codex 技能精选列表 | ComposioHQ 出品 |
| **sandcastle** | TypeScript 沙箱编码 Agent 编排 | mattpocock 出品 |
| **ViMax** | Agentic 视频生成 (导演+编剧+制片+生成) | HKUDS 出品 |
| **codex-free-router** | 连接多个免费 AI 提供商 | 40+ 提供商自动 fallback |

---

## 2026 年 07 月新出现工具 (GitHub Trending) - 2026-07-13 更新

### 代码智能与知识图谱

| 工具 | 描述 | 特点 |
|------|------|------|
| **codebase-memory-mcp** | 高性能代码知识图谱 MCP | 毫秒级索引，158 语言，子毫秒查询，99% 更少 token |
| **cognee** | 开源 AI 记忆平台 | 图基记忆，长期对话一致性 |
| **system_prompts_leaks** | 系统提示泄露集合 | Anthropic/OpenAI/Google/xAI 提示定期更新 |
| **zvec** | 轻量级进程内向量数据库 | 阿里开源，闪电般快速 |

### 视频与媒体制作

| 工具 | 描述 | 特点 |
|------|------|------|
| **OpenMontage** | 世界首个开源 Agentic 视频制作系统 | 12 pipelines, 52 tools, 500+ agent skills |
| **Agent-Reach** | 互联网视觉 Agent | 读取 Twitter, Reddit, YouTube, GitHub, Bilibili, 小红书 |

### Agent 编排与复用

| 工具 | 描述 | 特点 |
|------|------|------|
| **herdr** | 终端 Agent 复用器 | 多 Agent 复用，终端交互 |
| **orca** | 多 Agent 桌面 ADE | 并行 Agent 运行，支持订阅 |
| **strix** | 开源渗透测试工具 | AI 驱动的安全测试 |

### 安全与测试

| 工具 | 描述 | 特点 |
|------|------|------|
| **SkillSpector** | Agent 技能安全扫描器 | NVIDIA 出品，检测恶意模式 |
| **strix** | 渗透测试工具 | AI 驱动的漏洞发现与修复 |

### 专业领域工具

| 工具 | 描述 | 特点 |
|------|------|------|
| **hiring-agent** | AI 简历评估 Agent | 自动评估打分简历 |
| **OmniRoute** | 免费 AI 网关 | 231+ 提供商，50+ 免费，Claude/Codex/Cursor/Copilot 集成 |
| **Meetily** | 隐私优先 AI 会议助手 | 4x 转录速度，100% 本地处理 |

### 值得关注

| 工具 | 描述 | 特点 |
|------|------|------|
| **iroh** | QUIC + NAT 穿透库 | n0-computer 出品，IP 地址替代方案 |
| **supermemory** | 超快记忆引擎 | Memory API for AI |
| **dbx** | 轻量级数据库客户端 | 15MB, 跨平台, 8+ 数据库 |

---

## 2026 年 07 月新出现工具 (GitHub Trending) - 2026-07-27 更新

### AI 网关与路由

| 工具 | 描述 | 特点 |
|------|------|------|
| **OmniRoute** | 免费 MIT AI 网关 | 290+ 提供商 (90+ 免费), 500+ 模型, Claude/Codex/Cursor/Copilot 集成, RTK+Caveman 压缩节省 15-95% tokens |

### 安全与渗透测试

| 工具 | 描述 | 特点 |
|------|------|------|
| **strix** | 开源 AI 渗透测试工具 | 自动化发现和修复应用漏洞 |

### Agent 编排

| 工具 | 描述 | 特点 |
|------|------|------|
| **orca** | 多 Agent 桌面 ADE | 并行 Agent 运行, 支持订阅 |
| **herdr** | 终端 Agent 复用器 | 多 Agent 复用, 终端交互 |

### 效率与生产力

| 工具 | 描述 | 特点 |
|------|------|------|
| **OfficeCLI** | Office 套件 CLI 工具 | AI Agent 读写编辑 Word/Excel/PPT, 单二进制无需安装 |
| **Meetily** | 隐私优先 AI 会议助手 | 4x 转录速度, 100% 本地处理 |

### 设计与创意

| 工具 | 描述 | 特点 |
|------|------|------|
| **hallmark** | 反 AI-slop 设计技能 | Claude Code/Cursor/Codex 避免生成无聊内容 |

### 知识与记忆

| 工具 | 描述 | 特点 |
|------|------|------|
| **codebase-memory-mcp** | 高性能代码知识图谱 MCP | 毫秒级索引, 158 语言, 子毫秒查询, 99% 更少 token |

### 系统提示泄露

| 工具 | 描述 | 特点 |
|------|------|------|
| **system_prompts_leaks** | 系统提示泄露集合 | Anthropic/OpenAI/Google/xAI 提示定期更新 |

### 投资研究

| 工具 | 描述 | 特点 |
|------|------|------|
| **ai-berkshire** | AI 价值投资研究框架 | Claude Code/Codex + 巴菲特·芒格·段永平·李录四大师方法论 |

### 视频处理

| 工具 | 描述 | 特点 |
|------|------|------|
| **claude-video** | Claude 视频理解能力 | 下载视频、提取帧、转录、交给 Claude 分析 |
| **OpenCut** | 开源 CapCut 替代品 | 视频剪辑 |

### 页面自动化

| 工具 | 描述 | 特点 |
|------|------|------|
| **page-agent** | 页面 GUI Agent | 阿里巴巴出品, JavaScript 纯前端 GUI Agent |

### SEO

| 工具 | 描述 | 特点 |
|------|------|------|
| **open-seo** | 开源 Semrush/Ahrefs 替代品 | SEO 分析工具 |

---

## 2026 年 07 月新出现工具 (GitHub Trending) - 2026-07-19 更新

### 视频与媒体制作

| 工具 | 描述 | 特点 |
|------|------|------|
| **OpenMontage** | 世界首个开源 Agentic 视频制作系统 | 12 pipelines, 52 tools, 500+ agent skills |
| **ai-job-search** | AI 求职框架 | Claude Code 驱动，评估职位、定制简历、求职信 |

### 代码智能与知识图谱

| 工具 | 描述 | 特点 |
|------|------|------|
| **codebase-memory-mcp** | 高性能代码知识图谱 MCP | 毫秒级索引，158 语言，子毫秒查询，99% 更少 token |
| **codebase-memory-mcp** | 高性能代码索引 | 平均毫秒级索引，单一静态二进制，零依赖 |

### Agent 编排与工具

| 工具 | 描述 | 特点 |
|------|------|------|
| **herdr** | 终端 Agent 复用器 | 多 Agent 复用，终端交互 |
| **orca** | 多 Agent 桌面 ADE | 并行 Agent 运行，支持订阅 |
| **strix** | 开源渗透测试工具 | AI 驱动的漏洞发现与修复 |
| **page-agent** | 页面 GUI Agent | 阿里巴巴出品，纯前端 JavaScript GUI Agent |

### 安全与测试

| 工具 | 描述 | 特点 |
|------|------|------|
| **SkillSpector** | Agent 技能安全扫描器 | NVIDIA 出品，检测恶意模式 |
| **strix** | 渗透测试工具 | AI 驱动的漏洞发现与修复 |

### 专业领域工具

| 工具 | 描述 | 特点 |
|------|------|------|
| **hiring-agent** | AI 简历评估 Agent | 自动评估打分简历 |
| **OmniRoute** | 免费 AI 网关 | 231+ 提供商，50+ 免费，Claude/Codex/Cursor/Copilot 集成 |
| **Meetily** | 隐私优先 AI 会议助手 | 4x 转录速度，100% 本地处理 |
| **Agent-Reach** | 互联网视觉 Agent | 读取 Twitter, Reddit, YouTube, GitHub, Bilibili, 小红书 |

### 效率与优化

| 工具 | 描述 | 特点 |
|------|------|------|
| **OfficeCLI** | Office 套件 CLI 工具 | AI Agent 读写编辑 Word/Excel/PPT，单二进制无需安装 |
| **DesktopCommanderMCP** | Claude 终端控制 MCP | 终端控制、文件系统搜索、diff 编辑 |
| **OpenCut** | 开源 CapCut 替代品 | 视频剪辑 |

### 值得关注

| 工具 | 描述 | 特点 |
|------|------|------|
| **hallmark** | 反 AI-slop 设计技能 | Claude Code/Cursor/Codex 避免生成无聊内容 |
| **iroh** | QUIC + NAT 穿透库 | n0-computer 出品，IP 地址替代方案 |
| **supermemory** | 超快记忆引擎 | Memory API for AI |

---

## 2026 年 08 月新出现工具 (GitHub Trending) - 2026-08-15 更新

### 团队级记忆与知识管理

| 工具 | 描述 | 特点 |
|------|------|------|
| **TencentDB-Agent-Memory** | 腾讯团队级记忆中心 | 12,445 stars，将对话/文档/代码转化为四种可复用记忆资产 (Chat Memory, Skill, LLM-Wiki, Code-Graph)，跨 Agent/框架共享 |

### AI 网关与路由

| 工具 | 描述 | 特点 |
|------|------|------|
| **OmniRoute** | 免费 MIT AI 网关 | 330+ 提供商 (90+ 免费)，1200+ 模型，Kimi/Claude/GPT/Gemini/GLM/DeepSeek/MiniMax，支持 Claude Code/Codex/Cursor/Cline/Copilot，RTK+Caveman 压缩节省 15-95% tokens |

### 逆向工程与安全

| 工具 | 描述 | 特点 |
|------|------|------|
| **reverse-skill** | 逆向/渗透/安全技能路由包 | AI 自动路由 + 按需自举工具链 + 自动进化经验库，支持 Claude Code/Kiro/Cursor/Cline |

### 多 Agent 编排

| 工具 | 描述 | 特点 |
|------|------|------|
| **orca** | 多 Agent 桌面 ADE | 并行 Agent 运行，支持订阅，桌面/移动/VPS 跨平台 |

### 智能辅导

| 工具 | 描述 | 特点 |
|------|------|------|
| **DeepTutor** | 终身个性化辅导 | HKUDS 出品，终身个性化辅导 AI |

### 代码工具

| 工具 | 描述 | 特点 |
|------|------|------|
| **kimi-code** | Moonshot AI 代码 CLI | 下一代 Agent 起点 |
| **pi** | AI agent toolkit | 统一 LLM API，agent loop，TUI，coding agent CLI |
| **t3code** | - | pingdotgg 出品 |

### 知识蒸馏

| 工具 | 描述 | 特点 |
|------|------|------|
| **cangjie-skill** | 内容蒸馏成 Agent Skills | 把书、长视频、播客等高价值内容蒸馏成可执行的 Agent Skills |
| **book-to-skill** | PDF 转 Claude Code skill | 把技术书籍 PDF 转为可 study/reference/使用的 skill |

### 设计与架构

| 工具 | 描述 | 特点 |
|------|------|------|
| **archify** | Agent 架构图技能 | 生成美观可验证的架构/工作流/序列/数据流/生命周期图，自包含 HTML |
| **hallmark** | 反 AI-slop 设计技能 | 避免生成无聊内容 |
| **openwork** | Claude Cowork 开源替代 | different-ai 出品，powered by opencode |

### SEO

| 工具 | 描述 | 特点 |
|------|------|------|
| **open-seo** | 开源 Semrush/Ahrefs 替代 | SEO 分析工具 |

### 代码智能

| 工具 | 描述 | 特点 |
|------|------|------|
| **code-review-graph** | 本地优先代码智能图 | MCP 和 CLI 构建持久化代码地图，AI 只读关键内容，benchmark 上下文缩减 |

### 2026 年 08 月新出现工具 (GitHub Trending) - 2026-08-03 更新

### 代码质量与审查

| 工具 | 描述 | 特点 |
|------|------|------|
| **open-code-review** | 阿里开源代码审查工具 | 确定性 pipeline + LLM Agent，精确行级注释，多语言规则集 (NPE/线程安全/XSS/SQL 注入)，兼容 OpenAI/Anthropic |

### 浏览器自动化

| 工具 | 描述 | 特点 |
|------|------|------|
| **ego-lite** | 最快浏览器自动化工具 | 专为 AI Agent 设计，共享登录状态给 Codex/Claude Code，零成本零配置 |

### AI 网关与路由

| 工具 | 描述 | 特点 |
|------|------|------|
| **OmniRoute** | 免费 MIT AI 网关 | 290+ 提供商 (90+ 免费)，500+ 模型，Kimi/Claude/GPT/Gemini/GLM/DeepSeek/MiniMax，支持 Claude Code/Codex/Cursor/Cline/Copilot，RTK+Caveman 压缩节省 15-95% tokens |
| **aisuite** | 多提供商统一接口 | 简单统一接口访问多个生成式 AI 提供商 |

### 技能与学习

| 工具 | 描述 | 特点 |
|------|------|------|
| **book-to-skill** | PDF 转 Claude Code skill | 把技术书籍 PDF 转为可study/reference/使用的 skill |
| **i-have-adhd** | ADHD-friendly 输出 | 阻止 coding agent  bury the answer，专注关键信息 |

### 设计与 3D

| 工具 | 描述 | 特点 |
|------|------|------|
| **text-to-cad** | CAD/CAE/CAM agent skills 库 | AI 生成 CAD 设计 |

### 开源替代

| 工具 | 描述 | 特点 |
|------|------|------|
| **openwork** | Claude Cowork 开源替代 | different-ai 出品，powered by opencode |

---

## 2026 年 08 月新出现工具 (GitHub Trending) - 2026-08-31 更新

### AI 网关与路由

| 工具 | 描述 | 特点 |
|------|------|------|
| **OmniRoute** | 免费 MIT AI 网关 | 350+ 提供商 (90+ 免费), 1200+ 模型, Kimi/Claude/GPT/Gemini/GLM/DeepSeek/MiniMax, Claude Code/Codex/Cursor/Cline/Copilot 集成, RTK+Caveman 压缩节省 15-95% tokens |

### 记忆与知识管理

| 工具 | 描述 | 特点 |
|------|------|------|
| **ai-memory** | 跨 Agent 长期记忆解决方案 | 支持 Claude Code/Codex/Command Code/Devin/OpenCode/Cursor 等 15+ Agent, 跨供应商交接 |
| **OpenViking** | 火山引擎自进化上下文数据库 | 统一 Agent 记忆/知识 RAG 和技能, 三层加载 (L0/L1/L2) 节省 token |

### 知识蒸馏

| 工具 | 描述 | 特点 |
|------|------|------|
| **book-to-skill** | PDF 转 Claude Code skill | 把技术书籍 PDF 转为可 study/reference/使用的 skill |
| **cangjie-skill** | 内容蒸馏成 Agent Skills | 把书/长视频/播客等高价值内容蒸馏成可执行的 Agent Skills |

### 架构与设计

| 工具 | 描述 | 特点 |
|------|------|------|
| **archify** | Agent 架构图技能 | 生成美观可验证的架构/工作流/序列/数据流/生命周期图, 自包含 HTML |

### 多 Agent 编排

| 工具 | 描述 | 特点 |
|------|------|------|
| **swarm-forge** | 多 Agent 协作工具 | 简单工具协调多个 AI agents, 1,613 stars 本月 |

### 设备端模型

| 工具 | 描述 | 特点 |
|------|------|------|
| **needle** | 14MB 设备端基础模型 | 手机/可穿戴/智能家居/机器人专用, 极致轻量化 |

### 效率工具

| 工具 | 描述 | 特点 |
|------|------|------|
| **i-have-adhd** | ADHD-friendly 输出 | 阻止 coding agent bury the answer, 专注关键信息 |
| **pi** | AI agent toolkit | 统一 LLM API, agent loop, TUI, coding agent CLI |

### Claude 生态

| 工具 | 描述 | 特点 |
|------|------|------|
| **claude-plugins-community** | Claude 插件社区 | Claude Cowork 和 Claude Code 社区插件市场 |

---

## 2026 年 09 月新出现工具 (GitHub Trending) - 2026-09-11 更新

### Cursor 官方插件生态

| 工具 | 描述 | 特点 |
|------|------|------|
| **Thermos** | 热核分支审查 | 深度安全/正确性审计，严厉代码质量标准，并行 subagent |
| **Orchestrate** | 云端并行 Agent 编排 | 将大任务分发到并行云 agent，支持 planner/worker/verifier |
| **Cursor SDK** | TypeScript SDK | 构建应用、脚本和自动化 |
| **Cursor Team Kit** | 内部团队工作流 | CI、代码审查、发布、本地自动化和验证 |
| **Agent Compatibility** | Agent 兼容性扫描 | CLI 扫描 repo 兼容性，审计启动、验证和文档 |
| **PR Review Canvas** | PR 审查画布 | 按重要性分组渲染 PR diff |
| **Docs Canvas** | 文档画布 | 导航式文档渲染 |
| **CLI for Agents** | Agent CLI 设计模式 | 设计可靠 CLI 的模式：flags/help/管道/错误/幂等 |
| **Continual Learning** | 增量式持续学习 | transcript 驱动的高信号要点更新 AGENTS.md |
| **Teaching** | 教学技能 | 技能映射、练习计划和学习复盘 |

### AI 网关与路由

| 工具 | 描述 | 特点 |
|------|------|------|
| **NVIDIA Switchyard** | 模型智能路由 | 自动选择最便宜且能完成任务的模型，支持 NeMo Relay/LiteLLM 插件，Python/Rust 双库 |

### Apple Silicon 优化

| 工具 | 描述 | 特点 |
|------|------|------|
| **MTPLX** | MLX 3x 加速 | Apple Silicon 原生 MTP 推测解码，Qwen3.8-27B 效率提升 3x，无需外部草稿模型 |

### 语音与音频

| 工具 | 描述 | 特点 |
|------|------|------|
| **VoiceStudio** | 开源 ElevenLabs 替代 | 语音克隆、设计、视频配音、听写、转录、646 语言 audiobook 创建，全本地 |

### 设计技能

| 工具 | 描述 | 特点 |
|------|------|------|
| **diagram-design** | 38 种编辑图表 | Claude Code/Codex/Pi 专用，自包含 HTML + SVG，无阴影，无 Mermaid |

### 上下文优化

| 工具 | 描述 | 特点 |
|------|------|------|
| **context-mode** | 上下文窗口优化 | 沙箱化工具输出 (98% 减少)，持久化 session memory，MCP + hooks 跨 17 平台路由 |

### 重点观察：Cursor 插件生态成形

**Cursor 官方插件仓库** (cursor/plugins) 的发布标志着 Cursor 从 IDE 向 Agent 平台演进：

- **Thermos**: 强调"热核"级审查 — 自动化安全审计和代码质量评分，适合高标准代码库
- **Orchestrate**: 解决"大任务分解"问题 — 云端并行 worker + verifier，适合复杂项目
- **SDK**: TypeScript 优先，开放了构建自定义插件的完整工具链
- **趋势**: Claude Code/Codex 的 skill 生态正在被 Cursor 以"插件"形式重新定义

---

## 持续更新

- 最后更新: 2026-09-11
- 更新频率: 每周

---

## 2026 年 08 月新出现工具 (GitHub Trending) - 2026-08-24 更新

### 上下文数据库与记忆

| 工具 | 描述 | 特点 |
|------|------|------|
| **OpenViking** | 火山引擎自进化上下文数据库 | 统一 Agent 记忆、知识 RAG 和技能，三层加载 (L0/L1/L2) 节省 token，LoCoMo 准确率 80-83%，tau2-bench 任务成功率 +6.87pp/+11.87pp |
| **ai-memory** | 跨 Agent 长期记忆解决方案 | 支持 Claude Code/Codex/Command Code/Devin/OpenCode/Cursor 等 15+ Agent，支持跨供应商交接，quit Claude Code 继续 Codex 无需重新解释 |

### Agent 工作区

| 工具 | 描述 | 特点 |
|------|------|------|
| **Apache maka** | 本地优先 AI Agent 工作区 | Apache 孵化项目，将消息/工具调用/权限决策/终止事件记录为仅追加日志 |

### 本地推理与训练

| 工具 | 描述 | 特点 |
|------|------|------|
| **unsloth** | 本地 UI 运行和训练 LLMs 和 diffusion 模型 | 支持 Qwen3.8, Kimi K3, MiniMax-H3, Gemma 4, DeepSeek-V4, FLUX 等，一站式本地部署 |
| **needle** | 14MB 设备端基础模型 | 手机/可穿戴/智能家居/机器人专用，极致轻量化 |

### 视频生成

| 工具 | 描述 | 特点 |
|------|------|------|
| **OpenCut** | 开源 CapCut 替代品 | 视频剪辑，开源社区驱动 |
| **MoneyPrinterTurbo** | AI 短视频生成工具 | 根据主题或关键词一键生成高清短视频 |

### 重点观察：OpenViking 上下文数据库

**OpenViking** 是本周 GitHub Trending 明星项目（火山引擎出品）：

- **核心创新**: 记忆/资源/技能统一为虚拟文件系统 (viking:// 协议)，Agent 像开发者一样用 ls/tree/find 操作上下文
- **三层加载**: L0 摘要 (~100 tokens) → L1 概述 (~2k tokens) → L2 详情 (按需加载)
- **性能提升**: 
  - 用户记忆 (LoCoMo): 准确率从 24-57% 提升至 80-83%，输入 token 减少 34.3-91.0%
  - Agent 经验 (tau2-bench): 任务成功率 +6.87pp (零售) / +11.87pp (航空)
- **趋势**: 上下文工程正在从"黑盒向量存储"走向"可观测文件系统"