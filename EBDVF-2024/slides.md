## Raising the Role of Vocabulary Hubs for Semantic Data Interoperability in Dataspaces
Robert David,
Petar Ivanov,
Vladimir Alexiev

![](img/swc-logo-web.svg)
![](img/Ontotext-Logo-vector.svg)
![](img/underpin_logo_horizontal_icon_title_tagline_color_light_bg.svg)

3rd Workshop on Semantic Interoperability in Data Spaces 

Oct 1st, 2024, Budapest, Hungary

***
### Introduction

- the european data economy depends on the availability of data 
- technological foundation + services and tools to make use of it
- different industries and communities
- machine-learning systems need high-quality training data
    - predictive maintenance

Data space standards, like IDS, provide 
**technical foundation** and **data sovereignty** principles.

***
### Motivation

- interoperability is key for making use of shared data
- syntactic data exchange already solved, I.e. defined data formats and exchange standards
- semantic interoperability still an open challenge
- Starting point: IDS RAM and IM defines semantic metadata
- we need to extend it to cover **semantic interoperability for data**

***
### Approach
- Semantic Interoperability via a **Semantic Layer** for Dataspaces
    - based on IDS Vocabulary Hub
    - based on knowledge graph (KG) technologies
    - implemented by **GraphDB + PoolParty** products
- services + data for semantic interoperability
- data discovery & harmonisation
- semantic metadata + data for discovery and integration

***
### Use Cases
2 running projects:
DataBri-X
- energy community simulation and prediction
- legal knowledge graph + document analysis

UNDERPIN
- refinery predictive maintenance
- wind farms predictive maintenance


***
### Approach

Semantic Layer supports structured and unstructured data interlinked in the KG.
Structured
- Ontology-Based Data Access (OBDA)
- RDB to RDF Mapping Language (R2RML)
- CSV on the Web (CSVW)

Unstructured
- semantic document annotations via KG entities


***

### Approach

Semantic Layer supports inference services.

- reasoning based on W3C recommendations OWL & SHACL
- inference tagging expands semantic annotations in documents
- vocabulary crosswalks connect different similar vocabularies
- metadata inference to determine specific vocabularies for domains

***
### Integration Architecture

![](img/architecture.png)

***
### Data Consumer Benefits

- harmonized and semantically integrated data from disparate providers
- richer metadata descriptions
- incoming data bound dynamically to semantic descriptions
- richer discovery / easier data querying
- vocabulary crosswalks: expand queries and annotations by traversing the interlinked graph


***
### Conclusions and Future Work

A Semantic Layer for Data Spaces enchances the role of the Vocabulary Hub by interlinking structured and unstructured data from multiple providers and multiple formats into a KG based on a common harmonized model.
This improves both the discoverability and description of said data.

Future work:

- Implement use cases for richer discoverability, harmonized querying and support for different content types.
- Explore how ML can benefit regarding quality in practice when providing consolidated and cleaned data via dataspaces.
- Discuss how we can extend the IDS RAM with services to improve the support for semantic interoperability provided by our solution.
