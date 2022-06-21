TEXARGS= --interaction=nonstopmode --halt-on-error
TEXC = pdflatex $(TEXARGS)

all: pdf

pdf:
	@$(TEXC) repport
	@bibtex repport
	@$(TEXC) repport
	@$(TEXC) repport

affiche:
	@evince repport.pdf &


clean:
	@echo "Cleaning files..."
	@rm -f  *.aux
	@rm -f *.log
	@rm -f *.sage
	@rm -f *.scmd
	@rm -f *.sout
	@rm -f *.bbl
	@rm -f *.fls
	@rm -f *.toc
	@rm -f *.blg
	@rm -f *.fdb_latexmk
	@rm -f *.synctex.gz
	@rm -rf *.out
	@rm -rf *.nav
	@rm -rf *.snm
	@rm -rf *busy*
	@rm -rf *.pytxcode
	@rm -rf *.pyc