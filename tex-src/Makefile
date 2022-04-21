JobName=slides-amgss-april2022
TeX=pdflatex
LatexFlags= -jobname=$(JobName) --shell-escape

default:
	make build
	bibtex $(JobName)
	make build
	#make build
	make clean

build:
	$(TeX) $(LatexFlags) main.tex

clean:
	rm -f $(JobName).log $(JobName).aux $(JobName).out $(JobName).toc *.cpt
	rm -f $(JobName).nav $(JobName).snm $(JobName).vrb
	rm -rf _minted-*
