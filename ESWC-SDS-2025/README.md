# Semantics in Dataspaces (SDS 2025)
<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [Semantics in Dataspaces (SDS 2025)](#semantics-in-dataspaces-sds-2025)
    - [Call](#call)
        - [Important Dates](#important-dates)
        - [Topics of Interest](#topics-of-interest)
        - [Important: Integration with W3C Dataspaces Community Group](#important-integration-with-w3c-dataspaces-community-group)
        - [Submission](#submission)
        - [Workshop Chairs](#workshop-chairs)
    - [Instructions](#instructions)
- [quarto add quarto-journals/elsevier](#quarto-add-quarto-journalselsevier)
- [quarto install tinytex](#quarto-install-tinytex)
- [make](#make)
- [Install Zotero standalone: https://www.zotero.org/download/](#install-zotero-standalone-httpswwwzoteroorgdownload)
- [Install https://retorque.re/zotero-better-bibtex/](#install-httpsretorquerezotero-better-bibtex)
- [Add citations to https://www.zotero.org/groups/5539665/underpin/library, folder "paper-citations> EBDVF-2024" (also add to "Data Space Semantic Interoperability")](#add-citations-to-httpswwwzoteroorggroups5539665underpinlibrary-folder-paper-citations-ebdvf-2024-also-add-to-data-space-semantic-interoperability)
- [Have Zotero running](#have-zotero-running)
- [(After each addition of a citation to that collection)](#after-each-addition-of-a-citation-to-that-collection)
- [make bib-*](#make-bib-)

<!-- markdown-toc end -->

## Call
https://dbis.rwth-aachen.de/SDS25/

3 Jan 2025 to public-dataspaces@w3.org:

You are cordially invited to contribute to our upcoming workshop, The Third International Workshop on Semantics in Dataspaces (SDS 2025), on 01 or 02 June 2025, to be held in conjunction with ESWC25 in Portoroz, Slovenia.

Overview
- Dataspaces, which are critical to seamless and trusted data sharing, have gained prominence in Europe with the European Data Governance Act (DGA). This legislation defines terms and aims to increase trust, expand data availability, and promote common dataspaces. The impact spans sectors such as data providers, researchers, businesses, and citizens. Initiatives like the European Open Science Cloud and the adoption of the FAIR Data Principles further contribute to the relevance of dataspaces. Efficient data sharing within dataspaces requires semantic interoperability, for which the Semantic Web community has a long history of developing RDF-based solutions.
- The Semantics in Dataspaces (SDS) 2025 workshop seeks to advance semantic methods and solutions for dataspaces by encouraging collaboration between researchers and practitioners. It aims to advance the expressiveness, standardization, and integration of semantic technologies in dataspace architectures. The workshop promises interactive sessions, presentations, and discussions to drive advances in semantics for dataspaces.

### Important Dates
- Submission: March 06, 2025
- Notification of acceptance: April 03, 2025
- Registration: tba
- Camera-Ready submission: April 17, 2025
- Workshop at ESWC 2025: Full day on June 01 or 02, 2025

### Topics of Interest
The topics of this workshop aim to discuss both conceptual definitions and actual implementations of dataspaces, and to promote the role of the Semantic Web in these. The main topics of this workshop include but are not limited to:

Conceptual Perspective:
- Surveys on definitions and visions
- What are dataspaces and what are their core elements?
- How are components and data life cycles structured?
- Formal models of dataspaces
- The role of stakeholders in decision processes
- Impact and potential of unique identifiers
- Conceptual reusable assets

State-of-the-art Implementations:
- How do arising dataspaces coincide/differ with each other?
- Requirements of customers, stakeholders, and politics
- Who drives their implementations and what are their technology readiness levels?
- Common reusable elements and standards
- Gap between academic definitions and actual implementations

Semantics for Dataspaces:
- Review of arising dataspaces with a focus on the Semantic Web
- Potential of methods and solutions from the Semantic Web for dataspaces
- Tailored benefits of ontologies, unique identifiers, algorithms, etc.
- Measuring political, practical, scientific, performance, etc. challenges for adoption
- Investigating and reviewing the role of artificial intelligence and large language models for dataspaces

### Important: Integration with W3C Dataspaces Community Group

To foster collaboration and create a lasting impact, authors must align their work with the ongoing efforts of the W3C Dataspaces Community Group, as documented in the GitHub issues repository. This integration will promote consistency, reusability, and collective progress in addressing the core challenges of dataspaces.

Authors are therefore required to identify which generic challenge their paper addresses within this repository, and explicitly highlight this in their paper. If the challenge is not listed, they must contribute by adding it to the repository. Use cases are encouraged but must also be documented in the GitHub repository to ensure they contribute to a shared knowledge base.

Please note that papers that do not clearly integrate with the W3C Community Group’s ongoing efforts, including the identification of a relevant challenge or use case in the repository, may be subject to desk rejection.

### Submission
We welcome the following types of contributions:
- Full research papers with original research (10-15 pages).
- Short papers may contain original research in progress (5-9 pages).
- Position / vision papers may discuss vision statements or arguable opinions (up to 5 pages).
- System / demo papers may contain descriptions of prototypes, demos or software systems (5-9 pages).
- Resource papers may contain descriptions of resources related to the workshop topics, such as ontologies, knowledge graphs, ground truth datasets, etc (5-9 pages).

Workshop papers must be self-contained and in English. They should not have been previously published, should not be considered for publication, and should not be under review for another workshop, conference, or journal. Papers must be submitted according to the ESWC submission guidelines. The PDF files must have all non-standard fonts embedded. Papers will be evaluated according to their significance, originality, technical content, style, clarity, and relevance to the workshop.

https://dbis.rwth-aachen.de/SDS25/#submission:
- Submit your contributions via EasyChair: https://easychair.org/my/conference?conf=sds25
- Overleaf and Latex templates based on single-column LNCS, tailored for the CEUR-WS proceedings

### Workshop Chairs
All questions should be emailed to sds@dbis.rwth-aachen.de.
- Johannes Theissen-Lipp, RWTH Aachen University, Germany
- Pieter Colpaert, Ghent University, Belgium
- André Pomp, University of Wuppertal, Germany
- Edward Curry, University of Galway, Ireland
- Stefan Decker, RWTH Aachen University, Germany

## Instructions
- install quarto (https://quarto.org/docs/download/, or I've done it with "scoop"
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
