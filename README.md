# Repolex Knowledge Graph of deepset-ai/n8n-nodes-haystack-enterprise-mcp

RDF knowledge graph data for [deepset-ai/n8n-nodes-haystack-enterprise-mcp](https://github.com/deepset-ai/n8n-nodes-haystack-enterprise-mcp), parsed by [repolex](https://repolex.ai).

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
rlex download deepset-ai/n8n-nodes-haystack-enterprise-mcp
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 8abb74b3041cbfb1b5fd743128cf61f7186dee96
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 8abb74b3041cbfb1b5fd743128cf61f7186dee96
│           └── chunk-001.nq.gz
├── blob
│   ├── 14c97be8b8a67bbe8e2af1a4ad9153006cf3dc77.nq.gz
│   ├── 1f426c3a9284acad684ff0fda03a5577947162e9.nq.gz
│   ├── 292037551b6542489c359814467decbeb2d5fcb2.nq.gz
│   ├── 2bef00e2d0030cc59301124387a9cfa83885f455.nq.gz
│   ├── 320c107b3e5f0e08a9b443602d4063fb7c71cd33.nq.gz
│   ├── 42ef55d76b3878a07b5c128f14b4de3ca67802a6.nq.gz
│   ├── 43c994c2d3617f947bcb5adf1933e21dabe46bb5.nq.gz
│   ├── 4c3425bea5738db9ec9272be81b2cb3525227eb0.nq.gz
│   ├── 4e52a3ca3ef82fd4e8b1b0471937bdb57604d2de.nq.gz
│   ├── 53e7da497316f253a7d7383f0a0a4738c0d3780d.nq.gz
│   ├── 6e671e02f25255f880b8e5029310d5138ffe6ab3.nq.gz
│   ├── 825f5556e0d71edb4c2638ad7ff07772224bad42.nq.gz
│   ├── 8bd3d3386579902064117a4fae0677b4e5edadb4.nq.gz
│   ├── a4cfa3b19d64a4c41089f9d210fb93ad85645475.nq.gz
│   ├── a6478abe413accd4eaa893315121dd89616012bb.nq.gz
│   ├── aa4f3f5e62691ad2c720a09d4d52dd9cd1d294ee.nq.gz
│   ├── adc4e1a7b2eb1d0ebd503456272e1d06c395ff34.nq.gz
│   ├── b37b83bd19d1636045e6cf951e30a1f489c4e7ac.nq.gz
│   ├── b38b29c9575b0c7e7c58c7224972f1845eeda498.nq.gz
│   ├── b50c6b7a3c347ab391c3b3450a1fcfb4ab4b9912.nq.gz
│   ├── bb9f865a3a241317bc2fb95f3de51a7519d4a74e.nq.gz
│   ├── be498f91f82b3735b2bc11647a97147ed0f836d4.nq.gz
│   ├── d14443bbcedfef3b216c7d9828ba06f3150554f3.nq.gz
│   ├── da77319485347c0a3424f0ffef08534ac8c19f90.nq.gz
│   ├── f6008ac0b501714dee73b5cde96ff7f0f4445a72.nq.gz
│   └── fa7b5decac838346f4c558db62635d4dd4768d16.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 8abb74b3041cbfb1b5fd743128cf61f7186dee96.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 33 files
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

[deepset-ai/n8n-nodes-haystack-enterprise-mcp](https://github.com/deepset-ai/n8n-nodes-haystack-enterprise-mcp)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
