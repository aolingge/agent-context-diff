<p align="center">
  <img src="assets/readme-banner.svg" alt="Agent Context Diff banner" width="100%">
</p>

<h1 align="center">Agent Context Diff</h1>

<p align="center">检查上下文包差异说明是否包含新增、删除、风险、验证和影响范围。</p>

<p align="center"><a href="README.md">English</a> · <a href="#quick-start">快速开始</a> · <a href="#checks">检查项</a> · <a href="#ci-usage">CI</a></p>

<p align="center">
  <img alt="Node.js" src="https://img.shields.io/badge/node-%3E%3D18-2563EB">
  <img alt="dependencies" src="https://img.shields.io/badge/dependencies-0-111827">
  <img alt="license" src="https://img.shields.io/badge/license-MIT-16A34A">
</p>

<p align="center">
  <img src="assets/cli-preview.svg" alt="Agent Context Diff CLI preview" width="88%">
</p>

## 为什么做这个

AI Agent 工具越来越多，但很多仓库缺少能在本地和 CI 里重复执行的小检查。这个工具保持零依赖、可镜像、可复制，适合学生、独立开发者和开源维护者使用。

## Quick Start

```bash
npx github:aolingge/agent-context-diff --path context-diff.md
```

```bash
npx github:aolingge/agent-context-diff --path context-diff.md --markdown > report.md
npx github:aolingge/agent-context-diff --path context-diff.md --sarif > results.sarif
npx github:aolingge/agent-context-diff --path context-diff.md --annotations
```

## Checks

| Check | What it looks for |
| --- | --- |
| added | Lists added context. |
| removed | Lists removed context. |
| risk | Mentions risk or impact. |
| verify | Mentions verification. |

## CI Usage

See [docs/github-actions.md](docs/github-actions.md) and [docs/quality-gates.md](docs/quality-gates.md).

## Mirrors

- GitHub: https://github.com/aolingge/agent-context-diff
- Gitee: https://gitee.com/aolingge/agent-context-diff

## Contributing

Good first PRs: add checks, add fixtures, improve docs, or add GitHub Actions examples.

## License

MIT
