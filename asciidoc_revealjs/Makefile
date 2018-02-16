all: html

html: slides.html
pdf: slides.pdf

clean:
	$(RM) *.html *.pdf

clean-all: clean
	$(RM) -rf .bundle Gemfile.lock

%.html: %.ad
	bundle exec asciidoctor-revealjs -a revealjsdir=https://cdnjs.cloudflare.com/ajax/libs/reveal.js/3.6.0 $<

%.pdf: %.html
	pandoc $< -t beamer -o $@
