# semimorg

A monorepo scaffold for a planned code-modernization tool. The repository is in its initial state: no crates or packages have been added yet.

## Status

Early scaffold. The `crates/` and `packages/` directories exist but are empty (each contains only a placeholder `_` file to allow git to track the directory). The Cargo workspace has `members = []` and will not build anything. The npm workspace similarly has no members.

Two commits exist: the initial scaffold and a README update.

## Intended purpose (from project description)

The stated goal is code modernization without "morging" — the name is a portmanteau suggesting migration/refactoring done without the typical merge-chaos. The design intent is to use a "powerful, deterministic compiler" as the core engine, with AI involvement pushed back to the compiler-development stage rather than applied at runtime/usage time.

In practice: no implementation exists yet, so the actual behavior of the tool is not determined by code.

## Repository layout

```
semimorg/
├── Cargo.toml       # Virtual Cargo workspace (no members)
├── package.json     # npm workspace package (@portal-solutions/semimorg, no members)
├── crates/          # Intended location for Rust crates (currently empty)
└── packages/        # Intended location for JS/TS packages (currently empty)
```

## Tech stack (planned)

- **Rust** — primary implementation language (Cargo workspace)
- **Node.js / JavaScript** — secondary tooling (npm workspace, `type: "module"`)
- **zshy** (`^0.7.0`) — only current dev dependency, a shell-scripting library for Node

## License

MPL-2.0

## Source

GitHub: [portal-co/semimorg](https://github.com/portal-co/semimorg)
