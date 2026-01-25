# Makefile for Resonance Architecture Publications

LATEX = xelatex
LATEX_FLAGS = -interaction=nonstopmode -halt-on-error

# Find all .tex files in the current directory
SOURCES := $(wildcard *.tex)
# Convert the list of .tex files to a list of .pdf files
PDFS := $(SOURCES:.tex=.pdf)

.PHONY: all clean

all: $(PDFS)

# Rule to build a PDF from a TeX file
%.pdf: %.tex references.bib
	@echo "Building $@..."
	$(LATEX) $(LATEX_FLAGS) $<
	bibtex $(subst .tex,,$<)
	$(LATEX) $(LATEX_FLAGS) $<
	$(LATEX) $(LATEX_FLAGS) $<
	@echo "$@ has been successfully built."

clean:
	rm -f *.aux *.log *.out *.toc *.pdf *.fls *.fdb_latexmk
	@echo "Cleaned build artifacts."