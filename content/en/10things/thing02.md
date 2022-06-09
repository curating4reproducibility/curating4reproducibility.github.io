---
title: "Thing 2: Organization"
description: "It is easy to understand and keep track of the various objects in the research compendium and their relationship over time."
draft: false
weight: 40
toc: true
---
**Related FAIR Principles: [F2](https://www.go-fair.org/fair-principles/f2-data-described-rich-metadata/), [I3](https://www.go-fair.org/fair-principles/i3-metadata-include-qualified-references-metadata/), [R1.3](https://www.go-fair.org/fair-principles/r1-3-metadata-meet-domain-relevant-community-standards/)**

**[Related FAIR4RS Principles](https://doi.org/10.15497/RDA00068): F2, I2, R2, R3**

As research projects progress, they often evolve and things get more complicated and opaque over time; memory fails; project team members move on to new ventures. It is difficult to predict what may happen with a project down the line, so it is important to properly organize a compendium throughout the project itself.

**Organization is necessary to understand and to keep track of the various artifacts in the research compendium and the relationships among them over time.**


{{< details "Get Started" >}}
The organization of a research compendium depends on the types of files, their relationship to one another, as well as their interactions within the computational workflow. There is not a single, prescribed way for organizing research artifacts; however, these are some questions to consider as a project is being organized within a compendium:

- How are the objects organized within the research compendium?
- Can you identify what each object is?
- Can you determine the function of each object in relation to each other?
- Are names of files indicative of their content?
- How is the compendium packaged?
- Is the folder structure logical, and does it enhance understanding of the computational
workflow?
- Does the current structure permit streamlined reproducibility without errors?
- What if the objects cannot be organized in folders? What changes would you need to make
to your scripts to incorporate a step to download (and perhaps unzip) the files prior to
analysis and other steps?

{{< /details >}}

{{< details "Learn More" >}}
For more information on recommended organizational best practices and tips, please see the
following resources:

- **Tier protocol 4.0. TIER Protocol 4.0 | Project TIER | Teaching Integrity in Empirical
Research. (n.d.). Retrieved October 22, 2021, from [https://www.projecttier.org/tier-protocol/protocol-4-0/.](https://www.projecttier.org/tier-protocol/protocol-4-0/)**<br>
The TIER Protocol provides a guided hierarchy with descriptions and information on
structuring a research compendium for computational reproducibility and curation.
- **Open Science Framework (OSF). Best practices [File naming, Organizing files, Version
control]. [https://help.osf.io/hc/en-us/sections/360003624133-File-Management-and-Licensing](https://help.osf.io/hc/en-us/sections/360003624133-File-Management-and-Licensing)**<br>
The Open Science Framework offers many helpful tips and guides on best practices for
sharing data and research workflows.
- ***File management | Research Data Management Service Group*. (n.d.). Retrieved
December 14, 2021, from [https://data.research.cornell.edu/content/file-management](https://data.research.cornell.edu/content/file-management)**<br>
The Cornell Research Data Management Service Group has a robust resource for file
management recommendations and best practices.
- **Wilson G, Bryan J, Cranston K, Kitzes J, Nederbragt L, Teal TK. (2017). Good enough
practices in scientific computing. *PLoS Comput Biol 13*(6): e1005510.
[https://doi.org/10.1371/journal.pcbi.1005510](https://doi.org/10.1371/journal.pcbi.1005510)**<br>
Tips on project organization, including a project layout are described within this article.

Enabling reuse may mean separately handling the "objects" of the reproducible file bundle. This may be true when curating a bundle where the data is available elsewhere. If the data are archived separately from the code, then an additional step will likely need to be incorporated into the processing scripts to fetch the data. While adding extra labor, there are several benefits to this approach. This means that subsequent work can call upon the same data, rather than redepositing the same data with different code.

Explore how the links to data are captured in the landing page of the following datasets:

- **Irino, Tomohisa; Tada, Ryuji (2009): Chemical and mineral compositions of sediments
from ODP Site 127-797. *PANGAEA*, [https://doi.org/10.1594/PANGAEA.726855](https://doi.org/10.1594/PANGAEA.726855)**
- **Supplement to: Irino, T; Tada, R (2000): Quantification of aeolian dust (Kosa)
contribution to the Japan Sea sediments and its variation during the last 200 ky.
*Geochemical Journal, 34*(1), 59-93, [https://doi.org/10.2343/geochemj.34.59](https://doi.org/10.2343/geochemj.34.59)**

In some disciplines, journals require archiving the full compendium in specific archives, which may have certain requirements for organizing the research artifacts being deposited.

- **Willis, C., & Stodden, V. (2020). Trust but verify: How to leverage policies, workflows, and infrastructure to ensure computational reproducibility in publication. *Harvard Data Science Review, 2*(4). [https://doi.org/10.1162/99608f92.25982dcf](https://doi.org/10.1162/99608f92.25982dcf)**
- **Plutzer, E. (2019). Publication ethics, transparency, and replication: New policies at POQ. *Public Opinion Quarterly, 83*(2), 309-312. [https://doi.org/10.1093/poq/nfz028](https://doi.org/10.1093/poq/nfz028)**
- **Vilhuber, L. (2020). Reproducibility and replicability in economics. *Harvard Data
Science Review, 2*(4). [https://doi.org/10.1162/99608f92.4f6b9e67](https://doi.org/10.1162/99608f92.4f6b9e67)**

{{< /details >}}

{{< details "Go Deeper" >}}
A variety of tips, guidance, and online modules have been developed for further training on organization geared towards curation and reproducibility. Here are a few more resources to explore to go deeper:
 
- **University of Illinois at Urbana-Champaign Research Data Services. Data Nudges**<br>
[https://emails.illinois.edu/newsletter/158822.html](https://emails.illinois.edu/newsletter/158822.html)<br>
This Data Nudge recommends tips for file naming and outlines known issues with using
special characters in naming conventions. [Data Nudge #2,2017](https://emails.illinois.edu/newsletter/160474.html) highlights useful elements when crafting a file naming convention.
- **File Structure and Naming Prompt Sheet**<br>
[https://app.box.com/s/xiipln16t84y1ldwp5c7iefd395sypt4](https://app.box.com/s/xiipln16t84y1ldwp5c7iefd395sypt4)<br>
The File Structure and Naming Prompt Sheet is an adaptation of an MIT Libraries worksheet
to help researchers think through their naming conventions before adopting them for a
project.
- **Research Data MANTRA. Organising Data. (n.d.). Retrieved December 15, 2021, from
[https://mantra.ed.ac.uk/organisingdata/](https://mantra.ed.ac.uk/organisingdata/)**<br>
Part of the Research Data MANTRA online course, this section provides lessons on naming
and re-naming conventions, file and code versioning, as well as cloud collaboration tools.
The interactive course gives valuable examples and activities to further educate researchers and curators on data organization best practices.
- **RO-Crate (Research Object Crate)**<br>
[https://w3id.org/ro/crate](https://w3id.org/ro/crate)<br>
The intent of RO-Crate is to assist researchers in packaging their data, research objects, and workflows for curation.

{{< /details >}}
