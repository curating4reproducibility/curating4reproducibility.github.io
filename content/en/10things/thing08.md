---
title: "Thing 8: Metadata"
description: "Information about the research compendium and its components is embedded in a standardized, machine-readable code."
draft: false
weight: 80
toc: true
---
**Related FAIR Principles: [ALL](https://www.go-fair.org/fair-principles/)**

**[Related FAIR4RS Guiding Principle](https://doi.org/10.15497/RDA00068): ALL**

Metadata are information that describe an object and may convey details such as who created the object, when and how the object was created, its purpose, its license or other terms of use, and how it is related to other objects.

**Ideally structured and machine-readable, metadata about the research compendium and its component parts can be preserved and made accessible alongside the compendium to facilitate discovery and use.**

Ask: is information about the research process (data, analysis, and production), the research compendium, and each of its components FAIR: findable, accessible, interoperable, and reusable?

The FAIR guiding principles make specific recommendations on types of metadata and ways of encoding it that are especially important for making data and code available. For Findability, identifiers are important as well as rich metadata (see below). For Accessibility making clear how to access the data or software (see [Thing 6](../thing06)), and ensuring that metadata remains available are important. For Interoperability, the use of standards in encoding metadata are important (see below). Finally, Provenance (see [Thing 7](../thing07)) and licenses (see [Thing 6](../thing06)) are specifically mentioned in the context of enabling Reusability.

{{< details "Get Started" >}}
Machine readable metadata refers to information structured such that it can be automatically read and processed by a computer. There are various metadata schemas available to accommodate the standards, requirements, and conventions of various domains, a number of which have tools or templates that can be used to generate structured metadata or verify the integrity of a structured metadata record.

### Standards

A metadata standard is a set of required and optional metadata elements used to describe objects in a consistent manner. Use of a metadata standard can increase the probability of interoperability and contribute to a shared understanding of the meaning of the data.

To find a standard suitable for a particular discipline or data type, start with a metadata directory. Where a disciplinary standard doesn’t exist, it is better to adopt terms from an existing standard(s), or use a general-purpose metadata schema such as DCMI Metadata Terms or DataCite Metadata Schema. You may also consider joining the Research Data Alliance to start work on defining a standard.

#### Sample metadata directories

- The [Metadata Standards Catalog](http://rd-alliance.github.io/metadata-directory/standards/), created by the Metadata Standards Directory Working Group at the Research Data Alliance (RDA) is a directory of standards in use by various disciplines. Other relevant RDA work has been published by the [Metadata Interest Group](https://www.rd-alliance.org/groups/metadata-ig.html) and [Research Metadata Schemas Working Group](https://www.rd-alliance.org/groups/research-metadata-schemas-wg), including [Guidelines for Publishing Structured Metadata on the Web](https://www.rd-alliance.org/system/files/documents/Guidelines%20for%20publishing%20structured%20data_V3.0_20210615.pdf).
- INCF standards and best practices portfolio for neuroscience includes many examples of discipline and method specific standards. [https://www.incf.org/resources/sbps](https://www.incf.org/resources/sbps)
- FAIRSharing.org is a curated resource with many data and metadata standards, which can be narrowed by domain. [https://fairsharing.org/standards/](https://fairsharing.org/standards/)

#### Sample metadata standards

- Neuroscience: Brain Imaging Data Structure ([BIDS](https://bids.neuroimaging.io/)) is a standard for organizing and describing neuroimaging and behavioral data.
  - **Gorgolewski, K., Auer, T., Calhoun, V. et al. The brain imaging data structure, a format for organizing and describing outputs of neuroimaging experiments. *Sci Data 3*, 160044 (2016). [https://doi.org/10.1038/sdata.2016.44](https://doi.org/10.1038/sdata.2016.44)**<br>
The Brain Imaging Data Structure (BIDS) is a standard for organizing and describing MRI datasets. The BIDS standard uses file formats compatible with existing software, unifies the majority of practices already common in the field, and captures the metadata necessary for most common data processing operations.
- Health care data exchange: Fast Healthcare Interoperability Resources ([FHIR](https://www.hl7.org/fhir/index.html)) is a standard for communicating research findings; the intended scope of FHIR is broad, covering human and veterinary, clinical care, public health, clinical trials, administration and financial aspects. The standard is intended for global use and in a wide variety of architectures and scenarios.
- Social and behavioral science: Data Documentation Initiative ([DDI](https://ddialliance.org/)) is a standard used to describe survey data and observational data in social, behavioral, economic and health sciences – see below.

{{< /details >}}

{{< details "Learn More" >}}

### Templates

There are various tools and resources available that can be used to generate structured metadata, or to validate structured metadata records. The resources below can help you get started.

- The [Metadata Standards Catalog](https://rd-alliance.github.io/metadata-directory/tools/) maintains a list of tools for generating, editing, or validating metadata records
- The Consortium of European Social Science Data Archives (CESSDA) [“Documentation and metadata” training module](https://www.cessda.eu/Training/Training-Resources/Library/Data-Management-Expert-Guide/2.-Organise-Document/Documentation-and-metadata) includes links to a number of templates that can be used to describe resources in a standardized manner.
- [CEDAR](https://metadatacenter.org/) maintains a number of [Metadata Tools](https://more.metadatacenter.org/tools-training/cedar-metadata-tools) that can be used to annotate and describe data; although originally designed for biomedical data, CEDAR’s [Template Tools](https://more.metadatacenter.org/tools-training/cedar-template-tools) could be used to adapt templates for other disciplines
- GO FAIR [Metadata for Machines Workshops](https://www.go-fair.org/resources/go-fair-workshop-series/metadata-for-machines-workshops/)
- The [CodeMeta Generator](https://codemeta.github.io/codemeta-generator/) can be used to structure metadata that describes a software object in [JSON-LD notation](https://json-ld.org/). (See also the [User Guide](https://codemeta.github.io/user-guide/))

#### Crosswalks

A “crosswalk” is necessary when metadata created in one schema needs to be transformed to another schema, for example to facilitate sharing metadata between systems or to increase discoverability. For example, the crosswalk from [MARC to Dublin Core](https://www.loc.gov/marc/marc2dc.html) by the Library of Congress.

For a basic overview, see the ARDC 23 (Research Data) Things lesson on [metadata crosswalks](https://au-research.github.io/ARDC-23-things/researchdata/thing-13).

The following resources provide more information:

- **Ojsteršek. (2021). *Crosswalk of Most Used Metadata Schemes and Guidelines for Metadata Interoperability (1st ed.)* [Data set]. Zenodo. [https://doi.org/10.5281/zenodo.4420116](https://doi.org/10.5281/zenodo.4420116).**<br>
This resource provides crosswalks among the most commonly used metadata schemes and guidelines to describe digital objects in Open Science. This resource is also referenced by [FAIRsharing.org](https://fairsharing.org/collection/CrosswalkOfMostUsedMetadataSchemesAndGuidelines).

{{< /details >}}

{{< details "Go Deeper" >}}
An in-depth look at the Data Documentation Initiative:

The Data Documentation Initiative (DDI) has been working to establish “metadata standards and semantic products for describing social science data, data covering human activity, and other data based on observational methods.” DDI Lifecycle provides free standards that “document and manage different stages of the research data lifecycle, including conceptualization, collection, process, distribution, discovery, and archiving” of social, behavioral, economic, and health sciences. The standard includes metadata at the study- and file-level, for example:

### Study-level

- A researcher ID (e.g. [ORCID](https://orcid.org/)) is specified for each author specified
- Research organizations specified for author affiliations, [ROR](https://ror.org/) identifier added if possible
- Research funding is specified, [CrossRef Funder Registry](https://www.crossref.org/services/funder-registry/) Funder ID specified if possible. Grant ID is specified in standard format of funder (e.g. NIH funding IDs should include Activity code, Institute/Center, and Serial Number - see [NIH guide](https://era.nih.gov/erahelp/commons/#Commons/understandGrantNums.htm%3FTocPath%3D_____17))
- License is standard, linked, and machine-readable license describing allowable reuse (see License section in Thing 6 for more details)
- Study registrations are linked
  - Clinical Trials registrations include ClinicalTrials.gov Identifier
  - Study pre-registrations are linked with DOIs or links (e.g. OSF registries)
- Associated materials are linked using persistent identifiers or links
  - Associated publications or preprints are noted with full citations and DOIs
  - Protocols deposited in repositories include DOIs (e.g. Protocols.io)
  - Related datasets, code, other digital materials deposited in other repositories are linked with DOIs
  - Relationship type between these items and the compendium is noted in a standard, machine-readable way if possible (see e.g., [https://www.crossref.org/blog/doing-more-with-relationships-via-event-data/](https://www.crossref.org/blog/doing-more-with-relationships-via-event-data/))
- Title of compendium is meaningful, provides context to the work, and is not exactly the same as the title of an associated publication
- A publication date is listed for the compendium, revision dates are also listed

### File-level

- When possible, separate machinhttps://citation-file-format.github.io/e-readable and structured files are used to convey compendia metadata, such as
- Citation using [CITATION.cff](https://citation-file-format.github.io/) or BibTeX files ([CITATION.bib example](https://scipy.org/citing-scipy/))
- Environment variables captured in environment.yml
- License metadata can be done at least different 3 ways:
  - Captured as a standard text file ([LICENSE.txt example](https://github.com/scipy/scipy/blob/master/LICENSE.txt))
  - Recorded in metadata via a vocabulary (e.g., [SPDX terms](https://spdx.org/licenses))
  - Recorded in schema.org digest (as json) or markup in html
- Some mechanisms for capturing software/code metadata include:
  - [codemeta.json](https://codemeta.github.io/) file
  - [.zenodo.json](https://developers.zenodo.org/#deposit-metadata) (deposit metadata) file
  - [CITATION.cff](https://citation-file-format.github.io/) file

### Variable-level

- Variable-level DDI metadata define the variables and specify units of measurement and permitted values (including missing value codes); it is applied to quantitative data.
- This information is usually embedded within data files, e.g. as a header, or in column labels or generated from statistical package files.

The resources below offer a deeper look at metadata – what it is, how to use it, and some of the challenges.

- **Wilkinson, M., Dumontier, M., Aalbersberg, I. et al. (2016). The FAIR Guiding Principles for scientific data management and stewardship. *Scientific Data 3*, 160018. [https://doi.org/10.1038/sdata.2016.18](https://doi.org/10.1038/sdata.2016.18)**<br>
Machine-actionable metadata is information that enables the agent to have the capacity, “when faced with a digital object never encountered before, to: a) identify the type of object (with respect to both structure and intent), b) determine if it is useful within the context of the agent’s current task by interrogating metadata and/or data elements, c) determine if it is usable, with respect to license, consent, or other accessibility or use constraints, and d) take appropriate action, in much the same manner that a human would.”
- **CESSDA Training Team (2017 - 2020). *CESSDA Data Management Expert Guide*. Bergen, Norway: CESSDA ERIC. Retrieved from [https://www.cessda.eu/DMGuide](https://www.cessda.eu/DMGuide)**<br>
Start getting familiar with metadata with this guide from CESSDA.
- **Jedinger, Alexander. (2020). *What Is Metadata and How Do I Document My Data?* Presented at the CESSDA Training Days 2019 (CTD2019), Cologne, Germany: Zenodo. [http://doi.org/10.5281/zenodo.3923956](http://doi.org/10.5281/zenodo.3923956)**<br>
A video with Alexander Jedinger discussing metadata and data documentation.
- **Baca, Murtha, ed. (2016). *Introduction to Metadata (3rd ed.)*. Los Angeles: Getty Publications [http://www.getty.edu/publications/intrometadata](http://www.getty.edu/publications/intrometadata)**<br>
An overview of metadata, including its types, roles, and characteristics; a discussion of metadata as it relates to web resources; and a description of methods, tools, standards, and protocols for publishing and disseminating digital collections.
- **Alper, Brian S., Joshua E Richardson, Harold P Lehmann, Vignesh Subbian (2020). It is Time for Computable Evidence Synthesis: The COVID-19 Knowledge Accelerator initiative, *Journal of the American Medical Informatics Association, 27(8)*, 1338–1339, [https://doi.org/10.1093/jamia/ocaa114](https://doi.org/10.1093/jamia/ocaa114)**<br>
Efforts to establish universal standards for biomedical data exchange, including proposed metadata crosswalk.
- **Manninen, Lauren (2018) Describing Data: A Review of Metadata for Datasets in the Digital Commons Institutional Repository Platform: Problems and Recommendations, *Journal of Library Metadata, 18*(1), 1-11, [https://doi.org/10.1080/19386389.2018.1454379](https://doi.org/10.1080/19386389.2018.1454379)**<br>
A review of data hosted in Digital Commons repositories found that there is a need for a standardized language in describing research data within Digital Commons Institutional
Repositories.

{{< /details >}}
