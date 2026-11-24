# shan-learning-notes

把 GitHub 项目、技术文章或网页链接，整理成简洁、可核验、Obsidian 兼容的中文学习笔记。

这是一个 WorkBuddy 用户级 Skill。目标不是把原文压缩一遍，而是产出一篇「下次忘了也能快速看懂、不确定时能回到原文核对」的笔记。

## 核心做法

- **先判断材料类型。** 导航型（API 清单、资源合集）、工具 / 插件 / 整合包、库 / 框架、文章 / 论文，分别使用不同结构。
- **只保留帮助理解和使用的内容。** 定位、怎么用、关键限制、许可边界。默认删掉目录树、提交历史、功能堆砌、泛泛建议。
- **以原始资料为准。** 核对 README、LICENSE 和正文，区分原文事实、合理推断与待确认内容。
- **许可不混淆。** 仓库自身的许可，不等于所收录资源、模型权重或第三方 API 的许可。
- **Obsidian 友好。** 顶部 YAML 属性、可点击来源链接、协议高亮块。

## 文件结构

| 文件 | 作用 |
|---|---|
| `SKILL.md` | 不可省略的标准、执行流程、最终自检 |
| `references/templates.md` | 四类笔记模板与内容取舍标准 |

## 安装

把本仓库内容放到 WorkBuddy 用户级技能目录：

```text
C:\Users\<用户名>\.workbuddy\skills\shan-learning-notes\
```

保持 `SKILL.md` 与 `references/templates.md` 的相对位置。已安装时，直接更新这两个文件即可。

## 使用

在新对话中直接说：

> 用 shan-learning-notes 分析这个项目并生成笔记：<链接>

或：

> 帮我整理成学习笔记，侧重核心原理和商用许可

普通的「分析项目并写成笔记」「整理学习笔记」「总结这个仓库或文章」也会自动触发该 Skill。

## 笔记格式

每篇笔记以 Obsidian YAML 顶部属性开始：

```yaml
---
title: 项目名 项目学习笔记
date: 2026-11-24
tags:
  - 开源项目
source: https://github.com/作者/项目
---
```

`title`、`date`、`source` 必填；`tags` 可省略，最多两个。正文用 `[项目仓库](URL)` 保证可点击。项目笔记底部使用 Obsidian 高亮块：

```markdown
> [!important] 协议与商用
> 项目采用 [MIT License](许可证链接)，允许商用、修改和分发。
```

## 默认保存位置

`D:\BaiduSyncdisk\SHANAI\SHANAI\x\AI Note Temp`

生成后会复读文件，核对属性、链接、命令、数字和许可。

## 由来

整理标准来自多个真实项目的实践：[public-apis](https://github.com/public-apis/public-apis)、[MinerU-oneClick](https://github.com/artless-artist/MinerU-oneClick)、[dsh-design-studio](https://github.com/OrderG-X/dsh-design-studio)。三者的笔记遵循同一套「最小充分」原则，只是详略不同。
