# SNMP-Research

This repository contains a small research report about **SNMP (Simple Network Management Protocol)**, produced in the context of the course **Análise de Comunicações em Rede** (Master’s in Computer Security Engineering) at **Instituto Politécnico de Beja (ESTIG)**.

The report covers:
- SNMP fundamentals (manager/agent model, MIB/OIDs, operations)
- SNMP operations (GET, GET-NEXT, GET-BULK, SET, TRAP, INFORM)
- A comparison of **SNMPv1**, **SNMPv2c**, and **SNMPv3**
- Security evolution and practical implementation considerations

## Repository contents

- `LaTeX Report/Relatorio.tex` — main LaTeX source
- `LaTeX Report/Relatorio.pdf` — compiled PDF output
- `LaTeX Report/Recursos/` — images and bibliography resources
- `LICENSE` — repository license file

## Quick access

- **PDF (compiled report):** `LaTeX Report/Relatorio.pdf`
- **LaTeX source:** `LaTeX Report/Relatorio.tex`

## Build the PDF (LaTeX)

### Option A — latexmk (recommended)
From the repo root:

```bash
cd "LaTeX Report"
latexmk -pdf -interaction=nonstopmode -shell-escape Relatorio.tex
```

### Option B — pdflatex + biber
If your TeX distribution doesn’t include `latexmk`:

```bash
cd "LaTeX Report"
pdflatex Relatorio.tex
biber Relatorio
pdflatex Relatorio.tex
pdflatex Relatorio.tex
```

> Note: The project uses `biblatex` with `backend=biber`, so `biber` is required for the bibliography.

## Notes

This repo includes LaTeX build artifacts (e.g., `.aux`, `.log`, `.toc`, etc.) alongside the source. If you prefer a cleaner repository, you can add a `.gitignore` and keep only the source + PDF.

## Authors

- Martinho José Novo Caeiro
- Paulo António Tavares Abade

## License

See `LICENSE`.
