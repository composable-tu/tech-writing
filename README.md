# Tech Writing Skill

[中文 Readme](./README_zh.md)

A reusable skill that teaches the technical writing methodology proposed in [*How to Write Technical Texts*](https://azat.io/en/blog/how-to-write-technical-texts) by Azat S.

- Source article: https://azat.io/en/blog/how-to-write-technical-texts

## What This Skill Does

This skill captures the **writing methodology** from the article. It provides a structured framework for creating technical texts that are clear, concise, accessible, and practical.

## When to Use

- Writing or polishing technical articles, documentation, tutorials, or blog posts.
- Reviewing and improving an existing technical text.
- Making technical content clearer, more concise, or easier to understand.
- Presenting code examples inside technical texts.

## Quick Start

Use Vercel Skills to install this skill:

```zsh
npx skills add composable-tu/tech-writing
```

Open `SKILL.md` for the full methodology.

Key sections:

1. **General Rules** — narrative style, verbal nouns, passive voice, imperative mood.
2. **Structure** — paragraphs, short sentences, syntax, headings, introductions, conclusions.
3. **Editing Guidelines** — accessibility, concision, brevity, objectivity, clearness, evaluations, visualization.
4. **Code Examples** — naming conventions, imports, simplicity, commands, anti-patterns, relevance.
5. **Editing Workflow** — a repeatable checklist for final review.

## Before and After

Using DeepSeek V4 Flash, we wrote a short doc introducing the history of VoidZero Vite+ (title line removed).

With the Tech Writing Skill:

> Vite Plus is a unified frontend development toolchain. It combines Vite, Vitest, Oxlint, Oxfmt, Rolldown, tsdown, and Vite Task into a single command-line tool that manages runtimes, package managers, and frontend tooling.
>
> After reading this article, you will understand why Vite Plus was created and how to install it locally.
>
> Frontend tooling has become increasingly complex. A typical project requires managing:
>
> - Node.js versions (via nvm or fnm)
> - A package manager (npm, pnpm, or yarn)
> - A build tool (Vite, webpack, etc.)
> - A linter (ESLint)
> - A formatter (Prettier)
> - A test framework (Vitest, Jest, etc.)
> - Type checking (TypeScript)
>
> Each tool has its own configuration file. Upgrading versions, maintaining configs, and resolving compatibility issues consume a lot of development time.
>
> In March 2026, the VoidZero team open-sourced Vite Plus. The project is maintained by industry experts including Evan You (creator of Vue.js) and Long Yinan, and is released under the MIT license. The goal of Vite Plus is simple: replace all the tools above with one tool, so developers can focus on writing code instead of configuring toolchains.
>
> Vite Plus unifies the entire development workflow into a single command-line interface:
>
> - **`vp dev`** — starts the dev server with instant HMR powered by Vite
> - **`vp build`** — builds for production using Rolldown, up to 40× faster than webpack
> - **`vp check`** — runs formatting, linting, and type checking at once
> - **`vp test`** — runs tests powered by Vitest
> - **`vp install`** — installs dependencies using the correct package manager automatically
> - **`vp env`** — manages Node.js versions
>
> You only need to install the single `vp` tool, and your project root only needs one configuration file: `vite.config.ts`.

Without any skill:

> **Vite+** is a unified frontend development toolchain that combines [Vite](https://vite.dev/), [Vitest](https://vitest.dev/), [Oxlint](https://oxc.rs/), [Oxfmt](https://oxc.rs/), [Rolldown](https://rolldown.rs/), [tsdown](https://tsdown.dev/), and [Vite Task](https://github.com/voidzero-dev/vite-task) into a single command-line tool, managing runtimes, package managers, and frontend tooling.
>
> - **March 13, 2026** — The VoidZero team (composed of Evan You, creator of Vue.js, Long Yinan, MK, Wang Chi, Christoph Nakazawa, and others) officially announced the Vite+ Alpha release under the **MIT open-source license**.
> - Vite+ initially considered a paid licensing model, but the team ultimately decided to make it fully open source so more developers could benefit.
> - Its underlying tools are all mature, high-performance Rust tools with large community bases:
>   - Vite — 130 million+ weekly downloads
>   - Vitest — 62 million+ weekly downloads
>   - Oxc / Oxlint — 7 million+ weekly downloads
> - Vite+’s core advantage is **performance**: with Rust-based components, production builds are up to 40× faster than webpack, linting is 50–100× faster than ESLint, and formatting is up to 30× faster than Prettier.

## Repository Structure

```zsh
├── README.md                     # This file
├── README_zh.md                  # Chinese version of this README
├── LICENSE                       # License
├── .gitignore                    # Git ignore rules
└── skills/
    └── tech-writing/
        ├── SKILL.md              # Main skill file with full methodology
        └── knowledge/
            ├── source_article.md # Structured summary of the source article
            ├── methodology.md    # Distilled methodology framework
            ├── checklist.md      # Writing and review checklist
            └── distillation_notes.md # Notes on what was distilled and why
```

## License

- CC BY-NC-SA 4.0
