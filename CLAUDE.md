# CLAUDE.md

## gstack (受限模式)

**重要限制**：只允许使用以下三个核心功能模块，禁止调用其他 gstack 技能。

### 允许使用的技能

#### 1. 技术文档审查
- `/document-release` - 发布后的文档同步更新（更新 README/ARCHITECTURE/CONTRIBUTING 等）
- `/document-generate` - 从零生成缺失的技术文档（遵循 Diataxis 框架：教程/指南/参考/解释）

#### 2. QA 测试
- `/qa <url>` - 系统性 QA 测试：发现问题 → 修复 → 验证（原子化提交）
- `/qa-only <url>` - 仅报告问题的 QA 测试（不修改代码）

#### 3. 工程师级别 Review
- `/review` - 工程师级别的代码审查（Staff Engineer 视角）
  - 自动修复明显问题
  - 标记完整性缺陷
  - 生产环境 bug 检测

#### 4. 自动化规划
- `/autoplan` - 自动运行完整的计划评审流程（CEO + 设计 + 工程审查）
  - 自动生成经过全面评审的实施计划
  - 适合快速启动新功能开发

#### 5. 浏览器工具
- `/browse` - 无头浏览器，用于网页浏览和测试
  - 导航页面、与元素交互、验证状态
  - 截图、测试响应式布局、表单测试

#### 6. 学习与记忆
- `/learn` - 管理跨会话的项目学习积累
  - 查看、搜索、清理和导出学习记录
  - 让 gstack 在代码库上越用越智能

### 禁止使用的技能
以下 gstack 技能**不得使用**：
- /office-hours, /plan-ceo-review, /plan-eng-review, /plan-design-review, /plan-devex-review
- /design-consultation, /design-shotgun, /design-html, /design-review
- /ship, /land-and-deploy, /canary, /benchmark
- /open-gstack-browser, /setup-browser-cookies
- /setup-deploy, /setup-gbrain, /sync-gbrain
- /retro, /investigate, /codex, /cso
- /pair-agent, /careful, /freeze, /guard, /unfreeze, /gstack-upgrade

### 使用规范
1. 严格遵守上述功能限制
2. 如果需要使用其他技能，必须获得用户明确授权
3. 默认使用 headless 工具，不使用浏览器相关技能

## Project Context

This is the agentSearch project. Use gstack skills in RESTRICTED MODE only.
