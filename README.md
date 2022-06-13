---
title: "Bipolar Disorder & Lithium Response"
author: VNIEMS
date: June 03 2022
output: 
       github_document:
           toc: true
           toc_depth: 6
           number_sections: false
---

![](https://img.shields.io/badge/Release%20Date-June%202022-red?style=flat&logo=github&logoColor=red)

![](https://img.shields.io/badge/Release-v1.1.0-orange?style=flat&logo=github&logoColor=orange)

![](https://img.shields.io/badge/License-%20GPL--3.0--or--later-brightgreen?style=flat&logo=opensourceinitiative&logoColor=brightgreen)

```{r include=FALSE}
install.packages("rmarkdown",repos = "http://cran.us.r-project.org", dependencies = T, force =T)
library(rmarkdown)

install.packages("knitr",repos = "http://cran.us.r-project.org",dependencies = T, force=T)
library(knitr)

install.packages("crayon", repos = "http://cran.us.r-project.org", dependencies = T)
library(crayon)

options(knitr.table.format = "html") #set global option to get html table format!!!

knitr::is_html_output()
```

```{r include=FALSE}
remotes::install_github("haozhu233/kableExtra", dependencies = T, force =T)
library(kableExtra)
```

\|Banner\|

## About Our Project

Our project is presenting the analytic codes as part of the study, of which the manuscript, entitled "....", has been published in *Molecular Psychiatry*. [Ref or Doi will be added later]

The aim of the study in the manuscript is to identify the genetic contribution into lithium response in patients with bipolar disorder using multi-omics analysis of integrated between genome-wide association (GWAS) and RNA-sequencing (RNA-seq) data.

------------------------------------------------------------------------

## Table of Contents

-   [About Our Project](#envirius)

    -   [Idea](#idea)

    -   [Features](#features)

-   [Project Aim](#Project-Aim)

-   [The Project Workflow and File Descriptions](#The-Project-Workflow-and-File-Descriptions)

-   [Available plugins](#available-plugins)

    -   [Usage](#usage)

        -   [Check available plugins](#check-available-plugins)

        -   [Check available versions for each plugin](#check-available-versions-for-each-plugin)

        -   [Create an environment](#create-an-environment)

        -   [Activate/deactivate environment](#activatedeactivate-environment)

            -   [Activating in a new shell](#activating-in-a-new-shell)

            -   [Activating in the same shell](#activating-in-the-same-shell)

        -   [Get list of environments](#get-list-of-environments)

        -   [Get current activated environment](#get-current-activated-environment)

        -   [Do something in environment without enabling it](#do-something-in-environment-without-enabling-it)

        -   [Get help](#get-help)

        -   [Get help for a command](#get-help-for-a-command)

    -   [How to add a plugin?](#how-to-add-a-plugin)

        -   [Mandatory elements](#mandatory-elements)

------------------------------------------------------------------------
## Project Aim 

The purpose of this project is to distribute the codes that had been used in the multi-omics analysis of integrated between genome-wide association (GWAS) and RNA-sequencing (RNA-seq) data . The details of methods can be found in 1) the Method section in the main text and 2) the Supplemental Methods of the manuscript [Ref].

------------------------------------------------------------------------

## The Project Workflow and File Descriptions

This project includes 3 main subdirectories as follows:

#### I. Genome-wide association study (GWAS)

-   **GWAS analysis & imputation:** we did not provide the code. Here’s the summary:

    -   DNA from 1106 subjects was genotyped on the Illumina Psychip. Genotypes were called using the Ricopili pipeline (<https://sites.google.com/a/broadinstitute.org/ricopili/>).

    -   Data was screened for low call rate, low genotyping rate, and Hardy Weinberg equilibrium. Imputation was performed using IMPUTE2. Association was tested by linear regression as implemented in PLINK.

-   **A Versatile Gene-based Association Test (VEGAS):** [a web-based tool](https://vegas2.qimrberghofer.edu.au/) (Ref).

-   **GWAS boosting (GWAB) analysis:**

#### II. iPSC transcriptomic analyses

-   **Raw data of RNA-sequencing (RNA-seq)** -- stored in NCBI's Gene Expression Omnibus (Edgar et al., 2002) and are accessible through [**GEO Series accession number GSE205422**](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE205422).

-   **RNA-seq analysis:**

    -   Differential expression analysis

    -   Input files:

        -   Data #1: Phenotype data, kelsoe_metadata_111.csv

        -   Data #2: Gene expression data, all_genes_results_111s.txt

#### III. Network and functional enrichment analysis

-   **Network propagation analysis**

-   **Cluster analysis**

-   **KEGG pathway analysis**

-   **Pathview creation**

-   **Input files:**

    -   Data #3: DE_Genes_Li and CTRL_LRvsNR_for_Katie.xlsx

    -   Data #4: prioritized_genes_boosting_methods_5percent_190708.xlsx

| :Steps                                      | :File Description                 |
|--------------------------|----------------------------------------------|
| **I. Genome-wide association study (GWAS)** |                                   |
| GWAS analysis                               | Described somewhere else          |
| Gene-based analysis                         | Used VEGAS, a web-base tool (ref) |
|                                             |                                   |
| GWAS-boosting analysis                      | ???                               |
| **II. GWAS**                                |                                   |
| GWAS analysis                               | Described somewhere else          |
| Gene-based analysis                         | Used VEGAS, a web-base tool (ref) |
| GWAS-boosting analysis                      | ???                               |

------------------------------------------------------------------------

## Feature Guidance

| Features                     | ![](Downloads/Github%20test/R-Dark.svg){width="50"} | Reference |   Portals   |
|-----------------------|:---------------:|:---------------:|:---------------:|
| **Specs**                    |                                                     |           |             |
| Swagger 2.0                  |                          √                          |     √     |      √      |
| OpenAPI 3.0                  |                          √                          |     √     |      √      |
| OpenAPI 3.1                  |                      √ (basic)                      |     √     |      √      |
|                              |                                                     |           |             |
| **Theming**                  |                                                     |           |             |
| Fonts/colors                 |                          √                          |     √     |      √      |
| Extra theme options          |                                                     |     √     |      √      |
|                              |                                                     |           |             |
| **Performance**              |                                                     |           |             |
| Pagination                   |                                                     |     √     |      √      |
| Search (enhanced)            |                                                     |     √     |      √      |
| Search (server-side)         |                                                     |           |      √      |
|                              |                                                     |           |             |
| **Multiple APIs**            |                                                     |           |             |
| Multiple versions            |                                                     |     √     |      √      |
| Multiple APIs                |                                                     |           |      √      |
| API catalog                  |                                                     |           |      √      |
|                              |                                                     |           |             |
| **Additional features**      |                                                     |           |             |
| Try-it console               |                                                     |     √     |      √      |
| Automated code samples       |                                                     |     √     |      √      |
| Deep links                   |                                                     |     √     |      √      |
| More SEO control             |                                                     |           |      √      |
| Contextual docs              |                                                     |           |      √      |
| Landing pages                |                                                     |           |      √      |
| React hooks for more control |                                                     |           |      √      |
| Personalization              |                                                     |           |      √      |
| Analytics integrations       |                                                     |           |      √      |
| Feedback                     |                                                     |           | Coming Soon |

```{r}
colorize <- function(x, color) {
  if (knitr::is_latex_output()) {
    sprintf("\\textcolor{%s}{%s}", color, x)
  } else if (knitr::is_html_output()) {
    sprintf("<span style='color: %s;'>%s</span>", color,
      x)
  } else x
}
```

```{r echo=TRUE}
colorize ("some words in red", "red")
```

\<span style="color:red"\>cardinals\</span\> [cardinals]{style="color:red"}

![](Downloads/Github%20test/R-Dark.svg){width="50"}

![](Downloads/Github%20test/Python-Dark.svg){width="50"}

------------------------------------------------------------------------

## Contribution

Contributions for this project are:

-   **Code development team:**

    -   Katie Fisch, PhD
    -   Brin Sarah Rosenthal, PhD

-   **Executive manager and sponsor:**

    -   John Kelsoe, MD

-   **Administrator:**

    -   Vipavee Niemsiri, MD, PhD

------------------------------------------------------------------------

## License

**Copyright © 2022**

**The codes** in this project is *free* to be used and/or modify *under the terms of* **the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version**. Please see the policy and term of use <u>here</u>.

**All other files** as input files, for example, metadata files, are part of the study published in the manuscript entitled, “ …. ", which are *under* **a CC BY license (Creative Commons Attribution 4.0 International license)**.

------------------------------------------------------------------------

## Citation

If you use the code from this project, please cite with the Council of Science Editors (CSE) citation styles as an example below.

    CSE Bibliography Format:

    Niemsiri V. 2022. Bipolar Disorder and Lithium Response. San Francisco (CA): GitHub; [accessed 2022 Jun 6]. URL.

------------------------------------------------------------------------

## References


- [go to other github account](https://github.com/SommaiGH/master-readme) - external github account.
- [go to code file of this github account](https://github.com/OliveKmitl/oraganfood/blob/master/oraganfood/getFoodWhereIdShop.php) - internal code file

