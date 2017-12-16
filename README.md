# Cookiecutter latex letter template

## Setup
Install cookiecutter:

```bash
conda install cookiecutter
```

## New latex project

```bash
# first time
cookiecutter git@gitlab.com:s-schmeier/cookie-latex-letter.git

# subsequent use
cookiecutter cookie-latex-letter
```

## Within the project

### General command sequence

Makefile is included in each document directory.

```bash
# to create pdf
make pdf

# to continues recompile on change (use Skip pdf viewer on MacOS)
make pdfview

# remove artifacts
make clean
```

### Emacs

Add this to `.emacs` to enable pdflatex as default:

```
# .emacs
(setq TeX-PDF-mode t)
```

Use this shortcuts in emacs:

```
# Compile latex
C-c C-c RET

# Revert PDF
C-x C-v RET
```

