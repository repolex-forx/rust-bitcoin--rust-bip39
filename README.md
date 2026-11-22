# Repolex Knowledge Graph of rust-bitcoin/rust-bip39

RDF knowledge graph data for [rust-bitcoin/rust-bip39](https://github.com/rust-bitcoin/rust-bip39), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download rust-bitcoin/rust-bip39
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── d6dbc31678cc507c8cae62b3a059b0b48e866436
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── d6dbc31678cc507c8cae62b3a059b0b48e866436.nq.gz
│   └── repolex
│       └── d6dbc31678cc507c8cae62b3a059b0b48e866436
│           └── chunk-001.nq.gz
├── blob
│   ├── 072a883c1f320d418dcc44b25090d4cd21b7c40a.nq.gz
│   ├── 0d244aa0dbd5f5efec12c445f1383fecfd27b904.nq.gz
│   ├── 199f96100e7a8b3112d7d0ae47f5cadab25f409c.nq.gz
│   ├── 2796cdcc244ac52a537d026a5203e86bda46cb91.nq.gz
│   ├── 2a3b14ef88496dde78f656a91d66fe10b8f1b016.nq.gz
│   ├── 326ca554ce875afb062b6835c6738ecb9b097bb1.nq.gz
│   ├── 46b960f50aaa56ef59b24e09dba818ad6a197746.nq.gz
│   ├── 4b555f42f7210d694f6e8345a27620c3b03e2a20.nq.gz
│   ├── 4d4ece172b24bbfc566caefcae539f17b3ea85e2.nq.gz
│   ├── 548571735fe1daa057ac787fd0f3b8a41006ac98.nq.gz
│   ├── 6498fda0b80c8f56ccb7679ea8d1852db77d3767.nq.gz
│   ├── 6ca207ef004cb69d03041e7e5c288a2be4968045.nq.gz
│   ├── 711fe6a93e2ea53f9204c66596c4b2e09ea8df84.nq.gz
│   ├── 85ddac4abcd973505dab9bd88ca9f61390530157.nq.gz
│   ├── 87689635188d4502ff95863146205d520d976b78.nq.gz
│   ├── 89303804f4d9984177b8ceacfe0b10aa3823f57a.nq.gz
│   ├── 96ef6c0b944e24fc22f51f18136cd62ffd5b0b8f.nq.gz
│   ├── 99da0de20ce0c5d1dfadc4bff0fa1ca7e871741d.nq.gz
│   ├── a11b129fe8e9aa30aeeeb172170a9c74e25ffd3c.nq.gz
│   ├── b02b4f8fe5d865430a1d21ee1b0f0a417e86ab58.nq.gz
│   ├── d6c65534375e36b8888fe9b0e0c2bcc55021834a.nq.gz
│   ├── d730fd76573f1360930a94b1e3503216217952dd.nq.gz
│   ├── e6d9ba01bc44f365383d0d9bcc741e9867732f23.nq.gz
│   ├── ea56c0589bd8a181efa3d471147d4aa4ffe0b8ec.nq.gz
│   ├── ee31cdcbc025e60ac0743cf48913c5befac943a4.nq.gz
│   └── f8eb81092901dabb1e99f50c2b43e62571b5bbd0.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── d6dbc31678cc507c8cae62b3a059b0b48e866436.nq.gz
├── filetree
│   └── d6dbc31678cc507c8cae62b3a059b0b48e866436.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 36 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[rust-bitcoin/rust-bip39](https://github.com/rust-bitcoin/rust-bip39)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
