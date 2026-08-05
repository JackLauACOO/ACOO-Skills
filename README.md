# ACOO 阿酷内容大师 · 技能包

> 5 个 AI 技能，覆盖短视频内容创作全流程。

## 技能清单

|  序号 | 技能                         | 功能                   | 推荐顺序 |
| :-: | -------------------------- | -------------------- | :--: |
|  1  | **ACOO-HotTopicResearch**  | 热点选题策划               | ① 起点 |
|  2  | **ACOO-HeadlineCreator**   | 爆款标题创作               |   ②  |
|  3  | **ACOO-StructureDesigner** | 文案结构设计 + 情绪曲线 + 逻辑推理 |   ③  |
|  4  | **ACOO-ShortVideoScript**  | 口播脚本创作 + 分镜头设计       |   ④  |
|  5  | **ACOO-ScriptChecker**     | 文稿质量检查 + 标记式改稿       | ⑤ 收尾 |

## 创作全链路

```
阿酷热点选题 🔥 → 阿酷标题创作 🎯 → 阿酷结构设计 🏗️ → 阿酷脚本创作 🎬 → 阿酷文稿检查 🔍
```

## 技能格式

每个技能是一个独立文件夹，包含一个 `SKILL.md` 文件：

```
ACOO-HeadlineCreator/
└── SKILL.md       ← YAML frontmatter + Markdown 指令
```

### Frontmatter 字段

```yaml
name: ACOO-HeadlineCreator          # 技能唯一标识
description: ACOO·标题创作。...      # 触发描述
version: "1.0.0"                    # 版本号
author: ACOO 阿酷内容大师            # 作者
category: content-creation          # 分类
tags: [标题创作, 爆款标题, ...]      # 标签
trigger:                            # 触发词（SkillHub 必填）
  - "帮我取标题"
  - "起个标题"
```

## 兼容平台

以下 AI 工具原生支持 SKILL.md 格式，可直接导入：

| 平台                 | 安装方式                                                 |
| ------------------ | ---------------------------------------------------- |
| **WorkBuddy**      | 将技能文件夹放入 `~/.workbuddy/skills/`                      |
| **Easyclaw**       | 将技能文件夹放入技能目录，重启即可                                    |
| **Openclaw**       | 支持 SKILL.md 格式，放入项目 `.openclaw/skills/`              |
| **Codex (OpenAI)** | 将 SKILL.md 内容作为 system prompt 或 agent instruction 使用 |
| **Claude Code**    | 放入 `.claude/instructions/` 目录                        |
| **Cursor**         | 放入 `.cursor/rules/` 目录，或作为 `.cursorrules`            |

## 上传到 WorkBuddy SkillHub

> 让全球用户在 WorkBuddy 技能市场一键安装你的技能。

**准备工作：**

- 微信账号（用于扫码登录）
- 已完成实名认证的 SkillHub 开发者账号

**上传步骤：**

1. 打开浏览器访问 **<https://skillhub.cn/>**
2. 点击右上角「登录」，用微信扫码
3. 如未实名认证，先完成实名认证
4. 进入「个人中心」→ 点击「发布 Skill」
5. 依次上传 5 个技能：
   - 上传 `SKILL.md` 文件（每个技能文件夹内）
   - 填写技能介绍（支持图文，可参考下方简介模板）
   - 选择分类：**内容创作** 或 **content-creation**
   - 提交审核
6. 审核周期：**3-7 个工作日**
7. 审核通过后，技能会出现在 SkillHub 市场，所有 WorkBuddy 用户可搜索安装

**技能简介模板（复制到 SkillHub 介绍栏）：**

> **ACOO-HotTopicResearch 阿酷热点选题**  
> 从你的行业角度捕捉全网热点，策划爆款短视频选题。支持自定义赛道和目标受众，输出 5 个选题建议，含选题理由和趋势判断。

> **ACOO-HeadlineCreator 阿酷标题创作**  
> 根据选题创作 5 个不同风格的爆款标题，覆盖悬念/数字/对比/情感/痛点等风格，支持视频号、抖音等平台适配。

> **ACOO-StructureDesigner 阿酷结构设计**  
> 匹配 7 种爆款结构（黄金三段式/SCQA/PAS/起承转合等），融入 MECE 原则和金字塔原理，输出主观点+分观点+金句+情绪曲线+钩子+结尾。

> **ACOO-ShortVideoScript 阿酷脚本创作**  
> 根据选题和标题创作 60-90 秒口播脚本，含分镜头设计、情绪节奏承接和拍摄建议。完成后自动询问是否审核。

> **ACOO-ScriptChecker 阿酷文稿检查**  
> 检查口播脚本的段落衔接、信息密度和口播流畅度，找出观众划走风险点，支持标记式精准改稿。

### 通用安装方法

1. 下载对应的 zip 文件
2. 解压到你的 AI 工具的 skills/instructions 目录
3. 重启或刷新 AI 工具
4. 在对话中提及技能描述中的关键词即可自动触发

## 使用示例

```
用户：今天有什么热点可以追？
→ 自动触发 ACOO-HotTopicResearch

用户：帮我写个爆款标题
→ 自动触发 ACOO-HeadlineCreator

用户：这段脚本帮我审一下
→ 自动触发 ACOO-ScriptChecker
```

## 版本

- v1.0.0 (2026-08-05)：首次发布，含 5 个技能

## 作者

ACOO 阿酷内容大师 © 2026

---

*如果你使用的 AI 工具不支持 SKILL.md 格式，可以将 SKILL.md 的正文内容直接作为 system prompt 粘贴使用，效果相同。*
