all: html pdf

html: slides.html
pdf: slides.pdf

clean:
	$(RM) *.html

clean-all: clean
	$(RM) -rf venv

%.html: %.md
	landslide $< -d $@

%.pdf: %.md
	landslide $< -d $@
