# Repolex Knowledge Graph of minitest/minitest

RDF knowledge graph data for [minitest/minitest](https://github.com/minitest/minitest), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download minitest/minitest
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 339492cbaec5c460ec278e754199619d6431af35
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 339492cbaec5c460ec278e754199619d6431af35.nq.gz
│   └── repolex
│       └── 339492cbaec5c460ec278e754199619d6431af35
│           └── chunk-001.nq.gz
├── blob
│   ├── 0505c2c438db379f2d93b4ac74bcee4a3b5b508b.nq.gz
│   ├── 0c5e23fb313e3fdb3a122b8dec4a4345f9d99e21.nq.gz
│   ├── 14e32eb566e2f1bd37aba7584b68a497fad509d9.nq.gz
│   ├── 1987d122d13335f87708406f436f25c33e4c9023.nq.gz
│   ├── 23c2a229cc0f0ea518631cea864857b797d855a0.nq.gz
│   ├── 2b88f80e567f8355540e72afe15f07b444582109.nq.gz
│   ├── 2d7751bf3aa8eea3d03c0961ab29f4be27fa7362.nq.gz
│   ├── 3395c1af8741f05cd7e5d56e93e63d091970e7ec.nq.gz
│   ├── 3bc893d14e6e2571cab264ff9eecc672d83cb526.nq.gz
│   ├── 3be59cbfbb3959bcb89a781b545b875bfc792766.nq.gz
│   ├── 402713b0d15d7a63b0a136b518df07c570bd37dc.nq.gz
│   ├── 523495eb2a60d78e96efc570e3f1c845d98dcf8a.nq.gz
│   ├── 58902f5826efc24aee5f66207d54f98fdf61a756.nq.gz
│   ├── 5bbde6a197ae091cfd3ec3f4865cbbd78c0f79da.nq.gz
│   ├── 5d0526b4f2c720b207aaffdf5dc6e5caea0e7297.nq.gz
│   ├── 63b0d1dfb56d86a267c6c8ce54d7c9ba3b7b4a03.nq.gz
│   ├── 671b0c93f70e6642d0a25a90f7a35a482794eb64.nq.gz
│   ├── 69881c6f938ac09171bf46c963decaaf2113b217.nq.gz
│   ├── 7a1db21d14c0d91f135b14ef4c2b82bc6ba4244f.nq.gz
│   ├── 7ba0c5361e0eef3fcfe2403ec16fc30a6c6ae2fa.nq.gz
│   ├── 7ef36ec1afaf3da0d7c5c6da18ca3a221e6ecbf2.nq.gz
│   ├── 7fbbc307d5d487d9c41823c4ee2b4844560a2f07.nq.gz
│   ├── 941c19880cc7a9d395d6d805c4b33c162725db95.nq.gz
│   ├── 9d3534323dbe83cba08c32b46649dc5ec53736b1.nq.gz
│   ├── 9e17e0386d5541b0382b702c233564512ed54ef4.nq.gz
│   ├── afbfa7aa669ad15b4976254cb7b9f545c982a4ee.nq.gz
│   ├── afd2f08ca112640921e2495af943f6a65ecb286d.nq.gz
│   ├── b1370e14b400064247c8ca345955ccc2b7b26c22.nq.gz
│   ├── bb638b00079e7bf8a90cbc4b5d6363fd13e42f8a.nq.gz
│   ├── be73ae874f6c9cfb81707cb791241520447b692f.nq.gz
│   ├── bf7ec8a313fac570b34a789aed614bc81ad2f7d7.nq.gz
│   ├── c15a257792bf8e38822b12169ad65b1b17465acc.nq.gz
│   ├── c2fdb4abcab958f079583a7950060800d9200399.nq.gz
│   ├── c9461064494381895c4180bfd5322a33509ca3b1.nq.gz
│   ├── cff3bdaa412ca23598bc4079bf7769080dc2ef0c.nq.gz
│   ├── d9dc16c86ea85d3673717e7e798e2160f0a9686d.nq.gz
│   ├── da5513232a96ae09068b0d49c928a406b4086f31.nq.gz
│   ├── de070a9f42af5abcde9a488d2ee5ae4169b0a427.nq.gz
│   ├── de745ea1fdde4879ddd2921dc438b358b9cec527.nq.gz
│   ├── e08e9b78af0d6e3b4f5b2401edca0fb07f7c8640.nq.gz
│   ├── eab4dbf0fe65eff57cf2c4f5d20d007aeb2c155b.nq.gz
│   └── ef144d464a3a1cd8737f3d335867faad8eea257d.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 339492cbaec5c460ec278e754199619d6431af35.nq.gz
├── filetree
│   └── 339492cbaec5c460ec278e754199619d6431af35.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 52 files
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

## Source repository

[minitest/minitest](https://github.com/minitest/minitest)

---
*Parsed on 2026-04-10 by [repolex](https://repolex.ai)*
