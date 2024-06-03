# install quarto (https://quarto.org/docs/download/, or I've done it with "scoop")
# quarto add quarto-journals/acm
# quarto install tinytex
# make
paper.pdf: paper.qmd
	quarto render $^ --to acm-pdf 

# Install Zotero standalone: https://www.zotero.org/download/
# Install https://retorque.re/zotero-better-bibtex/
# Add citations to https://www.zotero.org/groups/5539665/underpin/library, folder "paper-citations> EBDVF-2024" (also add to "Data Space Semantic Interoperability")
# Have Zotero running
# (After each addition of a citation to that collection)
# make bibliography.bib
bibliography.bib::
	curl http://127.0.0.1:23119/better-bibtex/export/collection?/3128938/DS4FVYLV.bibtex -o $@
