# 讲题工作台 Skill · Lesson Desk Skill

从试卷和参考答案生成两份配套文件：可编辑的 PowerPoint，以及可导入[讲题工作台](https://github.com/zazedwhwhy/lesson-desk)继续核对、编辑和编排的 `.lesson.zip`。覆盖英语、语文和化学。

[下载 Skill v0.2.0](https://github.com/zazedwhwhy/lesson-desk-skill/raw/main/dist/lesson-desk-export-v0.2.0.zip) · [客户端安装说明](skills/lesson-desk-export/INSTALL.zh-CN.md) · [SHA-256](dist/SHA256SUMS.txt)

## 使用

按客户端说明安装整个 Skill 目录或上传 ZIP。支持 Agent Skills 的宿主需要提供文件访问、终端执行和 Node.js 22 或更高。化学公式的 PNG 预览还需在执行目录安装 `@napi-rs/canvas@1.1.0`。

> 用 `lesson-desk-export` 讲评附件中的试卷，按参考答案核对第 8、12 题，输出 PPT 和可导入讲题工作台的课件包。

解压课件 Skill ZIP 用于安装技能。生成的 `.lesson.zip` 在讲题工作台首页选择「导入课件包」。生成讲义默认保留教师核对状态。

## 构建来源

本仓库包含可直接使用的 Skill、说明、生成器和相应许可证。生成器是可携带的 Node.js 构建产物。其 [TypeScript 源码](https://github.com/zazedwhwhy/lesson-desk/tree/b3bc4f1e05d63a5a8b8c793d38b5261bbdb8c520/skills/lesson-desk-export/tool) 和 [打包脚本](https://github.com/zazedwhwhy/lesson-desk/blob/b3bc4f1e05d63a5a8b8c793d38b5261bbdb8c520/scripts/package-lesson-skill.mjs) 随讲题工作台源码维护。生成器和原 Skill 采用 MIT 许可证，打包的第三方声明在 `skills/lesson-desk-export/licenses/`。
