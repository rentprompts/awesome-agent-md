# Awesome Agents.md
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

An Awesome lists of real‑world **AGENTS.md** formats, templates, guides and tools for agents‑based projects, Already used by over 20k open-source projects. Contributions welcome! at [contributing guidelines](CONTRIBUTING.md).

Resources

## Contents
- [Universal Sample](#universal-sample)
- [Official Samples](#official-samples)
- [Templates](#templates)
- [Guides & Articles](#guides--articles)
- [Tools](#tools)

## Universal Sample

```markdown
## Dev environment tips
- Use `pnpm dlx turbo run where <project_name>` to jump to a package instead of scanning with `ls`.
- Run `pnpm install --filter <project_name>` to add the package to your workspace so Vite, ESLint, and TypeScript can see it.
- Use `pnpm create vite@latest <project_name> -- --template react-ts` to spin up a new React + Vite package with TypeScript checks ready.
- Check the name field inside each package's package.json to confirm the right name—skip the top-level one.

## Testing instructions
- Find the CI plan in the .github/workflows folder.
- Run `pnpm turbo run test --filter <project_name>` to run every check defined for that package.
- From the package root you can just call `pnpm test`. The commit should pass all tests before you merge.
- To focus on one step, add the Vitest pattern: `pnpm vitest run -t "<test name>"`.
- Fix any test or type errors until the whole suite is green.
- After moving files or changing imports, run `pnpm lint --filter <project_name>` to be sure ESLint and TypeScript rules still pass.
- Add or update tests for the code you change, even if nobody asked.

## PR instructions
- Title format: [<project_name>] <Title>
- Always run `pnpm lint` and `pnpm test` before committing.
```

## Official Samples
- [Introducing Codex – OpenAI Blog](https://openai.com/index/introducing-codex/) – First-party explanation of Codex and AGENTS.md usage.
- [OpenAI Codex – Official AGENTS.md](https://github.com/openai/codex/blob/main/AGENTS.md) – Root‑level file showing tests, environment and safety rules.

## Templates
- [Advanced AGENTS.md](List/templates/advanced.md) – A feature‑rich template with testing, safety and style rules.
- [Minimal AGENTS.md](List/templates/minimal.md) – A concise, no‑frills starting point.

## Real‑world Samples
- [Next.js Shop](List/nextjs-shop.md) – Monorepo TypeScript e‑commerce demo with pnpm workspaces.
- [Rust API Skeleton](List/rust-api.md) – Axum‑based REST API showcasing integration tests and nix setup.
- [Microsoft-poml](https://github.com/microsoft/poml/blob/main/AGENTS.md)-Prompt Orchestration Markup Language

## Guides & Articles
- [A Quick Look at ChatGPT Codex – Apidog Blog](https://apidog.com/blog/openai-launches-chatgpt-codex-an-ai-coding-agent) – Visual overview with a five-point minimal template.
- [ChatGPT Codex: The Missing Manual – Latent Space](https://www.latent.space/p/codex) – Detailed format guidance in 'Groom your Agents.md'.
- [Create an AGENTS.md file in your repo – Medium (Joe Njenga)](https://medium.com/@joe.njenga/openai-new-codex-agent-the-fully-agentic-coding-best-coding-agent-8fae9810a888) – Shares a sub-30 line minimal template with examples.
- [OpenAI Codex: A Guide With 3 Practical Examples – DataCamp](https://www.datacamp.com/tutorial/openai-codex) – Step-by-step tutorial including three AGENTS.md samples.
- [The killer feature of OpenAI Codex is parallelism – Medium (Morgan Linton)](https://medium.com/@morganlinton/the-killer-feature-of-openai-codex-is-parallelism-3918886db5cc) – Highlights AGENTS.md as key to Codex success.
- [Writing effective AGENTS.md format](https://agents.md) – Practical tips to accelerate agent onboarding.

## Tools
- [awesome‑lint](https://github.com/sindresorhus/awesome-lint) – Linter that enforces Awesome List style.

## License
This work is released under **CC0‑1.0**. See [LICENSE](LICENSE).
