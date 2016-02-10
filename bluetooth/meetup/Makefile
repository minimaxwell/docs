# Makefile pour beamer LaTeX

IMG_SVG=$(shell find img/ -name *.svg | sed 's/svg/png/')

all : svgs bt_meetup.pdf

%.pdf : %.tex
	pdflatex $?
	pdflatex $?

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

mr_proper : 
	rm -f *.pdf
	rm -f $(IMG_SVG)
