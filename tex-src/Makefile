BASENAME = main

all: pdf

pdf::
	latexmk --pdf ${BASENAME}

ps::
	latexmk --ps ${BASENAME}

clean::
	latexmk -c ${BASENAME}
	rm -f ${BASENAME}.pdf
	rm -f ${BASENAME}.bbl
	rm -f ${BASENAME}.run.xml
	rm -f ${BASENAME}.synctex.gz
