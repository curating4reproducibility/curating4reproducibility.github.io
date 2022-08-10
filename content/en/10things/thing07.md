---
title: "Thing 7: Provenance"
description: "The origin of the components of the research compendium and how each has changed over time is evident. "
draft: false
weight: 70
toc: true
menu:
  10things:
    parent: "10 Things"
---

**Related FAIR Guiding Principle: [R1.2](https://www.go-fair.org/fair-principles/r1-2-metadata-associated-detailed-provenance/)**

**[Related FAIR4RS Guiding Principle](https://doi.org/10.15497/RDA00068): R1.2**

Provenance is a fundamental archiving principle that refers to information about the origins, chain of custody, and ownership of an object, which helps to establish the object’s authenticity and authority. Provenance describes the lineage of data and other digital objects.

**In the context of research compendium components, knowledge about their sources, creation, and transformation over time is critical to assessing the quality, reliability, and trustworthiness of the compendium as well as the research outputs it serves to substantiate.**

The FAIR principles call for provenance to be captured as standardized machine-readable metadata. Provenance records a huge range of detail including the date the research object was created, the name of the creator, the tools and processes used to create the object, and any changes made to the object since its creation. An example of a formal standard for capturing provenance in a machine readable format is the WC3 PROV data model (see “Go deeper”).

Applies to **data, code, and computation**.

- For any transformation (including variable transformation), especially those done manually, e.g., when the full dataset cannot be made available due to the cost of collecting the data, privacy aspects of personal data, or intellectual property considerations, provenance should indicate how the subset was derived.
- If any external data sources are included or referenced, the creator, publisher, version and date accessed information should be documented. Where available, this includes a resolvable, globally unique permanent identifier such as a DOI. (e.g., [Data Citation Principles](https://doi.org/10.25490/a97f-egyk))
- A history of the modifications made to the code, ideally including attributed sources when code snippets are incorporated. Reference to dependencies that includes the actual version used, not a reference to the latest version. (e.g., [Software Citation Principles](https://doi.org/10.7717/peerj-cs.86), [Software Citation Guide](https://doi.org/10.12688/f1000research.26932.2)).
- Provenance of the research workflow that produced the outputs including scripts or representations in a formal workflow language such as the [Common Workflow Language](https://www.commonwl.org/user_guide/) or similar, and a history of changes to these.
- Workflow systems such as [Kepler](https://code.kepler-project.org/code/kepler/trunk/modules/provenance/docs/provenance.pdf), [Galaxy](https://docs.galaxyproject.org/en/master/api/api.html#module-galaxy.webapps.galaxy.api.provenance), [Taverna](http://www.taverna.org.uk/documentation/taverna-2-x/provenance/), [NextFlow](https://www.nextflow.io/blog/2019/easy-provenance-report.html) or [SnakeMake](https://snakemake.readthedocs.io/en/stable/snakefiles/reporting.html) can make it easier to capture provenance but require you to bring experiments or analysis into these systems prior to curation. “Code aware” data management/versioning systems such as [DataLad](https://www.datalad.org/) (or the many tools and platforms used in MLOps) are another option. Care needs to be taken in making a choice of system, that provenance records in a useful form can be
extracted for the target archive. See also [Thing 9: Automation](../thing09).

{{< details "Get Started" >}}
Formal, machine-readable capture of provenance can be quite daunting for a newcomer, and for manually curated materials, can be quite time consuming. To get started, focus less on formal capture, and more on what the relevant categories of provenance detail are in your context. Think about protocols or processes to ensure that this detail continues to be captured thereafter. This includes:

- What was the overall intent or purpose driving the compendium (or where this is captured)?
- What inputs were relevant when gathering data or writing code (funding, contributions, resources applied or consumed)?
- How were changes in files captured over time?
- Who contributed what to the outputs?
- Where did the relevant data come from, and (how) can others do the same data>
- What software tools and hardware were used in generating, preparing and analyzing the data?
- What scripts and workflows were generated?

Get started by sketching out these categories and more. You may not be able to access all of this information. In certain areas of research it may be necessary for you to capture precise detail about, for instance, where the data was gathered, or the conditions or constraints under which the project took place. You might like to explore the provenance records of a similar archive to the one you are targeting.

You may find that there are specific provenance requirements in order to be accepted to a certain archive. It is best to understand these requirements before data collection and analysis, as it can be impossible to uncover this detail once lost.

{{< /details >}}

{{< details "Learn More" >}}
A simple overview and suggestions for further reading is provided by the ARDC:

- **Australian Research Data Commons: Data Provenance. [https://ardc.edu.au/resources/working-with-data/data-provenance/](https://ardc.edu.au/resources/working-with-data/data-provenance/)**

Formal capture of data provenance is a major area of research, with [many published papers](https://www.sciencedirect.com/topics/computer-science/data-provenance). See, for instance:

- **Leipzig J., Nüst D., Hoyt C.T., Ram K., Greenberg J. (2021). The role of metadata in reproducible computational research. *Patterns 2*(9): 100322. [https://doi.org/10.1016/j.patter.2021.100322](https://doi.org/10.1016/j.patter.2021.100322)**<br>
Enabling reproducible research requires careful consideration of metadata. This resource unpacks metadata standards and steps for enabling reproducible in-silico experiments

{{< /details >}}

{{< details "Go Deeper" >}}
The [WC3 PROV data model (PROV-DM)](http://www.w3.org/2012/10/prov-dm) offers a conceptual overview of provenance information for research objects, or entities. In this model, all steps in the provenance of an object are broken down into relations between agents, entities and activities. Formal capture of this level of detail is best suited to systems that automate many or most aspects of transformations. If this describes you, then it may be worth going deeper with formal PROV representation of metadata.

Otherwise, if you have experience in capturing basic provenance detail, you may like to further consider:

- What provenance information is necessary vs nice to have?
- Is traceability more important than reproducibility?
- Should provenance be gathered only if the users ask for it?
- Is there a provenance system that orchestrates the data flow and keeps a log to describe it?
- Do you agree that provenance of sensitive data processing is itself sensitive?

There are many resources available for formal capture of provenance.

Read an article:

- **Goodman A, Pepe A, Blocker AW, Borgman CL, Cranmer K, Crosas M, et al. (2014) Ten simple rules for the care and feeding of scientific data. *PLoS Comput Biol 10*(4):e1003542. [https://doi.org/10.1371/journal.pcbi.1003542](https://doi.org/10.1371/journal.pcbi.1003542)**<br>
The higher the quality of provenance information, the higher the chance of enabling data reuse. If you want your work to be reproducible, “then provenance information is a must (e.g., working pipeline analysis code, a platform to run it on, and verifiable versions of the data).”

Consider provenance in automated data collection: Increasingly, tools for gathering data are assisting in elements such as question order variation in [computer assisted survey information collection](https://en.wikipedia.org/wiki/Computer-assisted_survey_information_collection) or spatio-temporal metadata capture associated with electronic field data collection. In addition to capturing the steps for an analysis, if you use tools such as this, it may be worth checking to see if you can extract provenance detail capturing those automated steps as well.
{{< /details >}}
