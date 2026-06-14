# Awesome EigenScript

> A curated list of [EigenScript](https://github.com/InauguralSystems/EigenScript)
> packages, tools, examples, and learning resources.

This is a **list, not a registry**. EigenScript's package tool
(`eigenscript --pkg add`) pins consumers to a git URL + tag — there
is no install-time lookup against this index. Listing here is purely
for discoverability.

## Contents

- [Packages](#packages)
  - [Getting Started](#getting-started)
- [Tools](#tools)
- [Learning](#learning)
- [Editor Integrations](#editor-integrations)
- [Showcase](#showcase)

## Packages

Packages are git repos consumable via
`eigenscript --pkg add <owner>/<name> <git-url> <tag>`. The tool
requires the `<owner>/<name>` form — bare names are reserved. See
[CONTRIBUTING.md](#contributing) for naming and versioning
guidance.

### Getting Started

- **[eigs-package-template](https://github.com/InauguralSystems/eigs-package-template)** —
  Forkable starting point for a new package. Layout, smoke test, CI
  workflow, and MIT license already wired up.

<!--
  Add categories as the ecosystem grows. Suggested first headings,
  uncomment as packages exist:

  ### Math & Numerics
  ### Text & Parsing
  ### I/O & Networking
  ### Data Structures
  ### Testing & Diagnostics
-->

## Tools

Build tools, formatters, linters, CI helpers — anything that wraps
the `eigenscript` binary.

- **[eigenscript](https://github.com/InauguralSystems/EigenScript)** —
  The language itself. `eigenscript --fmt`, `eigenscript --lint`,
  `eigenscript --pkg`, `eigenscript --lsp` are the built-in tools.
- **[homebrew-eigenscript](https://github.com/InauguralSystems/homebrew-eigenscript)** —
  Homebrew tap. `brew install InauguralSystems/eigenscript/eigenscript`.

## Learning

- **[docs/SPEC.md](https://github.com/InauguralSystems/EigenScript/blob/main/docs/SPEC.md)** —
  Language reference. Examples are runnable.
- **[docs/STDLIB.md](https://github.com/InauguralSystems/EigenScript/blob/main/docs/STDLIB.md)** —
  Standard library reference.
- **[docs/COMPARISON.md](https://github.com/InauguralSystems/EigenScript/blob/main/docs/COMPARISON.md)** —
  Side-by-side with Python and JavaScript.
- **[examples/](https://github.com/InauguralSystems/EigenScript/tree/main/examples)** —
  Idiomatic examples in the language repo.
- **[Browser playground](https://inauguralsystems.github.io/EigenScript/playground/)** —
  Run EigenScript in the browser (WASM, interpreter-only).

## Editor Integrations

- **[VS Code](https://github.com/InauguralSystems/EigenScript/tree/main/editors/vscode)** —
  TextMate grammar in the language repo.
- **[Vim](https://github.com/InauguralSystems/EigenScript/tree/main/editors/vim)** —
  Syntax file in the language repo.
- **LSP** — `eigenscript --lsp` speaks the Language Server Protocol;
  point any LSP-capable editor at it.

## Showcase

Real programs and projects written in EigenScript. (Empty for now —
open a PR when you ship something.)

## Contributing

PRs welcome. Two rules:

1. **One package per PR.** Add your entry under the right heading;
   if no heading fits, propose a new one in the PR description.
2. **Format**: `**[name](url)** — one-line description.` Keep
   descriptions to a single line; let the linked README do the
   selling.

Inclusion is at maintainer discretion: the package should solve a
real problem, have a tagged release, and have at least a smoke test
under CI. See [CONTRIBUTING.md in the language repo](https://github.com/InauguralSystems/EigenScript/blob/main/CONTRIBUTING.md#publishing-a-package)
for naming + versioning guidance.

## License

The list itself is [CC0](LICENSE) — public domain, do whatever.
Individual linked projects keep their own licenses.
