# Makefile pour beamer LaTeX

IMG_SVG=$(shell find img/ -name *.svg | sed 's/svg/png/')

all : svgs ble_cdl.pdf

%.pdf : %.tex
	pdflatex -shell-escape $?
	pdflatex -shell-escape $?

svgs : $(IMG_SVG)

%.png : %.svg
	convert -density 300 $? $@	

clean :
	rm -f *.aux
	rm -f *.log
	rm -f *.nav
	rm -f *.out
	rm -f *.snm
	rm -f *.toc
	rm -f *.vrb
	rm -f *.pdf
	rm -f *.pyg

mr_proper : clean
	rm -f $(IMG_SVG)
