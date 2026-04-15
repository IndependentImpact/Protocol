# Independent Impact Protocol

This repository contains the specification for the **Independent Impact Protocol** — a decentralized, Web3-based standard for environmental and social impact accounting. It is designed as an open, meritocratic alternative to traditional carbon-offset registries and ESG standards bodies, built on the [Hedera Hashgraph](https://hedera.com/) distributed ledger.

## Repository Structure

The specification is split across numbered Markdown files, each covering a distinct topic:

| File | Section |
|------|---------|
| `00-Protocol.md` | Master document title (compiled together with all sections by pandoc) |
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

The repository includes a `pandoc-defaults.yaml` file that lists every section in order.
Compilation requires [Pandoc](https://pandoc.org/) — no other tools are needed.

### 1. Install Pandoc

Follow the [official installation guide](https://pandoc.org/installing.html) for your operating system, or use a package manager:

```bash
# macOS
brew install pandoc

# Debian / Ubuntu
sudo apt install pandoc

# Windows (winget)
winget install --id JohnMacFarlane.Pandoc
```

### 2. Compile to Markdown

Run the following command from the root of the repository:

```bash
pandoc --defaults pandoc-defaults.yaml -o compiled-protocol.md
```

This produces `compiled-protocol.md` — a single Markdown file containing the full protocol.

### 3. Compile to Other Formats

Pandoc can produce the final document directly in other formats without an intermediate Markdown step:

```bash
# HTML
pandoc --defaults pandoc-defaults.yaml -o protocol.html

# PDF (requires a LaTeX distribution such as TeX Live or MiKTeX)
pandoc --defaults pandoc-defaults.yaml -o protocol.pdf

# DOCX
pandoc --defaults pandoc-defaults.yaml -o protocol.docx
```

> **Note:** Output files (`.html`, `.pdf`, `.docx`) are excluded from version control via `.gitignore`.

