---
title: "Thing 1:  Completeness"
description: "A research compendium contains all of the objects required to reproduce a predefined output."
draft: false
weight: 30
toc: true
---
**Related FAIR Principles: [R1](https://www.go-fair.org/fair-principles/r1-metadata-richly-described-plurality-accurate-relevant-attributes/), [R1.2](https://www.go-fair.org/fair-principles/r1-2-metadata-associated-detailed-provenance/), [R1.3](https://www.go-fair.org/fair-principles/r1-3-metadata-meet-domain-relevant-community-standards/)**

A research compendium contains all of the objects required to reproduce a predefined output.
When curation includes reproducing scientific claims or findings, you will need to check that all of the requisite objects and information are included in the research compendium. This often includes data, code, outputs, a codebook or data dictionary, and supporting documentation.

{{< alert theme="info" dir="ltr" >}}
Completeness ensures re-users of the research compendium are well-informed and have the context necessary to reproduce the results without needing to contact the original producer or track down missing components.
{{< /alert >}}<br>

{{< details "Get Started" >}}

When preparing a research compendium for reproducibility and curation, the goal should be to include all pertinent information, documentation, and files necessary to successfully run and recreate research output(s). Consider the following questions about each compendium component:

### Data

- If specific input data are necessary to reproduce a prespecified outcome, are the data included as a separate digital object?
- If not, has detailed information been provided on where and how to obtain the specific input data, or how to generate them?
- Are the data sensitive or restricted by the data producer? Is there enough information within the compendium to allow re-users to find and request access to these data?
- If input data are available from an external source, is there some promise of permanence? If there is a chance the data will change over time, will re-users be able to access or recreate the version of data used in this study?

### Code

- Are computing instructions included as digital objects in the research compendium?
- How are these computing instructions represented (e.g., personal scripts, bespoke manual steps, archived source code repository, a fully automated workflow available via open software libraries)?
- What environment, including hardware and software, does the computation rely on, and are all the packages specified?

### Output

- Does the compendium include an output as a separate digital object?
- What is the nature of the output in relation to the other objects in the compendium (i.e., is it a log from a statistical program, an executable paper, new data, new file, table, figure)?
Documentation
- Does the compendium include a codebook or data dictionary that defines the contents of the data file?
- Are variable definitions clear? Are units of measure included where appropriate?
- Does the compendium include a README file that outlines the contents of the compendium and the relationships among them?

### Container

- If the data or other objects are not in the container, are there precise instructions for accessing them during computation?
- Does the container require separate maintenance? Under what conditions will the container open?

{{< /details >}}

{{< details "Learn More" >}}

A research compendium should be able to stand on its own, with little interaction between a compendium producer and a re-user. Once deposited into a repository, the compendium should be accessible and reusable. More information on constructing a robust compendium can be found in [Thing 5: Documentation](../thing05) and [Thing 6: Access](../thing06).

Academics have been describing research compendiums and the necessary components that comprise a robust compendium for a few years now. Learn more about these recommendations below:

- **Sandve, G. K., Nekrutenko, A., Taylor, J., & Hovig, E. (2013). Ten simple rules for reproducible computational research. PLoS Computational Biology, 9(10), e1003285. https://doi.org/10.1371/journal.pcbi.1003285**<br>
The authors present a simple set of rules that can be used to make research more reproducible by enacting changes within your own research habits.
- **Berenson, K. R. (2017). Managing your research data and documentation. American Psychological Association. https://www.apa.org/pubs/books/4313048**<br>
In this book, Berenson outlines and describes how to construct a research compendium with reproducibility in mind.
- **Krafczyk, M. S., Shi, A., Bhaskar, A., Marinov, D., & Stodden, V. (2021). Learning from reproducing computational results: introducing three principles and the Reproduction Package. Philosophical Transactions of the Royal Society A: Mathematical, Physical and Engineering Sciences, 379(2197), 20200069. https://doi.org/10.1098/rsta.2020.0069**<br>

This article takes a slightly different approach of investigating the reproducibility of seven different articles. After performing their checks, the authors developed three principles for making research more reproducible based on the roadblocks they encountered in their own attempts at computation reproducibility.
{{< /details >}}

{{< details "Go Deeper" >}}
For examples of good compendiums, please see the following citations from various data repositories:

- **Ansolabehere, Stephen; Kuriwaki, Shiro, 2021, "Replication Data for: Congressional Representation: Accountability from the Constituent’s Perspective", https://doi.org/10.7910/DVN/QOVWMM Harvard Dataverse, V1, UNF:6:2J2iCVDbVbiImIApYE8mgw== [fileUNF]**
- **Berry, William; Fording, Richard; Hanson, Russell; Crofoot, Justin, 2021, "Replication Data for: The Validity of the Enns and Koch, and Berry et al. Measures of State Policy Mood: Continuing the Debate", https://doi.org/10.15139/S3/CQTBQU, UNC Dataverse, V1, UNF:6:iKVoC8ysGIWUdf5Gv/Cd9g== [fileUNF]**
- **Decarolis, Francesco, and Rovigatti, Gabriele. Data and Code for: From Mad Men to Maths Men: Concentration and Buyer Power in Online Advertising. Nashville, TN: American Economic Association [publisher], 2021. Ann Arbor, MI: Inter-university Consortium for Political and Social Research [distributor], 2021-09-29. https://doi.org/10.3886/E130502V1**

{{< /details >}}
