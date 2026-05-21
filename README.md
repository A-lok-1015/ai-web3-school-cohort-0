# ai-web3-school-cohort-0
start on May 20th in 2026
# 需求文档：AI × Web3 个人学习计划系统

## 简介

本系统面向希望系统学习 AI × Web3 技术栈的开发者（builder），基于 AI x Web3 School Handbook 大纲，提供结构化的学习路径、进度追踪、每日打卡和社区贡献工作流。目标是让学习者能够高效、持续地推进学习，并将学习成果沉淀为可复用的知识资产。

## 术语表

- **学习者（Learner）**：使用本系统进行学习的开发者
- **Handbook**：AI x Web3 School 的官方学习手册，包含四大模块
- **学习计划（Learning_Plan）**：结构化的学习路径文档，包含模块、主题、时间安排
- **打卡系统（Checkin_System）**：每日学习记录模板和追踪机制
- **学习仓库（Learning_Repo）**：用于存储笔记、代码实验和项目原型的 GitHub 仓库
- **反馈流程（Feedback_Flow）**：向 Handbook 提交改进建议和贡献的工作流程
- **模块（Module）**：Handbook 中的一级分类（AI 基础、Web3 基础、AI×Web3 Bridge、前沿探索）
- **主题（Topic）**：模块下的具体学习单元（如 LLM、RAG、Smart Contract 等）

---

## 需求列表

### 需求 1：个人学习计划

**用户故事：** 作为一名开发者，我希望拥有一份结构化的个人学习计划，以便我能够系统地覆盖 AI × Web3 的核心知识，并清晰追踪自己的学习进度。

#### 验收标准

1. THE Learning_Plan SHALL 覆盖 Handbook 的全部四大模块：AI 基础、Web3 基础、AI×Web3 Bridge、前沿探索
2. THE Learning_Plan SHALL 为每个模块下的每个主题提供预估学习时长（以小时为单位）
3. THE Learning_Plan SHALL 将学习路径划分为阶段（Phase），每个阶段包含若干主题
4. WHEN 学习者完成一个主题，THE Learning_Plan SHALL 提供可勾选的进度标记（checkbox）
5. THE Learning_Plan SHALL 包含每个主题的学习目标描述（1-3 条可验证的目标）
6. THE Learning_Plan SHALL 提供推荐的学习顺序，体现模块间的依赖关系
7. WHERE 学习者有前置知识，THE Learning_Plan SHALL 标注哪些主题可以跳过或加速
8. THE Learning_Plan SHALL 包含总体时间估算（周/月维度）

### 需求 2：GitHub 学习仓库结构

**用户故事：** 作为一名开发者，我希望有一个清晰的 GitHub 仓库目录结构，以便我能够有条理地存储学习笔记、代码实验和项目原型，并方便日后检索。

#### 验收标准

1. THE Learning_Repo SHALL 包含与 Handbook 四大模块对应的顶层目录
2. THE Learning_Repo SHALL 在每个模块目录下包含与主题对应的子目录
3. THE Learning_Repo SHALL 为每个主题目录提供标准化的子结构（notes/、code/、resources/）
4. THE Learning_Repo SHALL 包含根目录级别的 README.md 模板，说明仓库用途和导航方式
5. THE Learning_Repo SHALL 包含 daily-logs/ 目录用于存储每日打卡记录
6. THE Learning_Repo SHALL 包含 projects/ 目录用于存储综合项目原型
7. WHEN 学习者创建新的主题目录，THE Learning_Repo SHALL 提供可复用的目录模板说明
8. THE Learning_Repo SHALL 包含 .gitignore 模板，排除常见的临时文件和敏感信息

### 需求 3：每日打卡模板

**用户故事：** 作为一名开发者，我希望有一个标准化的每日学习打卡模板，以便我能够持续记录学习内容、收获和问题，形成可回顾的学习日志。

#### 验收标准

1. THE Checkin_System SHALL 提供包含日期、学习主题、时长的基础信息区域
2. THE Checkin_System SHALL 包含"今日学习内容"区域，支持结构化记录（要点列表）
3. THE Checkin_System SHALL 包含"核心收获"区域，用于记录最重要的 1-3 个洞察
4. THE Checkin_System SHALL 包含"遇到的问题"区域，记录未解决的疑问和障碍
5. THE Checkin_System SHALL 包含"明日计划"区域，明确下一步学习目标
6. THE Checkin_System SHALL 包含"资源链接"区域，记录参考的文章、文档、代码
7. WHEN 学习者完成打卡，THE Checkin_System SHALL 支持以 YYYY-MM-DD.md 格式命名文件
8. THE Checkin_System SHALL 提供周回顾模板，汇总一周的学习进展和调整计划

### 需求 4：Handbook 反馈流程

**用户故事：** 作为一名开发者，我希望有一个清晰的 Handbook 反馈和贡献流程，以便我能够将学习过程中发现的问题、改进建议和新内容贡献回社区。

#### 验收标准

1. THE Feedback_Flow SHALL 描述发现问题时的记录方式（本地草稿格式）
2. THE Feedback_Flow SHALL 提供 GitHub Issue 提交模板，包含问题类型、位置、描述、建议
3. THE Feedback_Flow SHALL 描述 Fork → Branch → PR 的标准贡献流程步骤
4. THE Feedback_Flow SHALL 定义贡献类型分类：错误修正、内容补充、新主题提案、代码示例
5. WHEN 学习者发现内容错误，THE Feedback_Flow SHALL 提供快速报告的最短路径（Issue 模板）
6. WHEN 学习者希望贡献新内容，THE Feedback_Flow SHALL 提供内容格式规范和 PR 描述模板
7. THE Feedback_Flow SHALL 包含贡献质量检查清单（自检 checklist）
8. IF 贡献被拒绝或需要修改，THE Feedback_Flow SHALL 描述如何响应 reviewer 反馈的步骤
