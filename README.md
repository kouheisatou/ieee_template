# ICMU2025 Paper Template

## Overview
This repository provides a LaTeX template for writing papers for ICMU2025.

## Features
- Output files are generated in the `out` directory.
- Uses the IEEE standard style (IEEEtran class and bst).
- Uses `pdflatex` for building.

## Environment Setup
### 1. Install TeX Live
If you do not have a LaTeX environment, it is recommended to install TeX Live.
- On macOS:
  ```sh
  brew install --cask mactex
  # Add TeX Live to PATH if necessary
  sudo tlmgr path add
  ```
- On Windows:
  Download the installer from the official TeX Live website (https://tug.org/texlive/) and follow the instructions.
- On Linux:
  ```sh
  sudo apt-get install texlive-full
  ```

### 2. Install latexmk
In most cases, latexmk is included with TeX Live. If you need to install it separately:
- On macOS/Linux:
  ```sh
  sudo tlmgr install latexmk
  ```
- On Windows:
  Use the TeX Live package manager (tlmgr) to add `latexmk`.

## How to Build
1. Install the required LaTeX environment (such as TeX Live).
2. Run the following command to generate the PDF:

```sh
latexmk
```

Or, to explicitly specify `pdflatex`:

```sh
latexmk -pdf
```

## File Structure
- `main.tex` : Main TeX file
- `IEEEtran.cls` : IEEE paper class file
- `IEEEtran.bst` : IEEE bibliography style
- `out/` : Output directory (auto-generated)
- `.latexmkrc` : Configuration file for latexmk

## Notes
- The IEEEtran class and style files are specified in `main.tex`.
- Please use `.bib` files for references.
