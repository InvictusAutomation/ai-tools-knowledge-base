# 🎯 Skill 体系设计与作用域管理深度研究报告
## 跨层级技能组织、任务匹配与动态编排最佳实践

> 本报告深入探讨 AI Agent Skill 体系的作用域管理问题，涵盖用户级、项目级、子目录级三级 Skill 的设计原则、组织策略与动态调用机制，为 Skill 的有效管理与复用提供全面的方法论指导。

---

## 第一部分：Skill 作用域体系概述

### 1.1 三级作用域模型

```
┌──────────────────────────────────────────────────────────────────┐
│                  Skill 三级作用域金字塔                      │
├──────────────────────────────────────────────────────────────────┤
│                                                          │
│               🌟 用户级 (User Level)                         │
│          文件: ~/.claude/CLAUDE.md                           │
│          作用域: 所有项目 (All Projects)                    │
│          用途: 通用能力、超能力、日常工具                    │
│          ┌─────────────────────────────────────────┐        │
│          │         项目级 (Project Level)        │        │
│          │    文件: 项目根目录/CLAUDE.md         │        │
│          │    作用域: 当前项目 (Current Project)  │        │
│          │    用途: 项目规范、特定工作流         │        │
│          │    ┌─────────────────────────────┐   │        │
│          │    │   子目录级 (Module Level)  │   │        │
│          │    │ src/module/CLAUDE.md       │   │        │
│          │    │ 作用域: 特定模块            │   │        │
│          │    │ 用途: 模块规范、能力       │   │        │
│          │    └─────────────────────────────┘   │        │
│          └─────────────────────────────────────────┘        │
│                                                          │
└──────────────────────────────────────────────────────────────────┘
```

### 1.2 各层级职责定义

| 级别 | 文件位置 | 作用域 | 生命周期 | 修改频率 |
|------|---------|--------|----------|----------|
| **用户级** | `~/.claude/CLAUDE.md` | 全局通用 | 永久 | 低 |
| **项目级** | 项目根目录/CLAUDE.md | 当前项目 | 项目周期 | 中 |
| **子目录级** | src/module/CLAUDE.md | 特定模块 | 模块周期 | 高 |

### 1.3 作用域冲突问题

```
┌──────────────────────────────────────────────────────────────────┐
│               常见作用域冲突                          │
├──────────────────────────────────────────────────────────────────┤
│                                                          │
│  冲突1: 重复定义                                             │
│  用户级: 通用代码审查规范                                    │
│  项目级: 重写项目代码审查规范                               │
│  子目录级: 模块特定审查规范                                  │
│                                                          │
│  冲突2: 优先级模糊                                         │
│  任务来了，应该用哪个层级的 Skill？                        │
│                                                          │
│  冲突3: 更新同步                                           │
│  用户级 Skill 更新了，项目级需要同步？                    │
│                                                          │
│  冲突4: 新 Skill 放哪里                                     │
│  新增的 Skill 应该放在哪一级？                             │
│                                                          │
└──────────────────────────────────────────────────────────────────┘
```

---

## 第二部分：层级设计与组织原则

### 2.1 用户级 Skill 设计

#### 2.1.1 什么 Skill 适合放用户级

```
用户级 Skill 判断标准：
✅ 跨项目通用
✅ 长期稳定不变
✅ 核心能力/超能力
✅ 高频使用（>50%项目）
✅ 与业务无关（通用工具）
```

| Skill 类型 | 示例 | 理由 |
|-----------|------|------|
| **编辑工具** | code-review, refactor | 所有项目需要 |
| **搜索工具** | web-search, docs-search | 通用能力 |
| **通用工作流** | git-workflow, test-runner | 项目通用 |
| **格式转换** | markdown-format, json-format | 工具性质 |
| **系统操作** | shell-command, file-ops | 底层能力 |

#### 2.1.2 用户级 Skill 模板

```markdown
# 用户级 Skill - CLAUDE.md

## 核心能力
- 通用问题解决
- 代码审查

## 超能力
- web_search: 网络搜索
- docs_search: 文档搜索
- memory: 记忆管理

## 常用工具
- code_refactor: 代码重构
- test_generate: 测试生成
- git_advanced: 高级 Git 操作

## 项目启动模板
- new_component: 创建新组件
- new_api: 创建新 API

## 注意事项
- 保持简洁
- 避免业务逻辑
- 定期清理
```

### 2.2 项目级 Skill 设计

