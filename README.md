# Resume

[![Build CV (XeLaTeX)](https://github.com/reiidoda/resume/actions/workflows/build-cv.yml/badge.svg)](https://github.com/reiidoda/resume/actions/workflows/build-cv.yml)

Single-source LaTeX CV with automated PDF build and GitHub Pages publishing.

**Live CV:** https://reiidoda.github.io/resume/  
**PDF:** https://reiidoda.github.io/resume/rei_doda_cv.pdf

---

## Overview

- **Canonical LaTeX source:** `cv/rei_doda_cv.tex`
- **Local build output:** `cv/output/rei_doda_cv.pdf`
- **Published site:** deployed to GitHub Pages via GitHub Actions

---

## Quick build (local)

### Prerequisites (macOS)
Install a TeX distribution that includes **XeLaTeX**:
- **MacTeX** (recommended) or **BasicTeX**

### Prerequisites (Windows)
Install a TeX distribution that includes **XeLaTeX**:
- **MiKTeX** (recommended) or **TeX Live**

Make sure `xelatex` is available in your PATH (MiKTeX can do this during installation).

### Build (macOS / Linux / Git Bash / WSL)
```sh
cd cv
mkdir -p output
xelatex -interaction=nonstopmode -halt-on-error -output-directory=output rei_doda_cv.tex
```

### Build (Windows PowerShell)

```powershell
cd cv
New-Item -ItemType Directory -Force -Path output | Out-Null
xelatex -interaction=nonstopmode -halt-on-error -output-directory=output rei_doda_cv.tex
```