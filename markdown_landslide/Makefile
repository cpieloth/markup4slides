all: html

html: slides.html
pdf: slides.pdf

clean:
	$(RM) *.html *.pdf

clean-all: clean
	$(RM) -rf venv

%.html: %.md
	landslide $< -d $@

%.pdf: %.md
	landslide $< -d $@
