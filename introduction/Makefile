SLIDES=introduction

all: ${SLIDES}.html

.PHONY: clean

${SLIDES}.html: ${SLIDES}.md
	pandoc -t dzslides -s $^ -o $@ --css style.css -i --self-contained

clean:
	rm -rf ${SLIDES}.html
