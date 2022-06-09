---
title: "Thing 4: Transparency"
description: "The research compendium provides full disclosure of the research process that produced the scientific claim."
draft: false
weight: 40
enableToc: true
tocLevels: ["h2", "h3", "h4"]
---
**Related FAIR Principles: [I3](https://www.go-fair.org/fair-principles/i3-metadata-include-qualified-references-metadata/), [R1](https://www.go-fair.org/fair-principles/r1-metadata-richly-described-plurality-accurate-relevant-attributes/), [R1.2](https://www.go-fair.org/fair-principles/r1-2-metadata-associated-detailed-provenance/), [R1.3](https://www.go-fair.org/fair-principles/r1-3-metadata-meet-domain-relevant-community-standards/)**

**[Related FAIR4RS Principles](https://doi.org/10.15497/RDA00068): I2, R1, R1.2, R2, R3**

Transparency is a precondition of computational reproducibility. Ideally, the research compendium provides full disclosure of the research process that produced the scientific claim.

The inability to reproduce results is often caused by missing or insufficient information about the knowledge production process: where and how the data were obtained or generated, the analytical steps taken to produce results, the technical specifications of the requisite computing environment, the scripts used to process or manipulate the data, and any other information (often taking the form of tacit knowledge) needed to understand and re-execute the analysis. Despite lengthy methods sections in scholarly journal articles, many of these critical “backstage” details are either not included or not within easy reach. This problem of such opaque, or “black box,” research can undermine the integrity of the scientific record when no individual besides the original investigator is able to undertake the analysis process to verify the reported findings.

**Transparency requires that details about how the data were captured and transformed, and how they were analyzed to produce published results are included in the research compendium.**


{{< details "Get Started" >}}
Think about a re-user of the research compendium and the specific information they would need in order to re-execute the analysis to generate expected results. Consider the questions below for each key aspect of research transparency.

### Access transparency

Access transparency requires that re-users of the research compendium are provided specific information about the location of the materials, protocols for accessing them, and their origin (i.e., provenance).

- Are explicit instructions provided on where and how to request and access materials not included in the compendium? If they cannot be made publicly available due to licensing or sensitive data restrictions, is this detail included?
- For research that involves secondary analysis of extant data or uses existing code, are original sources cited with a persistent identifier or stable URL that resolves to the specific data files used in the analysis?

### Production transparency
Production transparency is evident when details about the study design and research methods (e.g., sampling frameworks, response rates, validity testing) are clearly articulated.

- Are key aspects of the research design and analytic methods disclosed to allow for understanding and evaluation of the research process? 
- Is information on how data were selected, captured, transformed, and analyzed provided in adequate detail to understand the choices made and steps taken by the researcher?

### Analytic Transparency

- Are the technical specifications of the computing environment, including operating system, software, and packages requirements (and their versions), provided?
- Is the process used to transform raw or original data into the analysis dataset made evident in the script files?
- Do script files contain non-executable comments that explain the purpose of codeblocks to enhance human readability of the analytical workflow?

{{< /details >}}

{{< details "Learn More" >}}
Many scholars have been advancing the cause of transparency by highlighting its positive impact on scientific rigor and integrity while also describing the adverse effects of research that fails to disclose the processes that underpinned the results. Read the articles below to further understand the impetus for increasing transparency as a means to promote research reproducibility.

- **Elman, C., Kapiszewski, D., & Lupia, A. (2018). Transparent social inquiry: Implications for social science. *Annual Review of Political Science, 21*, 29–47.
[https://doi.org/10.1146/annurev-polisci-091515-025429](https://doi.org/10.1146/annurev-polisci-091515-025429)**<br>
The authors of this article explain the value and practice of research transparency in terms of transparency’s three primary elements--data access, production transparency, and analytic transparency.
- **Stark, P. B. (2018). Before reproducibility must come preproducibility. *Nature,
557*(7707), 613–613. [https://doi.org/10.1038/d41586-018-05256-0](https://doi.org/10.1038/d41586-018-05256-0)**<br>
Philip Stark introduces the term “preproducibility” to describe the desired condition in which adequate information is provided to enable individuals to repeat an experiment or analysis.

Transparent research requires actionable strategies for exposing the knowledge-making processes that are often omitted from the published research article. Learn about some of these proposed strategies from the resources below.

- **Miguel, E., Camerer, C., Casey, K., Cohen, J., Esterling, K. M., Gerber, A., Glennerster, R., Green, D. P., Humphreys, M., Imbens, G., Laitin, D., Madon, T., Nelson, L., Nosek, B. A., Petersen, M., Sedlmayr, R., Simmons, J. P., Simonsohn, U., & Van der Laan, M. (2014). Promoting transparency in social science research. *Science, 343*(6166), 30–31. [https://doi.org/10.1126/science.1245317](https://doi.org/10.1126/science.1245317)**<br>
This article makes the case for transparency in social science research and describes three specific practices--disclosure, registration and analysis plans, and open data and materials--that can increase transparency in scientific reporting.
- **Nosek, B. A., Alter, G., Banks, G. C., Borsboom, D., Bowman, S. D., Breckler, S. J., Buck, S., Chambers, C. D., Chin, G., Christensen, G., Contestabile, M., Dafoe, A., Eich, E., Freese, J., Glennerster, R., Goroff, D., Green, D. P., Hesse, B., Humphreys, M., …
Yarkoni, T. (2015). Promoting an open research culture. *Science, 348*(6242), 1422–1425. [https://doi.org/10.1126/science.aab2374](https://doi.org/10.1126/science.aab2374)**<br>
This article introduces the Transparency and Openness Promotion (TOP) guidelines, which looks to scholarly journals to promote the principles of transparency, openness, and reproducibility by issuing policies that require authors to engage in transparent research
practices.
- **EQUATOR Network. (n.d.). Enhancing the QUAlity and Transparency Of health Research. [https://www.equator-network.org/](https://www.equator-network.org/)**<br>
The EQUATOR Network offers a searchable online database of almost 500 reporting guidelines for various types of research studies along with guidance on how to choose from among the guidelines.
-See also [Thing 5: Documentation](../thing05) to learn how transparency is made evident by producing tangible documentation that records essential details of the research workflow and [Thing 7: Provenance](../thing07) to understand the importance of tracking the origin, chain of custody, and ownership of research materials.

{{< /details >}}

{{< details "Go Deeper" >}}
These resources go into more depth about research transparency by presenting disciplinary case studies, tools, and initiatives that promote transparency and specific situations in which transparency was crucial for addressing scientific challenges.

- **Jacobs, A. M., Büthe, T., Arjona, A., Arriola, L. R., Bellin, E., Bennett, A., Björkman, L., Bleich, E., Elkins, Z., Fairfield, T., Gaikwad, N., Greitens, S. C., Hawkesworth, M., Herrera, V., Herrera, Y. M., Johnson, K. S., Karakoç, E., Koivu, K., Kreuzer, M., … Yashar, D. J. (2021). The Qualitative Transparency Deliberations: Insights and implications. *Perspectives on Politics, 19*(1), 171–208. [https://doi.org/10.1017/S1537592720001164](https://doi.org/10.1017/S1537592720001164)**<br>
While the focus has been on quantitative research, transparency standards do indeed apply for qualitative research. This article discusses how transparency is operationalized in qualitative research.
- **Kidwell, M. C., Lazarević, L. B., Baranski, E., Hardwicke, T. E., Piechowski, S., Falkenberg, L.-S., Kennett, C., Slowik, A., Sonnleitner, C., Hess-Holden, C., Errington, T. M., Fiedler, S., & Nosek, B. A. (2016). Badges to acknowledge open practices: A
simple, low-cost, effective method for increasing transparency. *PLOS Biology, 14*(5), e1002456. [https://doi.org/10.1371/journal.pbio.1002456](https://doi.org/10.1371/journal.pbio.1002456)**<br>
This article explains how applying badges to transparent research can incentivize scientists to make their research more transparent.
- **The Center for Effective Global Action. (2020, June 23). Why COVID-19 makes research transparency more important than ever. *Medium*. [https://medium.com/center-for-effective-global-action/why-covid-19-makes-research-transparency-more-important-than-ever-84071f3586be](https://medium.com/center-for-effective-global-action/why-covid-19-makes-research-transparency-more-important-than-ever-84071f3586be)**<br>
This article uses the COVID-19 pandemic as a case study for the importance of research transparency.
- **Carsey, T. M. (2014). Making DA-RT a reality. *PS: Political Science & Politics, 47*(01), 72–77. [https://doi.org/10.1017/S1049096513001753](https://doi.org/10.1017/S1049096513001753)**<br>
Read about how a group of political scientists advocated for research transparency in their discipline by developing the Data Access and Research Transparency (DA-RT) statement, which has been incorporated into the ethics guidelines of the American Political Science Association, and adopted by a large number of political science journals.

{{< /details >}}
