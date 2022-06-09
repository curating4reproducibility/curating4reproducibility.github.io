---
title: "Thing 5: Documentation"
description: "Information describing compendium objects is provided in enough detail to enable independent understanding and use of the compendium."
draft: false
weight: 50
enableToc: true
tocLevels: ["h2", "h3", "h4"]
---
**Related FAIR Principles: [F2](https://www.go-fair.org/fair-principles/fair-data-principles-explained/f2-data-described-rich-metadata/), [R1](https://www.go-fair.org/fair-principles/r1-metadata-richly-described-plurality-accurate-relevant-attributes/), [R1.2](https://www.go-fair.org/fair-principles/r1-2-metadata-associated-detailed-provenance/), [R1.3](https://www.go-fair.org/fair-principles/r1-3-metadata-meet-domain-relevant-community-standards/)**

**[Related FAIR4RS Principles](https://doi.org/10.15497/RDA00068): R1, R1.2, R3**

An important strategy for demonstrating research transparency is to create comprehensive
documentation that captures important details of the research process so that others are able to follow it to reproduce published research results. Failing to record essential information about the research compendium—descriptions of individual compendium files, technical requirements for using compendium files, the origin of materials used in secondary analyses, dataset variable and value code definitions, analytical steps for generating expected results—relegates the research process to a “black box,” making it difficult or even impossible to reproduce results.

**Robust documentation is the outcome of an intentional practice that keeps in mind the information needs of the compendium re-user so that the research compendium and the materials contained within it are *independently understandable for informed reuse*.**


{{< details "Get Started" >}}
Documentation can take on various forms. Common examples are README files, data availability statements, data dictionaries or codebooks, and code headers and non-executable comments. However the information about compendium components and the analysis workflow is presented, reproducibility relies on the presence of robust documentation that assumes no prior knowledge of the research process, thereby making the tacit more explicit.

### README file

When reviewing the contents of a research compendium, it should be clear the contents of each file, the purpose it serves, and citations to the original sources of extant materials. This information is often communicated in a README file that provides the following:

- The purpose of the compendium
- Citation to the associated research publication
- List of files with descriptions of each file
- Citations to original sources of materials used in secondary analyses
- Operating system and software requirements including version information
- Specific step-by-step instructions on how to install, execute, and/or implement components of the compendium to reproduce expected results
- Licensing information that establishes acceptable uses of the materials

### Data availability statement

Especially for data and other research artifacts that cannot be made publicly available, it is important to provide information on where and how to access the files in a data availability statement. This document should contain the following:

- Formal data citation that, if available, includes a persistent identifier (e.g., DOI) or other stable URL
- Instructions on where and how to access the materials (e.g. [Data Citation Principles](https://doi.org/10.25490/a97f-egyk), [Guidance on Data Citations](https://social-science-data-editors.github.io/guidance/addtl-data-citation-guidance.html))
- Any specific protocols required to access the materials (e.g., IRB approval, data use agreement)
- Duration of any embargo placed on the materials

### Codebook

A codebook, also referred to as a data dictionary, gives meaning to each variable and value that appears in a dataset. For every dataset in the compendium, a codebook should define each variable by providing:

- Variable names and human-readable variable labels
- Value codes and human-readable value labels for categorical and dichotomous variables
- Variable formats (e.g., string, numeric, date)
- Missing value codes
- Functions or expressions used to generate constructed or derived variables

### Code headers and comments

Besides the scripts that execute the analysis workflow, code files should also include header information that identifies the associated study and technical specifications for executing the code, as well as non-executable comments that explain the analysis process. Specifically, code files should contain the following:

- Citation to the associated research publication
- Primary author name and contact information
- Operating system, software, and package dependencies including version information (this may be generated using a software command such as `print sessionInfo` [in R](https://cran.r-project.org/web/packages/sessioninfo/index.html) or included in a requirements.txt file)
- Character encoding
- Date of most recent code update
- Date of most recent code execution
- Code license (See [embedded SPDX license](https://www.linuxfoundation.org/blog/solving-license-compliance-at-the-source-adding-spdx-license-ids/) terms)
- Non-executable, human-readable comments explaining the function of scripts and how they map to results presented in the publication

{{< /details >}}

{{< details "Learn More" >}}
The resources below offer additional guidance on documentation practices for reproducibility, including how-tos and exemplars.

- **DataONE. (n.d.). *Best practice: Describe*. Data Management Skillbuilding Hub. [https://dataoneorg.github.io/Education/bp_step/describe/](https://dataoneorg.github.io/Education/bp_step/describe/)**<br>
DataONE’s Data Management Skillbuilding Hub offers useful Best Practices Primers that focus on the research data lifecycle. This Best Practice: Describe primer outlines best practices to implement when creating comprehensive documentation for the research compendium.
- **Research Data Management Working Group. (n.d.). *README files*. Harvard Longwood Research Data Management. [https://datamanagement.hms.harvard.edu/collect/readme-files](https://datamanagement.hms.harvard.edu/collect/readme-files)**<br>
The Longwood Medical Area Research Data Management Working Group offers useful resources on various research data management topics. The README Files web page describes the purpose and contents of a README file with a template and example included.
- **Social Science Data Editors. (2021, December 15). *Guidance on data citations*. Social Science Data Editors. [https://social-science-data-editors.github.io/guidance/addtl-data-citation-guidance.html](https://social-science-data-editors.github.io/guidance/addtl-data-citation-guidance.html)**<br>
This guide covers all aspects of creating formal citations, which should be included in the compendium when using secondary materials to produce research results.
- **Data Citation Synthesis Group: Joint Declaration of Data Citation Principles. Martone M. (ed.). (2014). [https://doi.org/10.25490/a97f-egyk](https://doi.org/10.25490/a97f-egyk)**<br>
Outlines best practices and principles for creating data citations that ensure accessibility and accreditation of data as research products.
- **Vilhuber, L., Connolly, M., Koren, M., Llull, J., & Morrow, P. (2020). A template README for social science replication packages (v1.0.0). [https://doi.org/10.5281/zenodo.4319999](https://doi.org/10.5281/zenodo.4319999)**<br>
This guide for creating a README for social science replication packages outlines components for increasing reproducibility.
- **Cornell University Research Data Management Service Group. (n.d.). Guide to writing "README" style metadata. [https://data.research.cornell.edu/content/readme](https://data.research.cornell.edu/content/readme)**<br>
This resource offers guidance on writing a README file, including a list of recommended content, formatting standards, and a README document template. This targets data documentation, but can serve as a model for other types of documentation (e.g., code).
- **Hoces de la Guardia, F., & Sturdy, J. (2019). Code readability & dynamic documentation. In *Best practices for transparent, reproducible, and ethical research*. Inter-American Development Bank, Office of Strategic Development Effectiveness. [http://dx.doi.org/10.18235/0001564](http://dx.doi.org/10.18235/0001564)**<br>
The “Code Readability & Dynamic Documentation” section of this book describes best practices for documenting code and specific coding suggestions for enhancing understandability.
{{< /details >}}

{{< details "Go Deeper" >}}
There are several tools available to assist with creating documentation that is complete, accurate, and understandable. The resources below include software packages, tutorials, and other tools to go one step further toward research transparency and reproducibility.

- **Arslan, R. C. (2019). How to automatically document data with the codebook package to facilitate data reuse. *Advances in Methods and Practices in Psychological Science, 2*(2), 169–187. [https://doi.org/10.1177/2515245919838783](https://doi.org/10.1177/2515245919838783)**<br>
This article introduces the codebook R package that makes it easier to produce a codebook containing the essential information about the dataset.
- **Rule, A., Birmingham, A., Zuniga, C., Altintas, I., Huang, S.-C., Knight, R., Moshiri, N., Nguyen, M. H., Rosenthal, S. B., Pérez, F., & Rose, P. W. (2019). Ten simple rules for writing and sharing computational analyses in Jupyter Notebooks. *PLOS Computational Biology, 15*(7), e1007007. [https://doi.org/10.1371/journal.pcbi.1007007](https://doi.org/10.1371/journal.pcbi.1007007)**<br>
While computational notebooks have been praised for supporting research reproducibility, there are specific practices that should be implemented, which these authors outline as rules for using Jupyter notebooks.
- **Data Documentation Initiative (DDI) Alliance. (n.d.). *Create a codebook*. DDI. [https://ddialliance.org/training/getting-started-new-content/create-a-codebook](https://ddialliance.org/training/getting-started-new-content/create-a-codebook)**<br>
This webpage offers a list of tools for generating a codebook from standardized DDI metadata captured in various statistical software packages.

{{< /details >}}
