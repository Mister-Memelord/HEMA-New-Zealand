MD_ARGS = -V papersize:a4 -V geometry:margin=3cm -V colorlinks=true -V linkcolor=blue -V date="`date +'%-dth %B %Y'`" --number-sections --shift-heading-level-by=-1
MDS = $(wildcard *.md)
PDFS = $(MDS:.md=.pdf)


.PHONY: all clean

all: $(PDFS)

%.pdf: %.md
	pandoc $(MD_ARGS) -o $@ $<


clean:
	-rm *.pdf
