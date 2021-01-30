all: sol1.pdf sol2.pdf

%.pdf: %.tex
	pdflatex $<
	rm -f sols.aux
	cat *.aux > sols.aux
	cat sols.aux > $(patsubst %.tex,%.aux,$<)
	pdflatex $<
	rm -f sols.aux
