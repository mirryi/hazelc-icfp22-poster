%.pdf: %.tex
	latexmk $*.tex
	mv target/$*.pdf $*.pdf

%.svg: %.pdf
	pdf2svg $*.pdf $@

all: uh.svg dh.svg hir.svg mir.svg mir-opt.svg lir.svg lir-rules.svg
