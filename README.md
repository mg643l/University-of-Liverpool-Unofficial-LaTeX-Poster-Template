# Unofficial University of Liverpool Poster Template

This repository contains an unofficial LaTeX beamer poster template for the University of Liverpool.

The color palette uses the official University of Liverpool brand colours, sourced from:
https://www.liverpool.ac.uk/intranet/brand/

## Copyright

Copyright (c) 2026 Joseph Wood (845jwood@gmail.com)

## License

This project is licensed under the MIT License.

See [LICENSE.md](LICENSE.md) for the full license text.

## Build (PDFLaTeX)

This template can be built with PDFLaTeX, including bibliography generation.

### Option 1: VS Code + LaTeX Workshop (recommended)

1. Open the folder in VS Code.
2. Open [poster.tex](poster.tex).
3. Run the LaTeX Workshop build command:
	- `Ctrl+Shift+P` -> `LaTeX Workshop: Build LaTeX project`
4. Make sure your recipe uses PDFLaTeX (e.g. `latexmk (pdfLaTeX)`).

If LaTeX Workshop is using LuaLaTeX by default, switch the recipe in settings to a PDFLaTeX recipe.

### Option 2: Terminal build

From the project root:

```powershell
latexmk -pdf poster.tex
```

To clean auxiliary files:

```powershell
latexmk -c
```

## Main Files

- [poster.tex](poster.tex): Main poster source
- [poster.bib](poster.bib): Bibliography entries
- [beamerthemegemini.sty](beamerthemegemini.sty): Base theme
- [beamercolorthemeliverpool.sty](beamercolorthemeliverpool.sty): Liverpool color theme
