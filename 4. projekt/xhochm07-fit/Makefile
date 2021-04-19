NAME=proj4
LOGIN=xhochm07

all: bibtex or biblatex

biblatex:
	pdflatex $(NAME).tex
	biber $(NAME).bcf
	pdflatex $(NAME).tex
bibtex:
	pdflatex $(NAME).tex
	bibtex $(NAME).aux
	pdflatex $(NAME).tex
	pdflatex $(NAME).tex
zip:
	zip $(LOGIN)-fit.zip *.tex Makefile *.bib *.bst

clean:
	rm -f $(NAME).{aux,dvi,log,pdf,ps,blg,bbl,log} $(LOGIN)-fit.zip
