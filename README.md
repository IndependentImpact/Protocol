# Independent Impact Protocol

This repository contains the specification for the **Independent Impact Protocol** — a decentralized, Web3-based standard for environmental and social impact accounting. It is designed as an open, meritocratic alternative to traditional carbon-offset registries and ESG standards bodies, built on the [Hedera Hashgraph](https://hedera.com/) distributed ledger.

## Repository Structure

The specification is split across numbered Markdown files, each covering a distinct topic:

| File | Section |
|------|---------|
| `00-Protocol.md` | Master document (assembles all sections via `!INCLUDE` directives) |
| `01-a-Introduction.md` | Introduction & platform overview |
| `02-a-OverviewOfConceptsAndTerminology.md` | Core concepts and terminology |
| `02-b-Bibliography.md` | Inline bibliography references |
| `03-a-Principles.md` | Governing principles (general, impact, accounting, reporting) |
| `04-a-AgentReputationSystem.md` | Agent reputation system (Knowledge & Skills + Conduct) |
| `05-a-ImpactScoringSystem.md` | Impact scoring system (ImSco) |
| `06-a-OtherScoringSystems.md` | Indicator, method, instrument, and course scoring |
| `07-a-Bounties.md` | Bounty system for tasks and collaboration |
| `08-a-Voting.md` | Reputation-weighted voting mechanisms |
| `09-a-Commenting.md` | Commenting on platform entities |
| `10-a-AntiGamingMechanisms.md` | Anti-gaming and security mechanisms |
| `11-a-TechnicalImplementation.md` | Technical implementation (Hedera integration) |
| `12-Bibliography.md` | Full bibliography |

## Compiling the Master Document

`00-Protocol.md` uses `!INCLUDE` directives to pull in every section. To compile these into a single Markdown file you need [MarkdownPP](https://github.com/jreese/markdown-pp) (Markdown Pre-Processor).

### 1. Install MarkdownPP

```bash
pip install MarkdownPP
```

### 2. Compile

Run the following command from the root of the repository:

```bash
markdown-pp 00-Protocol.md -o compiled-protocol.md
```

This produces `compiled-protocol.md` — a single Markdown file containing the full protocol.

### 3. (Optional) Convert to PDF or HTML

Once you have `compiled-protocol.md` you can convert it to other formats with [Pandoc](https://pandoc.org/):

```bash
# HTML
pandoc compiled-protocol.md -o protocol.html

# PDF (requires a LaTeX distribution such as TeX Live or MiKTeX)
pandoc compiled-protocol.md -o protocol.pdf
```

> **Note:** PDF and HTML output files are excluded from version control via `.gitignore`.

