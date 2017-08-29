#!/bin/bash
# LaTeX Makefile

FILE=main

all: $(FILE).pdf

.PHONY: clean
clean:
	rm -fv *.aux *.out *.log *.bbl *.blg *.brf *.idx *.toc
	rm -fv exercicios/*.aux exercicios/*.out exercicios/*.log exercicios/*.bbl exercicios/*.blg exercicios/*.brf exercicios/*.idx exercicios/*.toc


clean_all:
	rm -fv *.aux *.out *.log *.bbl *.blg *.brf *.idx *.toc *.pdf *.lof *.lot
	rm -fv exercicios/*.aux exercicios/*.out exercicios/*.log exercicios/*.bbl exercicios/*.blg exercicios/*.brf exercicios/*.idx exercicios/*.toc exercicios/*.pdf exercicios/*.lof exercicios/*.lot

$(FILE).pdf: $(FILE).tex
	pdflatex $(FILE)
	pdflatex $(FILE)
	bibtex $(FILE)
	pdflatex $(FILE)
	pdflatex $(FILE)