#### 2.2.1 什么 Skill 适合放项目级

```
项目级 Skill 判断标准：
✅ 项目特定规范
✅ 项目工作流
✅ 团队约定
✅ 中等频率使用
✅ 与项目技术栈相关
```

| Skill 类型 | 示例 | 理由 |
|-----------|------|------|
| **项目规范** | coding-standards, commit-msg | 团队规范 |
| **特定工作流** | deploy-flow, ci-pipeline | 项目流程 |
| **技术栈** | react-patterns, django-cmd | 技术相关 |
| **测试** | test-patterns, mock-data | 测试规范 |
| **文档** | api-docs, readme-gen | 项目文档 |

#### 2.2.2 项目级 Skill 模板

```markdown
# 项目级 Skill - CLAUDE.md

## 项目概览
- 项目名: MyProject
- 技术栈: React + Node.js + PostgreSQL
- 框架: Next.js 14, Prisma

## 代码规范
- 函数式组件优先
- Type Strict
- CSS Modules

## 工作流
- 提交规范: conventional-commits
- 分支: feature/*, bugfix/*, hotfix/*
- 审查: 2 Approve + CI Pass

## 项目命令
- dev: npm run dev
- test: npm run test:coverage
- build: npm run build
- migrate: prisma migrate dev

## 数据库操作
- model: prisma generate
- push: prisma db push
- seed: prisma db seed

## 注意事项
- 遵循 ESLint 配置
- 测试覆盖率 > 80%
```

### 2.3 子目录级 Skill 设计

#### 2.3.1 什么 Skill 适合放子目录级

```
子目录级 Skill 判断标准：
✅ 模块特定需求
✅ 模块独特模式
✅ 高频修改
�� 与��体模块强绑定
```

