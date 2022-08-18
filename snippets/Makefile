%.pdf: %.tex
	latexmk $*.tex
	mv target/$*.pdf $*.pdf

%.svg: %.pdf
	pdf2svg $*.pdf $@

.PHONY: all
all: uh.svg dh.svg dh-failed-cast.svg hir.svg mir.svg mir-opt.svg lir.svg lir-rules.svg

.PHONY: clean
clean: 
	rm -f *.svg *.pdf
