all: html

html: slides.html
pdf: slides.pdf

clean:
	$(RM) *.html *.pdf

%.html: %.ad
	asciidoc -b slidy $<

%.pdf: %.html
	pandoc $< -t beamer -o $@
