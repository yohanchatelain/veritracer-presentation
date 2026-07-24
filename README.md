# VeriTracer Presentation

Slides for *VeriTracer: Context-enriched tracer for floating-point arithmetic analysis*, presented at ARITH 25, Amherst MA USA, June 2018.

[![Build slides](https://github.com/yohanchatelain/veritracer-presentation/actions/workflows/build.yml/badge.svg)](https://github.com/yohanchatelain/veritracer-presentation/actions/workflows/build.yml)
[![Download PDF](https://img.shields.io/badge/slides-PDF-red?logo=adobeacrobatreader)](https://github.com/yohanchatelain/veritracer-presentation/releases/latest/download/veritracer-presentation.pdf)

## Repository structure

```
demo.tex     Main Beamer presentation source
demo.bib     Bibliography
latexmkrc    latexmk build configuration
sty/         Beamer theme (metropolis) style files
figures/     Images and PDF figures used by the slides
```

## Building locally

```sh
latexmk demo.tex
```

`latexmk` picks up the build rules from `latexmkrc` (shell-escape enabled for `minted`, `TEXINPUTS` pointed at `sty/` and `figures/`). The compiled `demo.pdf` is produced in the repository root.

## Continuous integration

Every push to `main` builds the slides via GitHub Actions, uploads the PDF as a workflow artifact, and republishes it to the `latest` release so it stays available from the badge above without needing to open the Actions tab.
