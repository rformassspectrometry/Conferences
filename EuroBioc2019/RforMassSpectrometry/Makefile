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


r4ms.pdf: r4ms.tex
	pdflatex r4ms.tex

.PHONY: all clean

clean:
	rm -f *~
	rm -f $(LATEXFILES)
	rm -f .Rhistory .Makefile.swp

