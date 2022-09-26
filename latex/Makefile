
ppc:
	clean
	pdflatex -output-dir=tmp ppc-info-net.tex
	bibtex tmp/ppc-info-net
	pdflatex -output-dir=tmp ppc-info-net.tex
	pdflatex -output-dir=tmp ppc-info-net.tex
	$(MAKE) clean

flow: clean
	pdflatex -output-dir=tmp flow.tex
	mv tmp/flow.pdf flow.pdf
	$(MAKE) clean
all: clean 
	$(MAKE) flow 
	$(MAKE) ppc

clean:
	rm -f tmp/*
	rmdir tmp
	mkdir tmp
