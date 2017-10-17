MD_DOCS := $(wildcard *.md)

HTML_DOCS = $(MD_DOCS:.md=.html)

%.html : %.md
	sed -e 's/\.md)/.html)/g' < $< | pandoc --to html5 -o $@

all: $(HTML_DOCS)
