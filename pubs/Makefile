# project name
NAME=benhachey
.PHONY = all clean purge

all: paper

paper:
	pdflatex ${NAME}
	bibtex ${NAME}
	pdflatex ${NAME}
	pdflatex ${NAME}

clean:
	rm -f `find . -name '*.log'`
	rm -f `find . -name '*.dvi'`
	rm -f `find . -name '*.ps'`
	rm -f `find . -name '*.aux'`
	rm -f `find . -name '*.blg'`
	rm -f `find . -name '*.bbl'`
	rm -f `find . -name '*.toc'`
	rm -f `find . -name '*.lof'`
	rm -f `find . -name '*.lot'`
	rm -f `find . -name '*~'`
	rm -f `find . -name '*.out'`
	rm -f `find . -name '*.nav'`
	rm -f `find . -name '*.snm'`
	rm -f `find . -name '*.vrb'`

purge:  clean
	rm -f ${NAME}.pdf