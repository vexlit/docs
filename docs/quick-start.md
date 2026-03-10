# Quick Start

## 1. Install the CLI

```bash
npm install -g @vexlit/cli
```

## 2. Scan Your Project

```bash
cd your-project
vexlit scan .
```

## 3. Review Results

VEXLIT outputs a table of findings with:
- **Severity** — Critical, High, Medium, Low, Info
- **Rule ID** — e.g., VEXLIT-001 (SQL Injection)
- **CWE** — Common Weakness Enumeration mapping
- **Location** — File path and line number
- **Description** — What's wrong and how to fix it

## 4. Generate SARIF Report

```bash
vexlit scan . --format sarif -o results.sarif
```

Upload the SARIF file to GitHub's Security tab for integrated vulnerability tracking.

## Next Steps

- [Configure severity thresholds](configuration.md)
- [Set up GitHub Action](../docs/cicd.md)
- [Install VSCode extension](vscode.md)