| 模块 | Skill 类型 | 示例 |
|------|-----------|------|
| **src/api/** | API规范 | rest-patterns, validation |
| **src/components/** | 组件规范 | react-patterns, storybook |
| **src/hooks/** | Hook规范 | hook-patterns |
| **tests/** | 测试规范 | test-fixtures, mocks |
| **scripts/** | 脚本 | build-scripts |

#### 2.3.2 子目录级 Skill 模板

```markdown
# 模块级 Skill - src/components/CLAUDE.md

## 组件规范
- 使用函数组件 + Hooks
- Props 类型定义
- Storybook 文档

## 模式
- Container/Presenter 模式
- Compound Components

## 测试
- React Testing Library
- Jest
- @testing-library/user-event

## 常用命令
- storybook: npm run storybook
- test: npm test -- --coverage
```

---

## 第三部分：Skill 组织决策树

### 3.1 新增 Skill 决策流程

```
┌──────────────────────────────────────────────────────────────────┐
│              新增 Skill 决策流程                            │
├──────────────────────────────────────────────────────────────────┤
│                                                          │
│  开始: 新增某个 Skill                                       │
│    │                                                     │
│    ▼                                                     │
│  Q1: 这个 Skill 跨项目通用吗？                          │
│    │                                                     │
│    ├─ ✅ 是 → 用户级                                     │
│    │                                                     │
│    └─ ❌ 否 → Q2                                       │
│    │                                                     │
│    ▼                                                     │
│  Q2: 只在这个项目使用？                                  │
│    │                                                     │
│    ├─ ✅ 是 → Q3                                       │
│    │                                                     │
│    └─ ❌ 否 → 共享库/包                                 │
│    │                                                     │
│    ▼                                                     │
│  Q3: 只在这个模块使用？                                  │
│    │                                                     │
│    ├─ ✅ 是 → 子目录级                                  │
│    │                                                     │
│    └─ ❌ 否 → 项目级                                    │
│                                                          │
└──────────────────────────────────────────────────────────────────┘
```

### 3.2 Skill 冲突解决策略

#### 3.2.1 同名冲突

```
冲突类型：三层都有同名 Skill

解决方案优先级：
1. 子目录级 > 项目级 > 用户级
2. 明确使用 @scope 来指定
3. 询问用户确认
```

```python
# 显式指定作用域
@user.code_review    # 用户级
@project.code_review  # 项目级
@module.code_review  # 子目录级
```

#### 3.2.2 优先级配置

```yaml
# .claude/config.yaml
skill_priority:
  # 搜索顺序
  search_order: [module, project, user]
  
  # 覆盖规则
  override:
    - type: module
    - type: project
    - type: user
  
  # 默认
  default: user
```

### 3.3 Skill 继承机制

```
┌��─────────────────────────────────────────────────────────────────┐
│               Skill 继承链                                  │
├──────────────────────────────────────────────────────────────────┤
│                                                          │
│                    用户级 Skill                           │
│                   ┌──────────────┐                        │
│                  /      │       \                        │
│                 /       │        \                       │
│          项目A    项目B    项目C                        │
│                                                                       
│  继承关系：                                            │
│  子目录级 ← 项目级 ← 用户级                           │
│                                                          │
│  加载顺序：                                            │
│  1. 加载用户级 (基础)                                 │
│  2. 加载项目级 (覆盖/扩展)                            │
│  3. 加载子目录级 (最终覆盖)                           │
│                                                          │
└──────────────────────────────────────────────────────────────────┘
```

---

## 第四部分：任务与 Skill 匹配

### 4.1 任务分类与 Skill 映射

```
┌──────────────────────────────────────────────────────────────────┐
│              任务 → Skill 匹配表                           │
├─���────────────────────────────────────────────────────────────────┤
│                                                          │
│  任务类型              → 推荐 Skill                       │
│  ──────────────────────────────────────────────────────  │
│                                                          │
│  代码审查      → @user.code-review                        │
│  重构代码     → @user.code-refactor                     │
│  编写测试     → @user.test-generate + @project.test-pattern │
│  新功能开发   → @project.component-patterns             │
│  API 开发    → @project.rest-patterns                   │
│  Bug 修复    → @user.debug + @project.debug-flow      │
│  文档编写    → @user.docs-generate                   │
│  部署       → @project.deploy-flow                   │
│  数据迁移   → @project.migration-patterns            │
│                                                          │
└──────────────────────────────────────────────────────────────────┘
```

### 4.2 自然语言匹配

#### 4.2.1 意图识别

```python
# 自然语言 → Skill 映射
intent_to_skill = {
    # 编码类
    "写/创建/新增" → ["code-generate", "component-new"],
    "修改/更新" → ["code-update", "refactor"],
    "删除" → ["code-delete", "cleanup"],
    "审查" → ["code-review", "audit"],
    "优化" → ["optimize", "performance-tune"],
    
    # 测试类
    "测试" → ["test-generate", "test-run"],
    "debug" → ["debug", "troubleshoot"],
    
    # 文档类
    "文档" → ["docs-generate", "readme-gen"],
    "说明" → ["explain", "docs"],
    
    # 部署类
    "部署" → ["deploy", "ci-cd"],
    "发布" → ["release", "publish"],
}
```

#### 4.2.2 模糊匹配处理

```python
# 模糊匹配流程
def match_skill(task_description: str) -> list[str]:
    """为任务匹配最佳 Skill"""
    
    # 1. 精确匹配
    exact = exact_match(task_description, all_skills)
    if exact:
        return exact
    
    # 2. 关键词匹配
    keywords = extract_keywords(task_description)
    keyword_matches = keyword_match(keywords, all_skills)
    
    # 3. 语义相似度
    semantic = semantic_match(task_description, all_skills)
    
    # 4. 组合多个
    return rank_and_combine(exact, keyword_matches, semantic)
```

### 4.3 Skill 推荐算法

```python
# Skill 推荐
class SkillRecommender:
    def __init__(self, project_skills, user_skills):
        self.project = project_skills
        self.user = user_skills
    
    def recommend(self, task: dict) -> list[dict]:
        """推荐最佳 Skill"""
        
        # 计算分数
        scores = []
        for skill in self.all_skills:
            score = {
                "relevance": self.task_match(task, skill),
                "scope_priority": self.scope_priority(skill),
                "recency": self.last_used(skill),
                "success_rate": self.success_rate(skill)
            }
            scores.append((skill, sum(score.values())))
        
        # 排序返回
        return sorted(scores, key=lambda x: x[1], reverse=True)
```

---

## 第五部分：Skill 链路编排

### 5.1 复��任��与 Skill 链

#### 5.1.1 什么是 Skill 链路

```
Skill 链路 = 多个 Skill 按顺序执行完成复杂任务

示例：开发一个 REST API
┌──────────────────────────────────────────────┐
│           Skill 链路示例                      │
├──────────────────────────────────────────────┤
│                                          │
│  Step 1: @project.api-template             │
│  (生成 API 模板)                          │
│          ↓                               │
│  Step 2: @user.code-generate             │
│  (生成基础 CRUD 代码)                     │
│          ↓                               │
│  Step 3: @user.test-generate            │
│  (生成测试)                            │
│          ↓                               │
│  Step 4: @user.code-review            │
│  (代码审查)                            │
│          ↓                               │
│  Step 5: @project.docs-generate       │
│  (生成文档)                            │
│                                          │
└──────────────────────────────────────────────┘
```

#### 5.1.2 预定义 Skill 链路

```yaml
# skill-chains.yaml
chains:
  new_api:
    name: "创建新 API"
    steps:
      - skill: @project.api-template
      - skill: @user.code-generate
      - skill: @user.test-generate
      - skill: @user.code-review
  
  new_feature:
    name: "新功能开发"
    steps:
      - skill: @user.analyze
      - skill: @project.architect
      - skill: @user.code-generate
      - skill: @user.test-generate
      - skill: @user.code-review
  
  bug_fix:
    name: "Bug 修复"
    steps:
      - skill: @user.debug-analyze
      - skill: @user.fix-code
      - skill: @user.test-generate
      - skill: @user.verify
```

### 5.2 动态 Skill 链路生成

#### 5.2.1 基于任务动态组合

```python
# 动态生成 Skill 链
def generate_skill_chain(task: str) -> list[str]:
    """根据任务动态生成 Skill 链"""
    
    # 1. 分解任务
    steps = decompose_task(task)
    
    # 2. 为每个步骤匹配 Skill
    skill_chain = []
    for step in steps:
        skill = match_best_skill(step)
        skill_chain.append(skill)
    
    # 3. 优化顺序
    return optimize_chain(skill_chain)
```

#### 5.2.2 自适应 Skill 链

```python
# 自适应 Skill 链执行
class AdaptiveSkillChain:
    def __init__(self):
        self.skills = load_all_skills()
    
    async def execute(self, task: str):
        result = None
        chain = []
        
        while not is_complete(task, result):
            # 找下一个 Skill
            skill = self.select_next_skill(task, result)
            chain.append(skill)
            
            # 执行
            result = await skill.execute(task, result)
            
            # 检查是否需要外部 Skill
            if skill.requires_external:
                external = await self.search_and_import(skill.requirement)
                result = await external.execute(result)
        
        return {
            "chain": chain,
            "result": result
        }
```

### 5.3 技能编排最佳实践

#### 5.3.1 编排原则

| 原则 | 说明 |
|------|------|
| **单一职责** | 每个 Skill 只做一件事 |
| **高内聚** | 相关 Skill 放一起 |
| **低耦合** | Skill 之间独立 |
| **可复用** | Skill 可单独使用 |
| **可测试** | 每个 Skill 可单独测试 |

#### 5.3.2 失败处理

```python
# Skill 链错误处理
async def execute_skill_chain(chain: list[Skill]):
    results = []
    
    for skill in chain:
        try:
            result = await skill.execute()
            results.append({"skill": skill.name, "result": result})
            
        except SkillError as e:
            # 回滚
            await rollback(results)
            
            # 搜索替代 Skill
            alternative = await search_alternative(skill, e)
            if alternative:
                result = await alternative.execute()
                results.append({"skill": alternative.name, "result": result})
            else:
                raise ChainError(f"Skill {skill.name} failed: {e}")
    
    return results
```

---

## 第六部分：外部 Skill 发现与集成

### 6.1 缺 Skill 怎么办

```
┌──────────────────────────────────────────────────────────────────┐
│              缺 Skill 时的决策树                           │
├──────────────────────────────────────────────────────────────────┤
│                                                          │
│  开始: 需要执行某个任务，但没有对应 Skill                     │
│    │                                                     │
│    ▼                                                     │
│  Q1: 现有 Skill 能组合吗？                              │
│    │                                                     │
│    ├─ ✅ 是 → 组合现有 Skill                             │
│    │                                                     │
│    └─ ❌ 否 → Q2                                       │
│    │                                                     │
│    ▼                                                     │
│  Q3: 网上能找到 Skill 吗？                             │
│    │                                                     │
│    ├─ ✅ 是 → 搜索并导入                               │
│    │                                                     │
│    └─ ❌ 否 → Q4                                       │
│    │                                                     │
│    ▼                                                     │
│  Q4: 能创建新 Skill 吗？                                │
│    │                                                     │
│    ├─ ✅ 是 → 创建并使用                               │
│    │                                                     │
│    └─ ❌ 否 → 人工处理                                 │
│                                                          │
└──────────────────────────────────────────────────────────────────┘
```

### 6.2 网上搜索 Skill

#### 6.2.1 搜索来源

```python
# 外部 Skill 来源
skill_sources = {
    # 官方市场
    "claude.ai/marketplace": "官方 Skill 市场",
    "clawhub.com": "ClawHub Skill 市场",
    
    # GitHub
    "github.com/topics/claude-skill": "GitHub Skill 主题",
    "github.com/topics/claude-code": "Claude Code 项目",
    
    # 社区
    "reddit.com/r/Claude_AI_Community": "Reddit 社区",
    "discord.com/invite/claude": "Discord 社区",
}
```

#### 6.2.2 搜索技巧

```python
# Skill 搜索
search_queries = [
    # 精确搜索
    "claude code skill for code review",
    "claude skill for api development",
    "claude skill for testing",
    
    # 模式搜索
    "CLAUDE.md for {}",
    "skill for {} claude",
    "claude code {} workflow",
]
```

### 6.3 Skill 导入与管理

#### 6.3.1 导入流程

```python
# Skill 导入
class SkillImporter:
    def __init__(self):
        self.known_sources = load_sources()
    
    async def import_skill(self, url: str) -> Skill:
        """从 URL 导入 Skill"""
        
        # 1. 下载
        content = await download(url)
        
        # 2. 解析
        skill = parse_skill(content)
        
        # 3. 验证
        await validate(skill)
        
        # 4. 本地化
        localize(skill)
        
        # 5. 注册
        register(skill)
        
        return skill
```

#### 6.3.2 Skill 版本管理

```yaml
# skill-registry.yaml
skills:
  code-review:
    version: 2.1.0
    source: github.com/user/repo
    last_update: 2025-04-01
    status: active
    
  api-generator:
    version: 1.5.0
    source: github.com/another/repo
    last_update: 2025-03-15
    status: needs_update
```

---

## 第七部分：Skill 维护与演化

### 7.1 Skill 生命周期

```
┌──────────────────────────────────────────────────────────────────┐
│                Skill 生命周期                              │
├──────────────────────────────────────────────────────────────────┤
│                                                          │
│  创建 → 测试 → 使用 → 优化 → 归档                       │
│    │      │       │       │       │                        │
│    ▼      ▼       ▼       ▼       ▼                     │
│  设计  验证 日常使用 迭代更新 废弃/替代               │
│                                                          │
│  维护指标：                                            │
│  - 使用频率: 高频使用 → 维护，低频 → 归档              │
│  - 错误率: 低错误率 → 保持，高错误率 → 修复          │
│  - 需求变化: 新需求 → 迭代                            │
│                                                          │
└──────────────────────────────────────────────────────────────────┘
```

### 7.2 Skill 审计

```python
# Skill 审计
class SkillAuditor:
    def audit_all(self):
        results = []
        
        for skill in self.all_skills:
            result = {
                "name": skill.name,
                "usage": self.get_usage(skill),
                "success_rate": self.get_success_rate(skill),
                "last_used": self.last_used(skill),
                "recommendations": self.get_recommendations(skill),
            }
            results.append(result)
        
        # 生成报告
        return self.generate_report(results)
```

### 7.3 Skill 清理

```python
# 清理建议
cleanup_suggestions = {
    # 要删除的
    "never_used": "从未使用的 Skill → 考虑删除",
    "outdated": "超过 6 个月未更新 → 更新或归档",
    "superseded": "已有新版本 → 迁移到新版本",
    
    # 要合并的
    "similar": "多个相似 Skill → 合并为一个",
    
    # 要移动的
    "wrong_level": "作用域不对 → 移动到正确层级"
}
```

---

## 附录

### A. Skill 模板库

```markdown
# Skill 模板

## 基本结构
# name: 技能名称
# description: 描述
# triggers: 触发条件
# actions: 执行动作
# context: 上下文要求
```

### B. 检查清单

| 检查项 | 用户级 | 项目级 | 子目录级 |
|--------|--------|--------|----------|
| 通用性 | ✅ | ❌ | ❌ |
| 稳定不变 | ✅ | ⚠️ | ❌ |
| 高频使用 | ✅ | ⚠️ | ⚠️ |
| 业务无关 | ✅ | ❌ | ❌ |

---

> 报告生成时间: 2025-04-01
> 作者: AI Tools Knowledge Base
> 许可: MIT