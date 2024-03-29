---
title: "Thing 10: Review"
description: "A series of managed activities are needed to ensure continued access to and functionality of the research compendium and its components for as long as necessary."
draft: false
weight: 100
toc: true
menu:
  10things:
    parent: "10 Things"
---
**Related FAIR Principle: [Reusable](https://www.go-fair.org/fair-principles/r1-metadata-richly-described-plurality-accurate-relevant-attributes/)**

**[Related FAIR4RS Principle](https://doi.org/10.15497/RDA00068): Reusability**

Computational reproducibility is a particular type of Reuse. It refers to a user’s ability to execute computations in order to reproduce results reported in scholarly publications ([NASEM, 2019](https://www.nap.edu/read/25303)). A primary reason for curation in this context is to assess whether computational reproducibility can be achieved using the digital artifacts contained within the research compendium.

Curators helping prepare and review materials for archiving and publishing are often the “first reusers” of these materials.

**A review is a series of managed activities that helps ensure continued access to and functionality of the research compendium and its components for as long as necessary.**

{{< details "Get Started" >}}
Sharing of data and code is increasingly encouraged or mandated by various stakeholders in the scientific landscape. The [OECD](https://doi.org/10.1787/947717bc-en) in 2020 notes that data and code are often required to achieve reproducibility of scientific results, a key goal: “sharing access to the data underpinning scientific publications allows peers to test and reproduce scientific results. In practice, data alone are often insufficient to test reproducibility, and enhanced access to analysis software is also necessary.”

The 2021 [UNESCO Recommendation on Open Science](https://unesdoc.unesco.org/ark:/48223/pf0000379949.locale=en) states that, “scientific outputs related to publications (e.g. original scientific research results, research data, software, source code, source materials, workflows and protocols, digital representations of pictorial and graphical materials and scholarly multimedia material) that are openly licensed or dedicated to the public domain should be deposited in a suitable open repository, following appropriate technical standards that allow them to be properly linked to publications.”

This document also recommends changes to “peer review and other evaluation and verification methods” in order to achieve improved “quality, reproducibility and impact of science, and thereby the reliability of the evidence needed for robust decision making and policy and increased trust in science.”

### Reviewing code

When curating for reproducible research, the [Data Quality Review Framework](http://dx.doi.org/10.2218/ijdc.v9i1.317) can help organize review activities into four categories: Files, Documentation, Data, and Code. Many of the Things in this document address concepts and strategies that cover reviewing files, documentation, and data.

We focus here on “Code Review” as it is a newer practice, but one that is integral to the archival and publication of a computationally reproducible research compendium.

In general terms, code review includes an assessment of,

- The purpose of the code (e.g., recoding variables, manipulating or testing data, testing hypotheses, analysis), and
- Whether the code accomplishes this goal. In many cases, that means a verification that the code is executable and that reported findings are verified.

Code review can take place before the research compendium is published (“pre-publication review”) or after it is published (“post-publication review”).

The practice of code review can be implemented by professional staff in repositories and archives, academic institutions, scholarly associations and commercial publishers, and third-parties or by peers.

{{< /details >}}

{{< details "Learn More" >}}
Curators can identify problems with code files and remediate them before materials are archived and published. The resources below include examples of code-related irreproducibility, guidelines, tools, and services for managing the review and verification process, and information about badges.

### Examples of code-related irreproducibility

Challenges to reproducibility that involve code may include,

- Un- or non-executable code. The code cannot be compiled, or running the code returns errors.
- Error in variable operation. The code executes but the operation diverges from its description in the manuscript. For example, a manuscript defines obese as BMI >28, but the code
defines obese as BMI>= 28.
- Output discrepancy. The code executes but produces different results. For example, R code produces a result that is different from the result reported in the manuscript.
- Messy code. The code executes but requires high computing power.
- Hardcoded values. The code executes but values reported in the code are not generated by the code. The value may be generated by hand calculator or a different application (e.g.,
Excel) and results are entered into a program file. This can cause errors when data is further refined or if a mistake was made when calculating it.
- Outdated comments. The code executes but it has been evidently updated such that comments in the code no longer apply. For example, comments have typos or have not been updated.

### How to review code and address code-related irreproducibility

Curators, data and information professionals, researchers and others all can contribute to preventing and addressing these problems to ensure that re-users of the research compendium are able to reproduce the results without needing to contact the original producer or track down missing components. Re-users might be the original authors at a later point in time, curators, peer reviewers, and others.

**Guidelines.** Several organizations engaged with code review offer useful guidelines for how to curate materials for reproducibility. Guidelines tend to be domain-specific because the requirements are specific. Some examples of domain-specific guidelines include,

- The [CURE Consortium](https://curating4reproducibility.org/) (Curating for Reproducibility) provides materials
- Fifteen Code Review Things (see [Thing 9: Automation](../thing09))
- [Cornell Center for Social Sciences R2](https://socialsciences.cornell.edu/research-support/R-squared) provides Reproduction Materials Review Recommendations

**Tools.** There are also several tools for managing the review, verification, and curation process. For example, [Whole Tale](https://wholetale.org/index.html), [CODECHECK](https://codecheck.org.uk/guide/community-workflow), and [CASCaD](https://www.cascad.tech/) are options for general-purpose projects. See this conversation about solutions for reproducibility on the [Taking the Pulse blog](https://reproducibility.acm.org/2021/04/30/reproducibility-solutions-taking-the-pulse/).

Some examples of domain-specific tools include,

- Yale Application for Data Review ([YARD](http://doi.org/10.5334/dsj-2020-028))
- Social Science Reproduction Platform ([SSRP](https://www.bitss.org/introducing-the-social-science-reproduction-platform-a-resource-for-teaching-and-improving-computational-reproducibility/))

See the “Go deeper” section below for more resources about the practice of reproducibility checks.

## Who reviews code

Researchers, curators, publisher and repository staff, and others may review the code to verify reproducibility. For example, a number of [ACM](https://www.acm.org/publications/policies/artifact-review-and-badging-current) (the Association of Computing Machinery) conferences and journals have instituted formal processes for artifact review.

Third-party services are individuals or organizations not affiliated directly with the primary stakeholders in the research lifecycle (e.g., researchers, repositories, institutions, or publishers). Third-party services can be contracted to assist with the verification process.

Some examples of domain-specific services include,

- [Cornell Center for Social Science R2](https://socialsciences.cornell.edu/research-support/R-squared)
- [Odum Institute for Research in Social Science](https://odum.unc.edu/archive/)

Who reviews and how is a function of the goal of the review as well as the timing (i.e., pre- or post-publication).

**Researchers can do a lot to facilitate computational reproducibility of their own research.** Anticipating and preventing code-related irreproducibility early in the research life-cycle is prudent. Researchers can avoid potential problems and help ensure a research compendium is ready for archiving and publication by following these five review steps before submitting a manuscript for publication:

1. Review your code. Run your code from start to finish in one go. If possible, use a different computer with just the base package of the statistical software used in the analysis installed. Correct all errors encountered. Note the following in the README:
    1. Operating System used and its version
    2. CPUs and RAMs
    3. Statistical software package used and their version
    4. Packages/libraries/Ados used and their version<br>
Why? So you can verify that the code is error-free; detect and note the packages, libraries, and ado files required to run your analysis; and so that future re-users of your files have sufficient information to rebuild the computing environment used in the analysis, if necessary.
2. Review your manuscript. Verify that methods and operationalization of variables stipulated in the manuscript were correctly implemented in the code. For example, if obesity was defined as bmi >28 in the manuscript, then it should be coded as bmi >28 in the code, and not bmi >=28. Ensure the following are cited in your manuscript:
    1. Dataset used. Cite yourself if you created the dataset.
    2. Statistical software used
    3. Packages, libraries, and ado files used
3. Review the output produced by your code. Compare the results generated by your code to the findings presented in the manuscript. They should be identical up to the last decimal place. Verify you are pulling numbers from the correct table columns or cells.
4. Review your data. Make sure all original and computed variables are labeled. And prepare a Data Availability Statement for each dataset used in the study, which details the steps to acquire the data and its license.
5. Review your README. Make sure it has instructions on how to reproduce the study, contact information of the primary author, data and code citations and licenses, data availability statements, and information about the computing environment and packages, libraries, and ados used in the study.

Note: A useful, domain-specific, resource is offered by the [American Economic Association (AEA) Data Editor](https://aeadataeditor.github.io/aea-de-guidance/preparing-for-data-deposit.html). These are guidelines for authors on how to prepare a “replication package” for an AEA journal.

{{< /details >}}

{{< details "Go Deeper" >}}
Review is an integral aspect of the scientific process and an important aspect of reproducible research. Learn more about key topics related to review.

### FAIR principles and code review

Gold standard data review has been a province of data archives for a long time (e.g., Inter-university Consortium for Political and Social Research ([ICPSR](https://www.icpsr.umich.edu/web/pages/datamanagement/lifecycle/index.html)), [UK Data Archive](https://www.data-archive.ac.uk/managing-data/digital-curation-and-data-publishing/curation-process/)). Many of the curation practices common in such archives conforms to the FAIR principles for data.

Recently, new platforms have been created to review and assess data and metadata specifically for “FAIRNESS” (e.g., FAIR Metadata Assessment tool is in development by [DataONE](https://www.dataone.org/fair/); [FAIR Evaluator](https://fairsharing.github.io/FAIR-Evaluator-FrontEnd) developed by [FAIRsharing.org](https://fairsharing.org/); [F-UJI](https://www.f-uji.net/) developed by PANGAEA under the umbrella of the [FAIRsFAIR](https://www.fairsfair.eu/) project; [Australian Research Data Commons’](https://ardc.edu.au/resources/working-with-data/fair-data/fair-self-assessment-tool/) FAIR data self assessment tool).

Efforts have been made to apply FAIR to [research software](https://www.sciencedirect.com/science/article/pii/S2666389921000362).

### Journal policies and computational reproducibility

Perhaps inspired by the [Transparency and Openness Promotion (TOP) Guidelines](https://www.cos.io/initiatives/top-guidelines), scholarly journals have been implementing policies requiring authors to provide data and code and submitting these materials to various levels of scrutiny and review.

The [National Academies of Science, Engineering, and Medicine](https://www.nap.edu/catalog/25303/reproducibility-and-replicability-in-science) in the U.S. made the following recommendation in its report:

> RECOMMENDATION 6-4: Journals should consider ways to ensure computational reproducibility for publications that make claims based on computations, to the extent ethically and legally possible.

The NASEM report goes on to acknowledge that this can present some challenges:

> Although ensuring such reproducibility prior to publication presents technological and practical challenges for researchers and journals, new tools might make this goal more realistic. Journals should make every reasonable effort to use these tools, make clear and enforce their transparency requirements, and increase the reproducibility of their published articles.

Examples of journal policies that require data and code sharing and that include a code review:

#### General

- [Science Data and Code Deposition Policy](https://www.science.org/content/page/science-journals-editorial-policies#data-and-code-deposition)
- [Nature Reporting Standards and Availability of Data, Materials, Code and Protocols](https://www.nature.com/nature-portfolio/editorial-policies/reporting-standards)
- [PLOS Materials, Software, and Code Sharing](https://journals.plos.org/plosone/s/materials-software-and-code-sharing)

#### Political Science

- [Journal of Politics Data Replication Policy](https://www.journals.uchicago.edu/journals/jop/data-replication)
- [American Journal of Political Science (AJPS) Verification Policy](https://ajps.org/ajps-verification-policy/) (read the [Christian, et al., (2018)](https://doi.org/10.2218/ijdc.v13i1.555) article on the collaboration between AJPS and the Odum Institute Data Archive to develop a workflow that bridges manuscript publication and data review processes.)

#### Economics & Management

- [American Economic Association (AEA) Code and Data Availability Policy](https://www.aeaweb.org/journals/data/data-code-policy)
- [Royal Economic Society Replication Policy](https://www.res.org.uk/journals/the-econometrics-journal/submissions/replication-policy.html)
- [Management Science Policy for Data and Code Disclosure](https://pubsonline.informs.org/page/mnsc/datapolicy)

### Resources on the practice of reproducibility checks

- **Christian, T.-M. L., Lafferty-Hess, S., Jacoby, W. G., & Carsey, T. (2018). Operationalizing the replication standard. *International Journal of Digital Curation, 13*(1), 114–124. [https://doi.org/10.2218/ijdc.v13i1.555](https://doi.org/10.2218/ijdc.v13i1.555)**<br>
A case study of the collaboration between AJPS and the Odum Institute Data Archive to develop a workflow that bridges manuscript publication and data review processes.
- **Nüst D. and Eglen S.J. (2021). CODECHECK: An Open Science Initiative for the Independent Execution of Computations Underlying Research Articles During Peer Review to Improve Reproducibility [version 2; peer review: 2 approved]. *F1000Research*, 10:253. [https://doi.org/10.12688/f1000research.51738.2](https://doi.org/10.12688/f1000research.51738.2)**<br>
The CODECHECK system uses open infrastructure and tools and can be integrated into review and publication processes in multiple ways.
- **Peer, L., Green, A., and Stephenson, E. (2014). Committing to Data Quality Review. *International Journal of Digital Curation, 9*(1): 263–91 [https://doi.org/10.2218/ijdc.v9i1.317](https://doi.org/10.2218/ijdc.v9i1.317)**<br>
“We can think of a continuum of data curation that progresses from a basic level where data are accepted ‘as is’ for the purpose of storage and discovery, to a higher level of curation which includes processing for preservation, improved usability, and compliance, to an even higher level of curation which also undertakes the verification of published results.”
- **Peer, L. and Dull, J. (2020). YARD: A Tool for Curating Research Outputs. *Data Science Journal, 19*(1), 28. [http://doi.org/10.5334/dsj-2020-028](http://doi.org/10.5334/dsj-2020-028)**<br>
YARD (Yale Application for Research Data) is an adaptable curation workflow tool that enhances research outputs and associated digital artifacts designated for archival and reuse.
YARD helps create high quality data packages that are FAIR, transparent, and reproducible.
- **Peng, R.D. (2011). Reproducible Research in Computational Science. *Science, 334*(6060), 1226-1227. [https://doi.org/10.1126/science.1213847](https://doi.org/10.1126/science.1213847)**<br>
Argues that articles that have passed the reproducibility review “convey the idea that a knowledgeable individual has reviewed the code and data and was capable of producing the results claimed by the author. In cases in which questionable results are obtained, reproducibility is critical to tracking down the ‘bugs’ of computational science.”

### Reproducibility badges

Badges are considered “simple, effective signals to promote open practices and improve preservation of data and materials by using independent repositories.

- The Association for Computing Machinery ([ACM](https://www.acm.org/publications/policies/artifact-review-badging)) lists several badges for reproducibility reviews.
- The Center for Open Science ([COS](https://www.cos.io/initiatives/badges)) badges acknowledge open science practices (sharing data, materials, or pre-registration).

For more information on badges, see:

- **Hardwicke, T.E., et al. (2021). Analytic Reproducibility in Articles Receiving Open Data Badges at the Journal Psychological Science: An Observational Study. *Royal Society
Open Science, 8*: 201494. [https://doi.org/10.1098/rsos.201494](https://doi.org/10.1098/rsos.201494)**<br>
Evaluated analytic reproducibility in 25 Psychological Science articles awarded open data badges between 2014 and 2015. 16 articles (64%) contained at least one major numerical discrepancy, requiring additional input from original authors.
- **Kidwell, M.C., et al. (2016). Badges to Acknowledge Open Practices: A Simple, Low-Cost, Effective Method for Increasing Transparency. *PLoS Biology 14*(5):e1002456. [https://doi.org/10.1371/journal.pbio.1002456](https://doi.org/10.1371/journal.pbio.1002456)**<br>
Found that when badges were earned, reportedly available data were more likely to be actually available, correct, usable, and complete than when badges were not earned. Badges are simple, effective signals to promote open practices and improve preservation of data and materials by using independent repositories.

### Active maintenance

Confirming computational reproducibility at a single point in time is not a guarantee of long term reproducibility. While some aspects of curation are more or less “one and done” (e.g., assigning a persistent ID to a file, documenting a dataset), others call for repeated assessment. As a curator, you will need to perform periodic reviews, or ***maintenance***, ideally in a scheduled and automated way, and remediate if need be.

The idea that digital curation is an ongoing activity, a “series of managed activities necessary to ensure continued access to digital materials for as long as necessary” is central to [digital preservation](https://www.dpconline.org/docs/digital-preservation-handbook/299-digital-preservation-handbook/file). It is reinforced in the foundational text that defines the FAIR principles: “Beyond proper collection, annotation, and archival, data stewardship includes the notion of ‘long-term care’ of valuable digital assets, with the goal that they should be discovered and re-used for downstream investigations, either alone, or in combination with newly generated data” ([Wilkinson et al., 2016](https://doi.org/10.1038/sdata.2016.18); Italics added).

Maintenance highlights the time dimension of curation. Consider this: It is common practice for an archive concerned about the authenticity and integrity of its digital content to make use of checksums at the time of deposit, and in subsequent periodic reviews (see, for example, [ICPSR Digital Preservation Policy Framework](https://www.icpsr.umich.edu/web/pages/datamanagement/preservation/policies/dpp-framework.html)). Similarly, concern about computational reproducibility calls for not only curation of the research compendium (that includes all the other Things in this document) at one point in time, often indicated with a badge (see, for example, the [ACM’s Artifact Review and Badging](https://www.acm.org/publications/policies/artifact-review-badging)), but a periodic review.

When planning to publish or archive a research compendium you will want to think about what might require periodic review. What might you worry about breaking down over time?

Specifically, consider the effect of the following scenarios on computational reproducibility:

- Digital files may get corrupted, inaccessible, or unavailable.
- Permissions to access data may change.
- Computer programs, scripts, or code may become unavailable or may not compile or execute.
- Computing environments and parameters may change.

The following resources may be useful in considering the above scenarios:

#### On the rationale for maintenance:

- **Wilkinson, M., Dumontier, M., Aalbersberg, I. et al. (2016). The FAIR Guiding Principles for Scientific Data Management and Stewardship. *Scientific Data 3*, 160018. [https://doi.org/10.1038/sdata.2016.18](https://doi.org/10.1038/sdata.2016.18)**<br>
The position that long-term care of digital materials is a continuous activity is articulated in the Wilkinson et al 2016 article that originally introduced the FAIR principles: “Beyond proper collection, annotation, and archival, data stewardship includes the notion of ‘long-term care’ of valuable digital assets, with the goal that they should be discovered and re-used for downstream investigations, either alone, or in combination with newly generated data” (Italics added).
- **UNESCO. (2020, March 2). *UNESCO Recommendation on Open Science*. [https://en.unesco.org/science-sustainable-future/open-science/recommendation](https://en.unesco.org/science-sustainable-future/open-science/recommendation)**<br>
The report states that, “Open research data… [should be made] available in a timely and user-friendly, human- and machine-readable and actionable format, in accordance with principles of good data governance and stewardship, notably the FAIR (Findable, Accessible, Interoperable, and Reusable) principles, supported by regular curation and maintenance” (Italics added).
- **Spinellis, D., Louridas, P., & Kechagia, M. (2021). Software Evolution: The Lifetime of Fine-Grained Elements. PeerJ. *Computer Science, 7*, e372. [https://doi.org/10.7717/peerj-cs.372](https://doi.org/10.7717/peerj-cs.372)**<br>
A challenge for ensuring long term computational reproducibility is rooted in the fact that it relies on code and software. When it comes to code, the time horizon for “regular curation and maintenance” is not clear. The lifespan of code is, by this estimation, less than two and a half years.
- **Peer, L., Orr, L., & Coppock, A. (2021). Active Maintenance: A Proposal for the Long-Term Computational Reproducibility of Scientific Results. *PS: Political Science & Politics, 54*(3), 462-466. [https://doi.org/10.1017/S1049096521000366](https://doi.org/10.1017/S1049096521000366)**<br>
Proposing that researchers dedicated to computational reproducibility should have a plan in place for “active maintenance” of their analysis code, and offering concrete suggestions for how data archives, journals, and research communities could encourage and reward the active maintenance of scientific code and data.

#### On strategies for maintenance:

- **Perkel, J. (2020). Challenge to Scientists: Does Your Ten-Year-Old Code Still Run? *Nature 584*, 656-658. [https://doi.org/10.1038/d41586-020-02462-7](https://doi.org/10.1038/d41586-020-02462-7)**<br>
As a dynamic digital object, code “will eventually decay, and you will have to repair it, and you’ll have to replace it,” as Carole Goble points out.
- **Akhlaghi, M., Infante-Sainz, R., Roukema, B. F., Khellat, M., Valls-Gabaud, D., & Baena-Gallé, R. (2021). Toward Long-Term and Archivable Reproducibility. *Computing in Science Engineering, 23*(3), 82–91. [https://doi.org/10.1109/MCSE.2021.3072860](https://doi.org/10.1109/MCSE.2021.3072860)**<br>
Introducing “Maneage” (managing data lineage), which enables cheap archiving, provenance extraction, and peer verification that has been tested in several research publications. The article includes 8 criteria for longevity (i.e., “the length of time that a project remains functional after its creation”). Includes review of the longevity of commonly used tools (e.g., Docker, Jupyter).
- **National Digital Stewardship Alliance (2019). *The Levels of Digital Preservation V2.0 Matrix*. [https://ndsa.org/publications/levels-of-digital-preservation/](https://ndsa.org/publications/levels-of-digital-preservation/)**<br>
A framework for thinking about the specific actions that curating for reproducible and FAIR research entails. The Framework specifies the actions necessary to ensure that digital content is known, protected, monitored, and sustained.

{{< /details >}}
