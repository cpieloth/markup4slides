all: html

html: slides.html

clean:
	$(RM) *.html

clean-all: clean
	$(RM) -rf .bundle Gemfile.lock

%.html: %.ad
	bundle exec asciidoctor-revealjs -a revealjsdir=https://cdnjs.cloudflare.com/ajax/libs/reveal.js/3.6.0 $<
