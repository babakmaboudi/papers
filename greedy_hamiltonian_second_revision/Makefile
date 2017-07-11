FILE=paper

all: $(FILE).pdf

clean:
	rm -rf *.aux *.blg *.out *.bbl *.log *.ps *.pdf *.dvi

$(FILE): $(FILE)
	latex $(FILE).tex
	dvips $(FILE).dvi
	ps2pdf $(FILE).ps

bib: $(FILE)
	latex $(FILE).tex
	dvips $(FILE).dvi
	ps2pdf $(FILE).ps
	bibtex $(FILE)
	latex $(FILE).tex
	dvips $(FILE).dvi
	ps2pdf $(FILE).ps
	latex $(FILE).tex
	dvips $(FILE).dvi
	ps2pdf $(FILE).ps
