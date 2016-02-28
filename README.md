# Imperial College London beamer poster template

Unofficial Imperial College London poster template based on the LaTeX [Beamer][beamer] class

[beamer]: https://bitbucket.org/rivanvx/beamer/wiki/Home

##### Required files needed are:
```
beamerposterICL.tex
beamerthemeICL.sty
./images/Imperial_2_Pantones.eps (logo)
posterRefs.bib
```

* **Personal information** the personal details in the footer may be declared in the style file (very bottom of beamerthemeICL.sty).
* **Orientation portrait/landscape** and **size**: This can be changed in preamble line:

```
\usepackage[orientation=landscape,size=a0]{beamerposter}\usepackage[orientation=portrait,size=a0]{beamerposter}  % e.g. custom size poster. Change orientation here

```

## Build instructions

Using `pdflatex`:
```
pdflatex -synctex=1 -interaction=nonstopmode beamerposterICL.tex
bibtex beamerposterICL.aux
pdflatex -synctex=1 -interaction=nonstopmode beamerposterICL.tex
```

