LATEXFILES = *.aux\
	*.snm\
	*.nav\
	*.vrb\
	*.bbl\
	*.blg\
	*.ilg\
	*.log\
	*.nlo\
	*.nls\
	*.toc\
	*.aux\
	Rplots.pdf\
	*.dvi\
	*.map\
	*.out\
	*.figlist\
	*.dep\
	*.dpth\
	*-blx.bib\
	*.run.xml\
	*.makefile


poster.pdf: poster.Rnw
	R --vanilla --silent -e "knitr::knit('poster.Rnw')"
	pdflatex poster.tex
	bibtex poster.aux
	pdflatex poster.tex

.PHONY: all clean

clean:
	rm -f *~
	rm -f $(LATEXFILES)
	rm -f .Rhistory .Makefile.swp

