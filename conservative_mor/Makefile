FILE=paper

all: $(FILE).pdf

clean:
	rm -rf *.aux *.blg *.out *.bbl *.log *.ps *.pdf *.dvi *.lot *.toc *.lof *.idx

$(FILE): $(FILE)
	pdflatex $(FILE).tex

bib: $(FILE)
	pdflatex $(FILE).tex
	bibtex $(FILE)
	pdflatex $(FILE).tex
	pdflatex $(FILE).tex
