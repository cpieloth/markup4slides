all: html

html: slides.html

clean:
	$(RM) *.html

%.html: %.ad
	asciidoc -b slidy $<
