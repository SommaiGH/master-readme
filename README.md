# Name of Project: Bipolar disorder and lithium response: pharmacogenomics response: pharmacogenomics
<img src="spec.png"> ![](https://img.shields.io/badge/Release%20Date-June%202022-red?style=flat&logo=github&logoColor=red)      ![](https://img.shields.io/badge/Release-v1.1.0-orange?style=flat&logo=github&logoColor=orange) ![](https://img.shields.io/badge/License-%20GPL--3.0--or--later-brightgreen?style=flat&logo=opensourceinitiative&logoColor=brightgreen)

This is the README for the project of “BipolarDisorder and Lithium Response:Pharmacogenomics”.

Note that this project is temporality under development, andcoming soon.

## About Our Project
**The aim** of the project is to identify the genetic contribution into lithium response in patients with bipolar disorder (BD) using multi-omics analysis of integrated between genome-wide association (GWAS) and RNA-sequencing (RNA-seq) data.

Here, we make available the analytic toolsemployed as part of the main study, of which the manuscript, entitled ***"Focal adhesion is associated with lithium response in bipolar disorder: evidence from a network-based multi-omics analysis", has been published in Molecular Psychiatry.*** [doi will be added after a paper is published] 


------------------------------------------------------------------------

## Table of Contents

-   [**About Our Project**](#envirius)   

-   [**Project Aim**](#Project-Aim)

-   [**The Project Workflow and File Descriptions**](#The-Project-Workflow-and-File-Descriptions)
    - [**Genome-wide association study (GWAS)**](#Genome-wide-association-study)
    - [**iPSC transcriptomic analysis**](#iPSC-transcriptomic-analysis)
    - [**Network and functional enrichment analysis**](#Network-and-functional-enrichment-analysis)

-  [**Feature guidance**](#Feature-guidance)
-  [**Contribution**](#Contribution)
-  [**License**](#License)
-  [**Citation**](#Citation)
-  [**References**](#References)

------------------------------------------------------------------------
## Project Aim 

**The purpose** of the project is to distribute the tool (code development) that had been used in the multi-omics analysis of integrated data between BD GWASand RNA-seq of patients-derived iPSC neurons.

The study workflow includingdetailed methods can be found in 1) the **‘Method’** section in the main text and 2) the **‘Supplemental Methods’** of the manuscript [doi will be added after a paper is published].

------------------------------------------------------------------------

## The Project Workflow and File Descriptions
This project includes **3 subdirectories** as shown below. Brief description is provided for each file, including additional/required data, which will be a useful resource for users.  

### Genome-wide association study

-   **Genome-wide association study (GWAS) analysis & imputation:** we did not provide the code. Here’s the summary:
    -   DNA from 1106 subjects was genotyped on the Illumina PsychChip (https://sites.google.com/a/broadinstitute.org/psych-chip-resources/home).
    -   Genotype data was screened for low call rate, low genotyping rate, and Hardy-Weinberg equilibrium. Imputation was performed using IMPUTE2. Association was tested by linear regression as implemented in PLINK.

- **Gene-based analysis**: we used a Versatile Gene-based Association Test (VEGAS): a web-based tool, https://vegas2.qimrberghofer.edu.au/.

- **GWAS boosting (GWAB) analysis**: The GWAS results were reprioritized by using network information and the algorithms implemented in GWAB and NetWAS methods.


### iPSC transcriptomic analysis

-   **Raw data of RNA-sequencing (RNA-seq)** <img src="dat.png"> stored in NCBI's Gene Expression Omnibus (Edgar et al., 2002) and are accessible through [**GEO Series accession number GSE205422**](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE205422).

-   **RNA-seq analysis:**

    -   Differential expression analysis
    -   Input files:
        -   Data #1: Phenotype data, kelsoe_metadata_111.csv
        -   Data #2: Gene expression data, all_genes_results_111s.txt
        

### Network and functional enrichment analysis

-   **Network propagation analysis**

-   **Cluster analysis**

-   **KEGG pathway analysis**

-   **Pathview creation**

-   **Input files:**
    -   Data #3: DE_Genes_Li and CTRL_LRvsNR_for_Katie.xlsx
    -   Data #4: prioritized_genes_boosting_methods_5percent_190708.xlsx


------------------------------------------------------------------------
## Feature Guidance
All source code shown here can be found in this GitHub project: 

| Features                     |<img src="R_logo.png">|<img src="Python_logo.png">|Add Software Required|
|------------------------------|:--------:|:--------:|:------------------------:|
| NetWas analysis              |          |     √    |                          |
| RNA-seq analysis             |    √     |          |                          |
| Network propagation analysis |          |     √    |          Cytoscape       |
| Cluster analysis             |          |          |                          |
| KEGG pathway analysis        |          |          |                          |
| Pathview creation            |          |     √    |                          |


------------------------------------------------------------------------

## Contribution

Contributions for this project are:

-   **Code development team:**
    - KathleenM. Fisch, Ph.D.
    - SaraBrinRosenthal, Ph.D.
-   **Executive manager and sponsor:**
    - John R. Kelsoe, M.D.
-   **Administrator:**
    - Vipavee Niemsiri, M.D., Ph.D.

------------------------------------------------------------------------

## License

**Copyright © 2022**

**The codein this project** is *free* to be used and/or modify *under the terms of* **the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or any later version.** Please see the policy and term of use <u>[here](https://github.com/SommaiGH/master-readme/blob/main/license.md) </u>.
 
------------------------------------------------------------------------

## Citation

If you use the code from this project, please cite with the Council of Science Editors (CSE) citation styles as an example below.

    CSE Bibliography Format:

    Niemsiri V. 2022. Bipolar Disorder and Lithium Response. San Francisco (CA): GitHub; [accessed 2022 Jun 6]. URL.

------------------------------------------------------------------------

## References


*Will be provided.*

<img src="https://github.com/SommaiGH/master-readme/blob/main/R-GitHub.svg" width="40px">

<img src="https://github.com/SommaiGH/master-readme/blob/main/Python-GItHub.svg" width="40px">

