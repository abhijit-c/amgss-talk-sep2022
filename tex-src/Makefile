JobName=slides-amgss-april2022
TeX=pdflatex
LatexFlags= -jobname=$(JobName) --shell-escape

default:
	make build
	biber $(JobName)
	make build
	make build
	make clean

build:
	$(TeX) $(LatexFlags) main.tex

clean:
	rm -f $(JobName).log $(JobName).aux $(JobName).out $(JobName).toc *.cpt
	rm -f $(JobName).nav $(JobName).snm $(JobName).vrb
	rm -f $(JobName).bbl $(JobName).blg $(JobName).bcf $(JobName).run.xml
	rm -rf _minted-*
