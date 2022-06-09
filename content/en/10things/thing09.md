---
title: "Thing 9: Automation"
description: "As much as possible, the computational workflow is script- or workflow-based so that the workflow can be re-executed using minimal actions."
draft: false
weight: 90
toc: true
---
**Related FAIR Principle: [Reusable](https://www.go-fair.org/fair-principles/r1-metadata-richly-described-plurality-accurate-relevant-attributes/)**

**[Related FAIR4RS Principle](https://doi.org/10.15497/RDA00068): Reusability**

**Automation refers to a process, for example, computation, transformation, or curation, that makes computational reproduction efficient and minimizes, if not eliminates, human intervention in reproducing research. Automation goes beyond documentation to avoid the need to manually set up processes (e.g., installing software, setting up the compute environment).**

There are many opportunities to automate aspects of the research process at various points during data handling and computation.

{{< details "Get Started" >}}
Automation means that information about the computational steps throughout the research process is script- or workflow-based, and manual processes are avoided to the fullest extent possible.

Including a good README file is a good first step: Instructions will always be needed.

>[Social Science Data Editors](https://social-science-data-editors.github.io/template_README/): “We note that a good replication package uses a minimal number of automated scripts, with no manual interventions required unless absolutely unavoidable.”

### Reasons for automation in research

The main steps in a project should be encoded in software and documented so they can be reliably reproduced.

- It’s better to use loops, functions or macros to automate any repetitive tasks for concise code (see [Reproducible Research Things: “Can you automate any repetitive tasks?”](https://guereslib.github.io/Reproducible-Research-Things/Step4Automation)).
- Avoids human error and undocumented idiosyncratic processes typical in manual workflows. Many disciplines use software-based or software-dependent means of data collection which help minimize human error. For example, in survey research, Computer-Assisted Telephone Interviewing (CATI) and Personal Interviewing (CAPI) are methods of coding information from telephone or personal interviews directly into a computer during the interview. CATI/CAPI software usually has built-in consistency checks, will not allow wild codes to be entered, and automatically prompts the interviewer for correct skip pattern questions ([ICPSR](https://www.icpsr.umich.edu/web/ICPSR/cms/2042)).
- Increases the likelihood that code will run on multiple machines, that necessary packages will be loaded, that data are pulled from the appropriate sources in the correct way. Automation helps with portability, that is, moving the execution of the same code with the same data to either a similar or different computing environment (see [TIER Protocol](https://www.projecttier.org/tier-protocol/protocol-4-0/#:~:text=). Portability: Any user should be able to run the scripts on their own computer or workspace) on the importance of portability).

{{< /details >}}

{{< details "Learn More" >}}

### Relative paths (versus absolute paths)

High quality code can help with automation. A key example is how input data are called.

When calling files, the absolute path starts from the root. In a typical computer, it would be the C drive: However, the relative path starts from the current working directory. Relative path calls files relative to their position from the current working directory. Using relative paths makes your reproducibility package portable and can be installed in any folder location. When you double-click on the program file to open the statistical software like SAS, STATA, and R, the location of the program file becomes the current working directory and you can leverage this behavior to simplify the process of reproducing your study.

### Workflows and pipelines

Script-based computation may cover data transformation, data analysis, figure and table generation, automated testing.

Consider dual workflows, “in which the data flow creates variables and datasets, while the analysis flow analyzes datasets, but does not construct variables or save datasets." (see [Scott Long](https://www.projecttier.org/fellowships-and-workshops/weekly-webcast-leaders-research-transparency/computing-workflow-reproducible-results/) remarks)

In addition to the data creation and data analysis workflows, the review and verification workflow should be automated as much as possible. See example of a curation tool, [YARD](http://doi.org/10.5334/dsj-2020-028).

### Computing environments

Rather than enabling scripts to run on different machines, constraining the execution environment to a specific operating system and specific dependencies may make it easier to ensure re-execution (see below for more). It may also be the truest representation of the compendium. An increasingly popular approach is to provide a build script for a container which fetches or contains all the relevant elements for reproduction. Doing so does not negate the need to properly document data and software, as the suitability of these approaches tend to change rapidly.

### Holding the computation environment as fixed: Platforms that make this easier

One way to aid automation is to hold the execution environment as fixed. Fixing the execution environment (hardware, operating system, software and dependencies) increases the likelihood that code that ran in the same environment will run again without issue in the future.

A common approach to making it easier to rerun code is to do the computation on a cloud based service or platform. Examples of this approach include [WHOLETALE](https://wholetale.org/), [Code Ocean](https://codeocean.com/), or [MyBinder](https://mybinder.org/). Many of these are services built on top of [JupyterHub](https://jupyter.org/hub) or [RStudio](https://www.rstudio.com/) which encapsulate the compute environment in a container. Integrations of similar functionality are also starting to become available within journals, notably the [reproducible article](https://elifesciences.org/labs/ad58f08d/introducing-elife-s-first-computationally-reproducible-article) from [eLife](https://elifesciences.org/), which brings the reproduction of results as close as possible to the published article. More complex solutions are explored below.
{{< /details >}}

{{< details "Go Deeper" >}}

### Fifteen (15) Code Review Things

This is a list of 15 code review-related tasks that help improve the quality and efficiency, automation of verification, reproducibility package preparation, and reuse.

1. File names of code are prefixed with the order of execution for easy identification of which code to run first and the next one.
2. Use a Master program file to call all programs used in the study (this is similar to the idea of “push button replication, see 3ie’s [push-button replication](https://www.3ieimpact.org/our-expertise/replication/push-button-replication) (PBR) project).
3. Note the software, packages, operating system used, and versions. And when the code was last executed.
4. Convert absolute file paths to relative file paths.
5. Check code for the presence of non-executable comments that document analysis processes.
6. Map code processes to paper sections using comments.
7. Remove or comment out unnecessary codes.
8. Label new variables and their values immediately after creation. These are needed should re-users need to rebuild their computing environment.
9. Run the code from start to finish in one go, using a different computer (not the one used to run the analysis). Rebuild the computing environment if necessary.
10. Address errors in the code. Repeat until no more errors are encountered.
11. Note the date the code was last executed from start to finish in the code.
12. Compare code output to findings presented in the article. The output should conform to a predetermined set of possible outputs (e.g., know what output you should expect from re-executing the workflow).
13. Verify that code generates output in the same order as they appear on the manuscript (if possible).
14. Insert a coding header to help researchers cite the article and code, contact the author, know the computing environment and software version used, and when the code was last updated or executed.
15. Create a Manuscript-Code-Output Checklist (Optional). It is a spreadsheet that lists the tables, figures, and in-text numbers found in your manuscript, specifies the program name and code line number that created them and verified that they were replicated.

### Automating aspects of code publishing

Github Actions with projects developed on GitHub can be used to automate validating or generating some types of metadata:

- Use [`howfairis`](https://github.com/marketplace/actions/fair-software) to automate assessing some FAIR aspects of the code components of your compendium
- Use [`cffconvert`](https://github.com/marketplace/actions/cffconvert) to validate a [citation file format (CFF)](https://citation-file-format.github.io/) file or use “CodeMeta2CFF” to convert a [CodeMeta](https://codemeta.github.io/) json file to CFF ([CFF support](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-citation-files) is also available within github)
- Use `pipreqs` to generate a requirements.txt via a [github action](https://github.com/marketplace/actions/automatic-requirements-txt-for-python-projects) (if working in python)

Consider running license compliance tests. These check that dependencies provide suitable licenses, and that the licenses between dependencies are compatible.

- The [OSS Review Toolkit (ORT)](https://github.com/oss-review-toolkit/ort) will work with projects written in several programming languages (see also the [experimental github action](https://github.com/marketplace/actions/run-ort))
- The [R Dependency License Report](https://github.com/marketplace/actions/r-dependency-license-report) is a github action that can be used with projects written in the R language

A small number of domain-agnostic research archives include integrations such that ingestion from a github repository (or some other git based code development platforms) can be automated. Project metadata must be provided within the repository using a valid format. For instance, see the [Zenodo](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content) and [Figshare](https://help.figshare.com/article/how-to-connect-figshare-with-your-github-account) integrations with GitHub.

- You can publish versions of your code using these integrations

### Holding the computation environment as fixed: Virtual Machines, Containers and other solutions

For desktop based workflows, the computation environment can be fixed in place using a number of solutions. This could be using a virtual machine, or especially common these days is to use containerisation. This allows for a ready made (or built) computation environment for code that assists with portability and re-execution. This can be done by carefully constructing images or build scripts to use [vagrant](https://www.vagrantup.com/), [docker](https://www.docker.com/) or [singularity](https://sylabs.io/), usually starting with an image or container that include all or most of the software required. The image or container might be a suitable target for archiving (being mindful of licensing restrictions), or the scripts and/or config files that describe how to build the image or container, fetch the appropriate code and data, and then combine them is potentially an approach that makes longer term preservation easier. There are also other tools that make it easier to use these technologies including [ReproZip](https://www.reprozip.org/).

There are also desktop based approaches that do fix the software and dependencies, but not the hardware or operating system. An example of this is [conda](https://conda.io/), or a level of abstraction above with repro-packs.

This “desktop based” approach isn’t necessarily bound to desktop use either, as many of the tools described above can also be deployed in the cloud in a scalable fashion.

See also the discussion of workflow or pipeline systems in [Thing 7](../thing07).

### Improving the technical infrastructure

In addition to scripts, the broader technical infrastructure can help with automation.

The technical infrastructure supporting the creation, publication, and distribution of computationally reproducible research artifacts has advanced greatly in recent years.

Automation requires that a well-developed technical infrastructure is trusted, and verified (See [Willis & Stodden, 2020](https://hdsr.mitpress.mit.edu/pub/f0obb31j/release/1?readingCollection=bf6d588c)).

{{< /details >}}
