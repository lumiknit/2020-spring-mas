OUT = out.pdf
.PHONY: all base.pdf clean

all: open

base.pdf:
	pdflatex -halt-on-error base.tex

$(OUT): base.pdf
	cp base.pdf $(OUT)

open: $(OUT)
	open $(OUT)
	
clean:
	rm -f *.aux *.log *.pdf
