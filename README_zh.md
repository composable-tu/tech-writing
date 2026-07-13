# Tech Writing Skill

一个可复用的 Skill，教授 Azat S. 在[《How to Write Technical Texts》](https://azat.io/en/blog/how-to-write-technical-texts)中提出的技术写作方法论。

- 原文链接：https://azat.io/en/blog/how-to-write-technical-texts

## 这个 Skill 做什么

本 Skill 提炼的是文章提出的**写作方法论**。它提供了一套结构化的框架，用于创建清晰、简洁、易懂且实用的技术文本。

## 何时使用

- 撰写或润色技术文章、文档、教程或博客。
- 审查并改进现有的技术文本。
- 让技术内容更清晰、更简洁或更易懂。
- 在技术文本中展示代码示例。

## 快速开始

使用 Vercel Skills 安装该 Skill：

```zsh
npx skills add composable-tu/tech-writing
```

打开 `SKILL.md` 查看完整方法论。

主要章节：

1. **通用规则** — 叙述风格、动名词、被动语态、祈使语气。
2. **文本结构** — 段落、短句、句法、标题列表、引言、结论。
3. **编辑准则** — 可及性、简洁、简短、客观、清晰、避免主观评价、可视化。
4. **代码示例** — 命名规范、导入、简洁性、命令输出、反模式、时效性。
5. **编辑流程** — 最终审查的可复用清单。

## 效果对比

使用 DeepSeek V4 Flash，撰写介绍 VoidZero Vite+ 历史的简短文档（已去除标题行）。

使用 Tech Writing Skill 后撰写的文档：

> Vite Plus 是一个统一的前端开发工具链。它将 Vite、Vitest、Oxlint、Oxfmt、Rolldown、tsdown 和 Vite Task 整合到一个命令行工具中，帮你管理运行时、包管理器和前端工具链。
>
> 读完本文后，你将了解 Vite Plus 的诞生背景，并学会在本地安装它。
>
> 前端开发工具链越来越复杂。一个项目通常需要同时管理：
>
> - Node.js 版本（借助 nvm 或 fnm）
> - 包管理器（npm、pnpm、yarn 中选择其一）
> - 构建工具（Vite、webpack 等）
> - 代码检查工具（ESLint）
> - 代码格式化工具（Prettier）
> - 测试框架（Vitest、Jest 等）
> - 类型检查（TypeScript）
>
> 每个工具都有自己的配置文件。版本升级、配置维护、工具之间的兼容性问题，消耗了大量开发时间。
>
> 2026 年 3 月，VoidZero 团队正式开源了 Vite Plus。项目由 Evan You（Vue.js 作者）、Long Yinan 等业界专家共同维护，基于 MIT 许可证发布。Vite Plus 的目标很简单：用一个工具替代上述所有工具，让开发者专注于编写代码，而不是配置工具链。
>
> Vite Plus 将整个开发流程所需的工具统一到一个命令行界面：
>
> - **`vp dev`** — 启动开发服务器，基于 Vite 提供即时 HMR
> - **`vp build`** — 使用 Rolldown 构建生产版本，比 webpack 快 40 倍
> - **`vp check`** — 同时运行格式检查、代码检查、类型检查
> - **`vp test`** — 运行测试，基于 Vitest
> - **`vp install`** — 自动使用正确的包管理器安装依赖
> - **`vp env`** — 管理 Node.js 版本
>
> 你只需要安装 `vp` 这一个工具，项目根目录下只需一个 `vite.config.ts` 配置文件。

不使用任何 Skill 撰写的文档：

> **Vite+** 是一个统一的前端开发工具链，它将 [Vite](https://vite.dev/)、[Vitest](https://vitest.dev/)、[Oxlint](https://oxc.rs/)、[Oxfmt](https://oxc.rs/)、[Rolldown](https://rolldown.rs/)、[tsdown](https://tsdown.dev/) 和 [Vite Task](https://github.com/voidzero-dev/vite-task) 整合到单一命令行工具中，管理运行时、包管理器和前端工具链。
>
> - **2026 年 3 月 13 日** — VoidZero 团队（由 Vue.js 作者尤雨溪 Evan You、Long Yinan、MK、Wang Chi、Christoph Nakazawa 等人组成）正式宣布 Vite+ Alpha 版本，并以 **MIT 开源许可证**发布。
> - Vite+ 最初曾考虑采用付费许可模式，但团队最终决定完全开源，以使更多开发者受益。
> - 其底层工具均为业界成熟的 Rust 高性能工具，拥有庞大的社区基础：
>   - Vite — 周下载量 1.3 亿+
>   - Vitest — 周下载量 6200 万+
>   - Oxc / Oxlint — 周下载量 700 万+
> - Vite+ 的核心优势在于**性能**：通过 Rust 编写的底层组件，生产构建速度比 webpack 快最高 40 倍，Lint 速度比 ESLint 快 50~100 倍，格式化速度比 Prettier 快最高 30 倍。

## 仓库结构

```zsh
├── README.md                     # 英文版说明
├── README_zh.md                  # 中文版说明（本文件）
├── LICENSE                       # 许可证
├── .gitignore                    # Git 忽略规则
└── skills/
    └── tech-writing/
        ├── SKILL.md              # 包含完整方法论的主 Skill 文件
        └── knowledge/
            ├── source_article.md # 原文结构化摘要
            ├── methodology.md    # 提炼后的方法论框架
            ├── checklist.md      # 写作与审校检查清单
            └── distillation_notes.md # 蒸馏说明与取舍记录
```

## 许可证

- CC BY-NC-SA 4.0
