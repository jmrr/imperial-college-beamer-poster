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

Personal information that is in the footer is declared in the style file (very bottom of beamerthemeICL.sty).


## Build instructions

Using `pdflatex`:
```
pdflatex -synctex=1 -interaction=nonstopmode beamerposterICL.tex
bibtex beamerposterICL.aux
pdflatex -synctex=1 -interaction=nonstopmode beamerposterICL.tex
```

