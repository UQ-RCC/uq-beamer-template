# UQ LaTeX Beamer Template

#### Author: Zane van Iperen &lt;z.vaniperen@uq.edu.au&gt;

This is a best-effort recreation of UQ's "Own the Unknown" PowerPoint template in LaTeX.

## Things to note:
* I've only done one of the thank you pages. There's 4.
* The LinkedIn icon mismatches the rest, so I ignore it.
* Any included images are ripped straight from `UQ-PowerPoint-template.pptx` (not included).

## Usage:

You must use the `xelatex` compile. See `example.tex` for a more detailed example.
```tex
\documentclass[xetex,aspectratio=169]{beamer}

\usetheme{uq2019}

\begin{document}
    \begin{frame}
        \frametitle{Sample frame title}
        This is a text in the first frame.
        This is a text in the first frame.
        This is a text in the first frame.
    \end{frame}
\end{document}
```

## Installation:

Simply install it into `$TEXMF`:
```bash
TEXMF=$(kpsewhich -var-value=TEXMFHOME)
mkdir -p "$TEXMF/tex/latex"
git -C "$TEXMF/tex/latex" clone https://github.com/UQ-RCC/uq-beamer-template.git
```
