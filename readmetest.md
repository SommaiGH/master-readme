<h1 align="center">Bipolar Disorder and Lithium Response: Pharmacogenomic Study

![](https://img.shields.io/badge/Release%20Date-June%202022-red?style=flat&logo=github&logoColor=red)      ![](https://img.shields.io/badge/Release-v1.1.0-orange?style=flat&logo=github&logoColor=orange) ![](https://img.shields.io/badge/License-%20GPL--3.0--or--later-brightgreen?style=flat&logo=opensourceinitiative&logoColor=brightgreen)</h1>

### This is the README for the project of “Bipolar Disorder and Lithium Response: Pharmacogenomic  Study”.
### Note that this project is temporality under development, and coming soon.


## About Our Project
**The aim** of the project is to identify the genetic contribution into lithium response in patients with bipolar disorder (BD) using multi-omics analysis of integrated between genome-wide association (GWAS) and RNA-sequencing (RNA-seq) data.

Here, we make available the analytic toolsemployed as part of the main study, of which the manuscript, entitled ***"Focal adhesion is associated with lithium response in bipolar disorder: evidence from a network-based multi-omics analysis"***, has been published in *Molecular Psychiatry*. [doi will be added after a paper is published] 

-----------------------------------------------------------------------

## Table of Contents
-   [About our project](#About-Our-Project)   
-   [Project aim](#Project-Aim)
-   [The project workflow and file descriptions](#The-Project-Workflow-and-File-Descriptions)
    - [Step 1: Genome-wide association study (GWAS)](#Genome-wide-association-study)
    - [Step 2: iPSC transcriptomic analysis](#iPSC-transcriptomic-analysis)
    - [Step 3: Network and functional enrichment analysis](#Network-and-functional-enrichment-analysis)

-  [Feature guidance](#Feature-guidance)
-  [Contributing](#Contributing)
-  [License](#License)
-  [Citation](#Citation)
-  [References](#References)

------------------------------------------------------------------------
# Project Aim 

**The purpose** of the project is to distribute the tool (code development) that had been used in the multi-omics analysis of integrated data between BD GWAS and RNA-seq of patients-derived iPSC neurons.

The study workflow including detailed methods can be found in 1) the **‘Method’** section in the main text and 2) the **‘Supplemental Methods’** of the manuscript [doi will be added after a paper is published].

------------------------------------------------------------------------

## The Project Workflow and File Descriptions
This project includes **3 subdirectories** as shown below. Brief description is provided for each file, including additional/required data, which will be a useful resource for users.  
#### Step 1:
#### Genome-wide association study

-   **Genome-wide association study (GWAS) analysis & imputation:** we did not provide the code. Here’s the summary:
    -   DNA from 1106 subjects was genotyped on the Illumina PsychChip (https://sites.google.com/a/broadinstitute.org/psych-chip-resources/home).
    -   Genotype data was screened for low call rate, low genotyping rate, and Hardy-Weinberg equilibrium. Imputation was performed using IMPUTE2. Association was tested by linear regression as implemented in PLINK.

- **Gene-based analysis:** we used a Versatile Gene-based Association Test (VEGAS): a web-based tool, https://vegas2.qimrberghofer.edu.au/.

- **GWAS prioritizing analysis:** The GWAS results were reprioritized by using network information and the algorithms implemented in **genome-wide boosing analysis (GWAB)** and NetWAS methods.

#### Step 2:
#### iPSC transcriptomic analysis

-   **Raw data of RNA-sequencing (RNA-seq)** <img src="/img/dat.png"> stored in NCBI's Gene Expression Omnibus (Edgar et al., 2002) and are accessible through [**GEO Series accession number GSE205422**](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE205422).

-   **RNA-seq analysis:**

    -   Differential expression analysis: the functionsare used for RNA-seq differential expression analysis and downstream analysis.
    -   Input files:
        -   Data #1: Phenotype data, kelsoe_metadata_111.csv
        -   Data #2: Gene expression data, all_genes_results_111s.txt
        
#### Step 3:
#### Network and functional enrichment analysis

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

| Features                     |<img src="https://github.com/SommaiGH/master-readme/blob/main/img/R-GitHub.svg" width="50px">|<img src="https://github.com/SommaiGH/master-readme/blob/main/img/Python-GItHub.svg" width="50px">|Additional software required|
|------------------------------|:--------:|:--------:|:------------------------:|
| NetWas analysis              |          |     √    |                          |
| RNA-seq analysis             |    √     |          |                          |
| Network propagation analysis |          |     √    |          Cytoscape       |
| Cluster analysis             |          |          |                          |
| KEGG pathway analysis        |          |          |                          |
| Pathview creation            |          |     √    |                          |


------------------------------------------------------------------------

## Contributing

Contributions for this project are:

-   **Code development team:**
   
    - Kathleen M. Fisch, Ph.D.
    
    - Sara Brin Rosenthal, Ph.D.
    
-   **Executive manager and sponsor:**

    - John R. Kelsoe, M.D.
    
-   **Administrator:**
 
    - Vipavee Niemsiri, M.D., Ph.D.

------------------------------------------------------------------------

## License

> **Copyright © 2022**
> 
> **The code in this project** is *free* to be used and/or modify *under the terms of* **the GNU General Public License as published by the Free Software Foundation, > either version 3 of the License, or any later version**. Please see the policy and term of use <u>[here](https://github.com/SommaiGH/master-> readme/blob/main/license.md)</u>.
> 
> **Note that** All other files such as input data files, as part of the manuscript entitled, *“Focal adhesion is associated with lithium response in bipolar disorder: evidence from a network-based multi-omics analysis"* published in MolecularPsychiatry [doi will be added] are under **a CC BY 4.0 license (Creative Commons Attribution 4.0 International license)**.
 
------------------------------------------------------------------------

## Citation

If you use the code from this project, please cite with **the Council of Science Editors (CSE)** citation styles as an example below.

    CSE Bibliography Format:   
    
    Niemsiri V, Rosenthal SB, Fisch KM, and Kelsoe JR. 2022. Bipolar Disorder and Lithium Response. San Francisco (CA): GitHub; [accessed 2022 Jun 6]. URL.

------------------------------------------------------------------------

## References


*Will be provided.*

<p>
<details><summary>Cool Dropdown #1</summary><br/>
```js
// so wow, much amazing... you can even put code in these drop downs!
document.getElementById('root')
```s
[Or a link - like to google](https://google.com)
- Or a List
  - or a nested List
  - like this
  - with 😊 emojis
- Like this
Or even just normal text
</details>
<details><summary>Cool Dropdown #2</summary><br>
More cool text hiding in my dropdown
</details>
<details><summary>Cool Dropdown #3</summary><br>
Easter egg! :egg::egg::egg:
</details>
</p>
### `definitions.identifier`

- **type**: One of the following `object` types (click to expand/collapse):<br><br>
    1. <details>
          <summary>DOI</summary>
          <br>
          <ul>
            <li>
              <code>type</code>:
              <ul>
                <li><strong>type</strong>: <code>enum</code> with singular value <code>doi</code></li>
                <li><strong>required</strong>: <code>true</code></li>
                <li><strong>description</strong>: The type of identifier.</li>
              </ul>
            </li>
            <li>
              <code>value</code>:
              <ul>
                <li><strong>type</strong>: <a href="#definitionsdoi"><code>definitions.doi</code></a></li>
                <li><strong>required</strong>: <code>true</code></li>
                <li><strong>description</strong>: The value of the DOI, e.g. <code>10.5281/zenodo.1003149</code></li>
              </ul>
            </li>
            <li>
              <code>description</code>:
              <ul>
                <li><strong>type</strong>: <a href="#definitionsidentifier-description"><code>definitions.identifier-description</code></a></li>
                <li><strong>required</strong>: <code>false</code></li>
                <li><strong>description</strong>: The description of the DOI, e.g. <code>This is the DOI for version 0.11.4.</code></li>
              </ul>
            </li>
          </ul>
        </details>
    1. <details>
          <summary>URL</summary>
          <br>
          <ul>
            <li>
              <code>type</code>:
              <ul>
                <li><strong>type</strong>: <code>enum</code> with singular value <code>url</code></li>
                <li><strong>required</strong>: <code>true</code></li>
                <li><strong>description</strong>: The type of identifier.</li>
              </ul>
            </li>
            <li>
              <code>value</code>:
              <ul>
                <li><strong>type</strong>: <a href="#definitionsurl"><code>definitions.url</code></a></li>
                <li><strong>required</strong>: <code>true</code></li>
                <li><strong>description</strong>: The value of the URL, e.g. <code>https://github.com/citation-file-format/citation-file-format</code>.</li>
              </ul>
            </li>
            <li>
              <code>description</code>:
              <ul>
                <li><strong>type</strong>: <a href="#definitionsidentifier-description"><code>definitions.identifier-description</code></a></li>
                <li><strong>required</strong>: <code>false</code></li>
                <li><strong>description</strong>: The description of the URL, e.g. <code>The homepage for the project</code>.</li>
              </ul>
            </li>
          </ul>
        </details>
    1. <details>
          <summary>Software Heritage identifier</summary>
          <br>
          <ul>
            <li>
              <code>type</code>:
              <ul>
                <li><strong>type</strong>: <code>enum</code> with singular value <code>swh</code></li>
                <li><strong>required</strong>: <code>true</code></li>
                <li><strong>description</strong>: The type of identifier.</li>
              </ul>
            </li>
            <li>
              <code>value</code>:
              <ul>
                <li><strong>type</strong>: <a href="#definitionsswh-identifier"><code>definitions.swh-identifier</code></a></li>
                <li><strong>required</strong>: <code>true</code></li>
                <li><strong>description</strong>: The value of the Software Heritage identifier, e.g. <code>swh:1:dir:bc286860f423ea7ced246ba7458eef4b4541cf2d</code>.</li>
              </ul>
            </li>
            <li>
              <code>description</code>:
              <ul>
                <li><strong>type</strong>: <a href="#definitionsidentifier-description"><code>definitions.identifier-description</code></a></li>
                <li><strong>required</strong>: <code>false</code></li>
                <li><strong>description</strong>: The description of the Software Heritage identifier, e.g. <code>The directory object of the repository as stored on Software Heritage.</code>.</li>
              </ul>
            </li>
          </ul>
        </details>
    1. <details>
          <summary>Other</summary>
          <br>
          <ul>
            <li>
              <code>type</code>:
              <ul>
                <li><strong>type</strong>: <code>enum</code> with singular value <code>other</code></li>
                <li><strong>required</strong>: <code>true</code></li>
                <li><strong>description</strong>: The type of identifier.</li>
              </ul>
            </li>
            <li>
              <code>value</code>:
              <ul>
                <li><strong>type</strong>: Nonempty <code>string</code>.</li>
                <li><strong>required</strong>: <code>true</code></li>
                <li><strong>description</strong>: The value of the identifier, e.g. <code>arXiv:2103.06681</code>.</li>
              </ul>
            </li>
            <li>
              <code>description</code>:
              <ul>
                <li><strong>type</strong>: <a href="#definitionsidentifier-description"><code>definitions.identifier-description</code></a></li>
                <li><strong>required</strong>: <code>false</code></li>
                <li><strong>description</strong>: The description of the identifier, e.g. <code>The ArXiv preprint of the paper.</code>.</li>
              </ul>
            </li>
          </ul>
        </details>
- **required**: N/A
- **description**: An identifier.
- **usage**:<br><br>
    ```yaml
    identifiers:
      - type: doi
        value: 10.5281/zenodo.1003149
        description: The concept DOI of the work.
    ```
    ```yaml
    identifiers:
      - type: doi
        value: 10.5281/zenodo.4813122
        description: The versioned DOI for version 1.1.0 of the work.
    ```
    ```yaml
    identifiers:
      - type: doi
        value: 10.5281/zenodo.1003149
        description: The concept DOI of the work.
      - type: doi
        value: 10.5281/zenodo.4813122
        description: The versioned DOI for version 1.1.0 of the work.
    ```
    ```yaml
    identifiers:
      - type: doi
        value: 10.5281/zenodo.1003149
        description: The concept DOI of the work.
      - type: doi
        value: 10.5281/zenodo.4813122
        description: The versioned DOI for version 1.1.0 of the work.
      - type: swh
        value: "swh:1:dir:bc286860f423ea7ced246ba7458eef4b4541cf2d"
        description: The Software Heritage identifier for version 1.1.0 of the work.
      - type: url
        value: "https://github.com/citation-file-format/citation-file-format/releases/tag/1.1.0"
        description: The GitHub release URL of tag 1.1.0.
      - type: url
        value: "https://github.com/citation-file-format/citation-file-format/tree/16192bf05e99bcb35d5c3e085047807b5720fafc"
        description: The GitHub release URL of the commit tagged with 1.1.0.
    ```
    ```yaml
    preferred-citation:
      identifiers:
        - type: other
          value: "arXiv:2103.06681"
          description: The ArXiv preprint of the paper
    ```
