# 讲题工作台 Skill · Lesson Desk Skill

在 Hermes Agent 或其他支持 Agent Skills 的客户端整理英语、语文和化学试卷，生成讲义、可编辑的 PowerPoint 和可导入[讲题工作台](https://github.com/zazedwhwhy/lesson-desk)的课件包。只做扫描识别、整理、校对或修正时，可以单独交付课件包。

[下载 Skill v0.4.0](https://github.com/zazedwhwhy/lesson-desk-skill/releases/download/v0.4.0/lesson-desk-export-v0.4.0.zip) · [客户端安装说明](skills/lesson-desk-export/INSTALL.zh-CN.md) · [三科功能清单](skills/lesson-desk-export/references/workflows.md) · [SHA-256](dist/SHA256SUMS.txt)

## 在 Hermes Agent 中使用

解压 ZIP，把整个 `lesson-desk-export` 放进当前 Hermes 配置的 `skills/`。输入 `/reload-skills` 后用 `/lesson-desk-export`。Hermes 需要已连接的模型、材料和输出路径的访问权限，以及 Node.js 22 或更高版本。化学公式的 PNG 预览还需在执行目录准备 `@napi-rs/canvas@1.1.0`。

> /lesson-desk-export 给这篇英语阅读做词汇手账、句法拆解和第 21–24 题的选项对证，交付 PPT 和讲题工作台课件包。

从讲题工作台首页选择「导入课件包」，打开生成的 `.lesson.zip`。导入和修订无需配置工作台 API。普通生成保留教师核对状态。

## 构建来源

本仓库包含可直接使用的 Skill、生成器和许可证。[TypeScript 源码](https://github.com/zazedwhwhy/lesson-desk/tree/5b75866893f458c87d3762338a841ec860e9fdc9/skills/lesson-desk-export/tool)与[打包脚本](https://github.com/zazedwhwhy/lesson-desk/blob/5b75866893f458c87d3762338a841ec860e9fdc9/scripts/package-lesson-skill.mjs)随讲题工作台维护。Skill 采用 MIT 许可证，随包第三方声明位于 `skills/lesson-desk-export/licenses/`。
