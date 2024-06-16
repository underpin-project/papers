# install quarto (https://quarto.org/docs/download/, or I've done it with "scoop")
# quarto add quarto-journals/elsevier
# quarto install tinytex
# make
paper.pdf: paper.qmd bibliography.bib
	quarto render paper.qmd --to elsevier-pdf 

# Install Zotero standalone: https://www.zotero.org/download/
# Install https://retorque.re/zotero-better-bibtex/
# Add citations to https://www.zotero.org/groups/5539665/underpin/library, folder "paper-citations> EBDVF-2024" (also add to "Data Space Semantic Interoperability")
# Have Zotero running
# (After each addition of a citation to that collection)
# make bib-*
bib-vlado::
	curl http://127.0.0.1:23119/better-bibtex/export/collection?/3128938/DS4FVYLV.bibtex -o bibliography.bib

bib-petar::	
	curl http://127.0.0.1:23119/better-bibtex/export/collection?/6/DS4FVYLV.bibtex -o bibliography.bib
