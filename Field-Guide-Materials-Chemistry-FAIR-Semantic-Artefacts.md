# Field Guide for Increasing the FAIR Maturity of Materials and Chemistry Semantic Artefacts

Developed by Harmonised Terminologies and Schemas for FAIR Data in Materials Science and Related Domains Working Group

[Group Homepage](https://www.rd-alliance.org/groups/harmonised-terminologies-and-schemas-fair-data-materials-science-and-related-domains-wg/activity/)

## Executive summary

The FAIR data principles present an aspirational set of foundational principles—Findability, Accessibility, Interoperability, and Reusability—that guide data producers as they work to improve the machine actionability of their data and metadata. The FAIR data principles do not explicitly define a set of actions to increase FAIR maturity. Instead, they describe a continuum of features, attributes, and behaviors that move a digital resource closer to that goal \[[FAIR](https://doi.org/10.1038/sdata.2016.18), [FAIRmaturity](https://zenodo.org/records/3909563#.YGRNnq8za70)\]. While there have been some efforts to provide technical approaches to improve FAIR maturity within the materials and chemistry disciplines through the development of semantic artefacts and services (e.g., [Materials Registries](https://www.rd-alliance.org/groups/working-group-international-materials-resource-registries/)), most efforts have not been widely adopted. One key factor inhibiting the success of efforts to develop semantic artefacts for the materials and chemistry disciplines has been that the resulting semantic artefacts created by past working groups often have low FAIR maturity and do not have sufficient relationships to other semantic artefacts within and outside and outside the domain. This document serves as a practical field guide for individuals and groups who are developing or maintaining semantic artefacts and mappings for the materials and chemistry disciplines.

## Objectives

This document seeks to provide practical guidance on how to increase the FAIR maturity of semantic artefacts for materials science and related domains.

## Target audience

This document targets individuals and groups actively working to develop or maintain semantic artefacts and mappings for the materials and chemistry disciplines.

## Definitions

For definitions of important terms, see also [https://zenodo.org/records/6675295](https://zenodo.org/records/6675295)

- **Controlled Vocabulary** — A controlled vocabulary is a curated, normalised, restricted list of terms for a specific use or context. Thesauri and taxonomies are types of controlled vocabularies, but not all controlled vocabularies are thesauri or taxonomies \[[FAIRsemantics](https://doi.org/10.5281/zenodo.6276576)\]. This is shown in relation to other concepts in Figure 1\.
- **Dataset** — A collection of data, published or curated by a single agent, and available for access or download in one or more representations. \[[DCAT](https://www.w3.org/TR/vocab-dcat-3/)\]
- **Digital Object** — A sequence of bits, or a set of sequences of bits, incorporating a work or portion of a work or other information in which a party has rights or interests, or in which there is value, each of the sequences being structured in a way that is interpretable by one or more of the computational facilities, and having as an essential element an associated unique persistent identifier \[[DOA](https://www.dona.net/digitalobjectarchitecture)\].
- **Glossary** — A glossary is an alphabetical list of terms in a particular domain of knowledge with the definitions for those terms \[[FAIRsemantics](https://doi.org/10.5281/zenodo.6276576)\]. This is shown in relation to other concepts in Figure 1\.
- **Knowledge Graph** — While there isn’t a widely-accepted definition, knowledge graphs are generally an interlinked collection of facts, concepts, entities, and relationships that uses a graph-structured data model or topology to represent and operate on data \[[Wikipedia](https://en.wikipedia.org/wiki/Knowledge_graph), [ontotext](https://www.ontotext.com/knowledgehub/fundamentals/what-is-a-knowledge-graph/), [IBM](https://www.ibm.com/think/topics/knowledge-graph)\].
- **Material** — Any natural or processed mass of matter that is an input to or output from a materials engineering or manufacturing process.
- **Metadata** —  Data about data. Information describing the characteristics of data, such as structural metadata describing data structures and descriptive metadata describing data contents and permissible usage.
- **Ontology** — An ontology is a formal version of a thesaurus where relations are described using a formal system such as Description Logic (DL) to mathematically classify individuals of classes and properties \[[FAIRsemantics](https://doi.org/10.5281/zenodo.6276576)\]. This is shown in relation to other concepts in Figure 1\.
- **Ontological Mapping** —  Semantic bridges that link entities from different yet overlapping ontologies in order to support knowledge sharing and reuse.\[[https://doi.org/10.3233/WEB-180371](https://doi.org/10.3233/WEB-180371)\].  Mappings document the correspondence between entities (concepts, terms) \[[https://doi.org/10.1093/database/baac035](https://doi.org/10.1093/database/baac035)\] , see also \[[Wikipedia](https://en.wikipedia.org/wiki/Ontology_alignment)\]
- **Schema** — A schema is a structured representation that defines the rules, constraints, and organization of data within a specific format, such as XML or JSON, to ensure its validity and consistency. It acts as a blueprint that specifies the expected structure, data types, required elements, and relationships within a dataset. Schemas are used for validation, enabling automated checks to confirm whether a given instance record conforms to the defined rules, ensuring that the data is both syntactically and semantically correct according to the schema's specifications.
- **Schema Language** — A schema language is a formal language used to define the structure, constraints, and validation rules for data in a specific format, such as XML or JSON. It provides a standardized way to describe the expected organization, data types, cardinality, and relationships within a dataset. Schema languages enable automated validation of data by ensuring that it conforms to the specified rules and requirements. Examples include XML Schema Definition (XSD) for XML and JSON Schema for JSON.
- **Semantic Artefact** — A semantic artefact is defined in this work as a machine-actionable formalisation of a conceptualisation, enabling sharing and reuse by humans and machines. These artefacts may have a broad range of formalisation, from loose sets of terms, taxonomies, thesauri to higher-order logics. \[[FAIRsemantics](https://doi.org/10.5281/zenodo.6276576)\]
- **Taxonomy** — A taxonomy is a controlled vocabulary with a hierarchical structure used to classify things or concepts. Terms within a taxonomy have relations to other terms (parent/broader term, child/narrower term).
- **Term/class/concept** — A term/class/concept is an individual element with a unique semantic interpretation, represented with a unique identifier \[[FAIRsemantics](https://doi.org/10.5281/zenodo.6276576)\]. This is shown in relation to other concepts in Figure 1\.
- **Thesaurus** — A thesaurus is essentially a controlled vocabulary following a standard structure, where all terms have relationships of three kinds to each other: hierarchical (broader term/narrower term), associative (related term), and equivalent (use/used for or see/ seen from). Some terms in thesauri might have additional explanatory notes, such as scope notes (brief explanations about the coverage of the term or of how it should be used in indexing) or history notes \[[FAIRsemantics](https://doi.org/10.5281/zenodo.6276576)\]. This is shown in relation to other concepts in Figure 1\.

![A representation of different semantic concepts shown in an onion-like diagram where complex approaches, such as formal ontologies, encompass simpler technologies, such as vocabularies.](semantic-onion.svg)
**Figure 1:** A visual representation of different semantic concepts and artefacts. Figure derived from \[[FAIRsemantics](https://doi.org/10.5281/zenodo.6276576)\].

## FAIR Maturity Indicators for Semantic Artefacts

In this section, maturity indicators for Semantic Artefacts are reviewed and listed. They are grouped according to their relevance to Findability, Accessibility, Interoperability and Reusability.  Where indicators have an impact on more than one aspect of FAIR, they are listed in each relevant category.

Input has been obtained from existing recommendations:

- Yann Le Franc, Luiz Bonino, Hanna Koivula, Jessica Parland-von Essen, & Robert Pergl. (2022). D2.8 FAIR Semantics Recommendations Third Iteration (V1.0). Zenodo. [https://doi.org/10.5281/zenodo.6675295](https://doi.org/10.5281/zenodo.6675295)
  The items below starting with P-Rec. are from this resource.
- Daniel Garijo and Maria Poveda. Best Practices for Implementing FAIR Vocabularies and Ontologies on the Web. [https://dgarijo.com/papers/best\_practices2020.pdf](https://dgarijo.com/papers/best_practices2020.pdf) and [https://ceur-ws.org/Vol-2980/paper321.pdf](https://ceur-ws.org/Vol-2980/paper321.pdf)

Also from input received during RDA VP22 [RDA VP22 Collaborative Notes - Kickoff of Harmonised terminologies and schemas for FAIR data in materials science and related domains Working Group](https://docs.google.com/document/d/1-sya46TD5keH7xtvPqaObQCe162OY7x3Hv8-ENuQkQ0/edit)

We introduced the following sub-categories:

- Metadata
- Identifiers
- Repositories
- API/Protocols
- Licensing
- Policies
- Formats and standards
- Provenance
- Mappings and alignments

### Findability

- Metadata
  - Rich metadata about the usage of the semantic artefact and its limitations are available.
  - P-Rec. 3: A common minimum metadata schema must be used to describe semantic artefacts and their content
  - Minimum metadata schema:
    - Metadata for Ontology Description and Publication Ontology \- [https://github.com/FAIR-IMPACT/MOD](https://github.com/FAIR-IMPACT/MOD), version 3.2 (machine actionable DCAT profile)
    - Paper on minimum metadata Clement Jonquet, Biswanath Dutta, Luiz O. Bonino da Silva Santos, Robert Pergl, Yann Le Franc. Common Minimum Metadata for FAIR Semantic Artefacts. Onto4FAIR 2023 \- 2nd Workshop on Ontologies for FAIR and FAIR Ontologies, C. Trojahn; L. O. Bonino da Silva Santos; G. Guizzardi; C. Jonquet, Jul 2023, Sherbrooke, Canada. ⟨[hal-04106533v2](https://hal.science/hal-04106533)⟩
    - FAIR IMPACT follow-up: [https://zenodo.org/records/12579779](https://zenodo.org/records/12579779)
- Identifiers
  - Each term, concept, etc. has an identifier.
  - P-Rec. 1: Globally Unique, Persistent and Resolvable Identifiers (GUPRIs, also known as PIDs) must be used for Semantic Artefacts, their content (terms/concepts/classes and relations), and their versions.
  - P-Rec. 2: GUPRIs must be used for Semantic Artefact Metadata Records. Metadata and data must be published separately, even if it is managed jointly.

- Repositories
  - Semantic repositories should be indexed in a searchable resource.
  - P-Rec. 4: Semantic Artefact and its content should be published in an appropriate semantic repository
  - P-Rec.5: Semantic repositories must offer a [common API](https://github.com/FAIR-IMPACT/MOD-API) to access Semantic Artefacts and their content in various serialisations for both use/ reuse and indexation by any search engine
  - P-Rec. 6: Build semantic artefact search engines that operate across different semantic repositories
  - For a detailed discussion of maturity of semantic artefact catalogues, see [https://www.nature.com/articles/s41597-024-03185-4](https://www.nature.com/articles/s41597-024-03185-4)

### Accessibility

- API/Protocols
  - semantic artefacts are retrievable via open/standard protocol
  - Sub-elements of semantic artefacts are retrievable via GUPRI/PID using open and standard protocol
  - P-Rec. 5: Semantic repositories must offer a common API to access Semantic Artefacts and their content in various serialisations for both use/ reuse and indexation by any search engines
  - P-Rec. 7: Repositories should offer a secure protocol and user access control functionalities
  - Common API model (FAIR IMPACT): [MOD-API](https://github.com/FAIR-IMPACT/MOD-API)
- Licensing
  - Semantic artefacts should be as open as possible, with clear access rights for the relevant communities
- Policies
  - P-Rec. 8: Human and machine-readable persistence policies for semantic artefacts metadata and data must be defined

### Interoperability

- [Mappings](https://github.com/mapping-commons/rda-fair-mappings) and alignments, semantic interoperability
  - Rich and comprehensive mappings to other semantic artefacts should be provided
  - Connection to well-known top- and middle-level ontologies are recommended
  - P-Rec. 10: Foundational Ontologies should be used to align semantic artefacts
  - P-Rec. 12: Semantic mappings between the different elements of semantic artefacts should be serialised in machine-readable formats
  - P-Rec. 13: Crosswalks, mappings and bridging between semantic artefacts should be documented, published and curated
  - Provide reference to controlled vocabularies where possible and in the absence of those, contribute to their development.
- Formats and standards
  - The [FAIR Semantics Recommendations](https://zenodo.org/records/6675295) are:
    - P-Rec. 9: Semantic artefacts must be made available as a minimum portfolio of common serialisation formats.
    - P-Rec 11: A standardised language should be used for describing high expressivity semantic artefacts.
  - We further recommend that
    - Metadata of semantic artefacts must be available as RDF, serialised as JSON-LD (preferred), Turtle and RDF-XML.
    - Content of a semantic artefact must be serialised  in a textual, machine-actionable format, e.g., JSON-LD, JSON, XML
    - Metadata of semantic artefacts must provide all required information to process and interpret its content. This is especially true for non-strict defined formats like CSV (RFC 4180, RFC 7111\)
  - Utilise existing domain standards, for example standard definitions and notations (e.g., in chemistry \- Gold Book, InChI/SMILES/IUPAC nomenclature)
- Provenance
  - P-Rec. 15: Provenance information regarding the reuse of components from third-party semantic artefacts should be made explicit
  - Include versions wherever applicable

### Reusability

- Licensing for reuse
  - P-Rec. 16: The semantic artefact must be clearly licenced for reuse by machines and humans
  - We recommend the use of permissive licences.
- Metadata
  - Rich (more than minimum) metadata must be provided about the usage of the semantic artefact and its limitations.
- Provenance
  - P-Rec. 15: Provenance information regarding the reuse of components from third-party semantic artefacts should be made explicit
  - P-Rec. 17: Provenance must be clear for both humans and machines
  - Provenance of the terms and concepts and their definitions from other resources (e.g. Wikipedia) used in semantic artefacts should be provided.
- Mapping and alignments, semantic interoperability
  - P-Rec. 12: Semantic mappings between the different elements of semantic artefacts should be serialised in machine-readable formats
  - P-Rec. 13: Crosswalks, mappings and bridging between semantic artefacts should be documented, published and curated
  - Human-readable documentation and support tools (people have to build the machines to read the data) should be provided.
- Formats and standards
  - Data structures with low human dependence and high preservability, written in accordance with international standards (e.g. W3C) should be used.
