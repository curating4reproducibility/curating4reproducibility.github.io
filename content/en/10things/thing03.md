---
title: "Thing 3: Economy"
description: "Fewer extraneous objects in the compendium mean fewer things that can break and require less maintenance over time."
draft: false
weight: 30
toc: true
---
**Related FAIR Principles: [R1](https://www.go-fair.org/fair-principles/r1-metadata-richly-described-plurality-accurate-relevant-attributes/)**

**[Related FAIR4RS Principles](https://doi.org/10.15497/RDA00068): R1**

When curating a reproducible file bundle, consider any extraneous parts that can be cut to make the overall bundle simpler to streamline computational reproduction.

**Economizing everything means fewer research objects can break while also requiring less care and maintenance over time.**

{{< details "Get Started" >}}
Simplifying and commenting out code are a couple of methods for tackling economization; however, the approach may vary depending on the type of software or methods being used for analysis. During file review and/or curation, here are some questions to consider:

- Can the scripts be simplified by removing redundancies or using loops and functions, for example?
- Are code blocks ordered logically according to the presentation of the results in the publication?
- Is there a master script that groups together all the other scripts? Are there additional scripts outside the master script and if so, are they necessary?
- Are the dependencies to the scripts or code all necessary?
- Are there comments in the code to help understand the computational workflow?
- Are there notebooks?
{{< /details >}}

{{< details "Learn More" >}}
More information on economization in the context of a research compendium can be found in [Thing 5: Documentation](../thing05) and [Thing 9: Automation](../thing09). The following resources contain relevant information as well:

- ***Literate programming*. (n.d.). Retrieved December 15, 2021, from [http://www.literateprogramming.com/](http://www.literateprogramming.com/)**<br>
A collection of best practices and guidance for programming, documentation, and code commenting.
- **Gillespie, C., & Lovelace, R. (n.d.). *Efficient R programming*. Retrieved December 15, 2021, from [https://csgillespie.github.io/efficientR/](https://csgillespie.github.io/efficientR/)**<br>
This book covers not only programmer efficiency, but also computational efficiency to write more effective and streamlined code using R.
- **Martin, R. C. (Ed.). (2009). *Clean code: A handbook of agile software craftsmanship*. Prentice Hall. [https://enos.itcollege.ee/~jpoial/oop/naited/Clean%20Code.pdf](https://enos.itcollege.ee/~jpoial/oop/naited/Clean%20Code.pdf)**<br>
A guide on writing clean and concise code covering topics such as good vs. bad commenting, slow code, and formatting.
- **Gentzkow, Matthew and Jesse M. Shapiro. (2014). *Code and data for the social sciences: A practitioner’s guide*. University of Chicago. [https://faculty.chicagobooth.edu/matthew.gentzkow/research/CodeAndData.pdf](https://faculty.chicagobooth.edu/matthew.gentzkow/research/CodeAndData.pdf), last updated January 2014.**<br>
Chapter 6, in particular, discusses the three rules of abstraction when writing code to eliminate redundancy and improve readability of the final product.
{{< /details >}}

{{< details "Go Deeper" >}}
As mentioned previously, the approach to economizing code is dependent upon many factors. Here are resources specific to a few disciplines that highlight some best practices:

- **Benureau, Fabien C.Y., and Rougier, Nicolas P. (2018). *Re-run, repeat, reproduce, reuse, replicate: Transforming code into scientific contributions. Frontiers in Neuroinformatics, 11*. [https://doi.org/10.3389/fninf.2017.00069](https://doi.org/10.3389/fninf.2017.00069).**
- **Palomino, Jenny, Wasser, Leah, and Joseph, Max. (2021). *Earth Lab. Earth Data Analytics*. Intro to Earth Data Science. Section 7 - Write Efficient and Clean Code Using Open Source Python. [https://www.earthdatascience.org/courses/intro-to-earth-data-science/write-efficient-python-code/](https://www.earthdatascience.org/courses/intro-to-earth-data-science/write-efficient-python-code/)**
- **Battig, W. F. (1962). Parsimony in psychology. *Psychological Reports, 11*(2), 555–572. [https://doi.org/10.2466/pr0.1962.11.2.555](https://doi.org/10.2466/pr0.1962.11.2.555)**

There are also tools available to assist with cleaning code. For example:

- **ROpenSci. (n.d.). *A tool for writing cleaner, more transparent code*. Retrieved December 15, 2021, from [https://docs.ropensci.org/Rclean/](https://docs.ropensci.org/Rclean/)**
{{< /details >}}
