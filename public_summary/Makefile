MAIN = main
LATEX = pdflatex -interaction=nonstopmode -halt-on-error

.PHONY: all clean

all:
	$(LATEX) $(MAIN).tex
	$(LATEX) $(MAIN).tex

clean:
	rm -f $(MAIN).aux $(MAIN).log $(MAIN).out $(MAIN).toc $(MAIN).pdf
