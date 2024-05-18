base:=main

all: references.bib
	./latexrun \
	  --latex-args="-shell-escape" \
	  $(base).tex

#	  --bibtex-cmd="biber" \

references.bib:
	cat $(shell find ../resources/ -iname "*.bib") \
	  > references.bib

clean:
	./latexrun --clean-all

.PHONY: all clean references.bib
