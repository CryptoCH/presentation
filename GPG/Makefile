SLIDES=gpg

all: ${SLIDES}.html

.PHONY: clean

style.css: style.sass *.sass
	sass style.sass > $@

${SLIDES}.html: ${SLIDES}.md style.css
	pandoc -t dzslides -s ${SLIDES}.md -o $@ -i --self-contained --css style.css

clean:
	rm -rf ${SLIDES}.html
	rm -rf *.css
