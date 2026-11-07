# Repolex Knowledge Graph of ansible-collections/community.google

RDF knowledge graph data for [ansible-collections/community.google](https://github.com/ansible-collections/community.google), parsed by [repolex](https://repolex.ai).

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
rlex download ansible-collections/community.google
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 44bae7c578954bf47819706870e050210981e0df
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 44bae7c578954bf47819706870e050210981e0df
│           └── chunk-001.nq.gz
├── blob
│   ├── 038e5eb48e4050aa58f7e556bcbd4db0d7fcd76c.nq.gz
│   ├── 068725436e1c903247ef812fadcd0fd8f8b4e693.nq.gz
│   ├── 0972cd2e8e58d51f20c6b0d23d8f89154c7ac076.nq.gz
│   ├── 0e3093d8b257b2cccfee3fe3dc9bdd212a9efc01.nq.gz
│   ├── 13fbdc44dfbe49d29d08675ca6a4a3fc07b3487d.nq.gz
│   ├── 16494a447a4ee1de242f78471d817519ccd1344b.nq.gz
│   ├── 1feac1e03c51f7e9d66a52355c0cf712fa113622.nq.gz
│   ├── 27122af06a50ce7ed7ff6c6479316757771fed9c.nq.gz
│   ├── 2d9230c8f7bb6a5521e7420faa0bffbf35709bef.nq.gz
│   ├── 3a06f18d206bb720b96afe60b1e87832572c1c92.nq.gz
│   ├── 3eed2df2fcd4efeb7ade752d7c91317baee06441.nq.gz
│   ├── 48395f2a964b3381d382c984b3e848d5a296c9ba.nq.gz
│   ├── 4af3186328668f2d1cf2377ad697f582a869c254.nq.gz
│   ├── 6723f464884f73c9397d7a4aebc2fb47b83b8129.nq.gz
│   ├── 7098f705d7ce5d16d23f113afbc7d0a6b6b1b5b0.nq.gz
│   ├── 740c8115458b12e3a8f24220e718e0b33ef2e16d.nq.gz
│   ├── 7698e3c5ecec7d0afed70eeb1c5de52295a48a4a.nq.gz
│   ├── 845234ff748a2b0c3ce7ce0318112f8775ff87e2.nq.gz
│   ├── 88eed5c9f33c8bbd68f68e73402ab7e4be4d66a6.nq.gz
│   ├── 8bb88c798277ac803d5878e0cbd3d8e0284747f2.nq.gz
│   ├── 8e33c3d75ceb7b310a71dd342da3355fdda4183d.nq.gz
│   ├── 98f08ad6a8474fbcc3e338436bae46663d4aa4ae.nq.gz
│   ├── 9e53e1e23d1b2a9ad6f158713a498b4f5cfc5321.nq.gz
│   ├── a034f3b6c97a12fb6e1b28573913f84fbcecb0b9.nq.gz
│   ├── a4b1ec4e4712e3c340479a959d6943901a29cee0.nq.gz
│   ├── a9ad45e4d669016261b4f7a55d7061274a3438dd.nq.gz
│   ├── a9d40b8b58ab89ac9d4ed75a4ed798adcc197a40.nq.gz
│   ├── aac114060fee635ebf5fd72a18b48f280d42e490.nq.gz
│   ├── ae58c5c59d9c66180ba03b7a68597f52137f1e2e.nq.gz
│   ├── af27a9c4ab3ef33dcb1a9b0c69a51e83cd44b1ad.nq.gz
│   ├── c233efa5ec7658843baf0bca8282f46c46cfa355.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ec436b4221c286a85babc558a668e69cb09bed93.nq.gz
│   ├── ec804d278dd0e7a099f440a84579edf8a6c59eef.nq.gz
│   ├── f288702d2fa16d3cdf0035b15a9fcbc552cd88e7.nq.gz
│   ├── f2dffaa46ff20e4c1e06938e578136d18d1de0b4.nq.gz
│   ├── fd47167f93c914966a60bc2e0f049bb26d7bfc2f.nq.gz
│   ├── febfd24256e93391387cadd632fbb390123e2da3.nq.gz
│   └── ff29b56de10efbbc546505ed6ea063b2808d3d91.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 44bae7c578954bf47819706870e050210981e0df.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 47 files
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

[ansible-collections/community.google](https://github.com/ansible-collections/community.google)

---
*Parsed on 2026-11-07 by [repolex](https://repolex.ai)*
