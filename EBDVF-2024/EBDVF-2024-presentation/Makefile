all: presentation.html presentation.pdf

presentation.html: presentation.qmd
	quarto render $^ --to revealjs
	
presentation.pdf: presentation.html
	/home/ptr/node_modules/.bin/decktape $^ $@
