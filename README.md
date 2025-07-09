# CICICA Central American Course in Single-cell Cancer Analysis
## July 7-11 2025, Centro de Investigación en Cirugía y Cáncer (CICICA), Universidad de Costa Rica, San José, Costa Rica.
## Course Overview
This course offers a comprehensive introduction to the entire workflow of a single-cell RNA sequencing (scRNA-seq) experiment, with a particular focus on cancer research. Through theoretical modules and hands-on activities, participants will gain a deeper understanding of the principles, challenges, and advantages of single-cell technologies in biomedical research.

By performing each step of the scRNA-seq analysis pipeline—from raw data processing to biological interpretation—students will build practical skills and develop critical thinking around the design and application of single-cell studies. Emphasis is also placed on the use of publicly available datasets and databases as powerful resources to explore hypotheses and generate new insights in molecular cell biology and beyond.

## Bioinformatics Team
- [Benilton S. Carvalho](https://scholar.google.com/citations?user=44vQTS4AAAAJ&hl=en), Universidade Estadual de Campinas (UNICAMP), Brazil
- [Raúl Arias-Carrasco](https://scholar.google.com/citations?user=WRPcvtMAAAAJ&hl=en), Universidad Tecnológica Metropolitana, Chile
- [Ricardo Chinchilla-Monge](https://scholar.google.com/citations?user=BNQ9LNAAAAAJ&hl=es), Universidad de Costa Rica, Costa Rica
- [Vinicius Maracaja-Coutinho](https://scholar.google.com.br/citations?user=T_dpe84AAAAJ&hl), Advanced Center for Chronic Diseases (ACCDiS), University of Chile, Chile
- [Yesid Cuesta-Astroz](https://scholar.google.com/citations?hl=en&user=q0hiAjEAAAAJ), Universidad de Antioquía, Colombia

## Hands-On Bioinformatics Training Material

Below, you will find the links to slides  and Google Colab notebooks for the practical modules. 

### Practical Modules with Google Colab Notebooks:

- [Notebook 01 - Processing raw scRNA-seq data](https://colab.research.google.com/drive/1h0iurkpWVqQJki2JwinFEHrrieg7Wffj):
_Processing raw single-cell sequencing data (scRNA-seq) is a crucial step in the whole pipeline analysis of scRNA-Seq experiments. Depending on the library preparation method used, the RNA sequences will be acquired either from 3’ ends (or 5’ ends) of the transcripts (10X Genomics, CEL-seq2, Drop-seq, inDrops) or from full-length transcripts (Smart-seq). The choice of a specific method will depend entirely on the biological question and the downstream analysis to be implemented from a count matrix. In this notebook we will cover theoretical and practical steps in setting up from raw sequences (reads)to count matrix analysis pipelines, as well as explore the basic output of the Cell Ranger tool._
[**Lecture: Preprocessing**](https://github.com/viniciusmaracaja/HCA-LATAM_2023/blob/main/2023_10_23_HCA_LatinAmerica_preprocessing.pdf).

- [Notebook 02 - Quality Control, Exploratory Analysis, Data Normalization, and Clustering in scRNA-seq experiments](https://colab.research.google.com/drive/17IGUqvipvqForM5_o3eDUfhZfQc2_Cux?usp=sharing):
_In that part of the course, we will guide you through the initial steps of scRNA-seq data analysis, including data importing and organization, filtering, and preliminary visualization. These essential steps ensure quality and metadata information control over heterogeneous datasets before using the Seurat package and Bioconductor infrastructure. Once the data is imported, we will focus on assessing dataset quality through various metrics and visualizations, enabling the identification and removal of poor-quality cells. Furthermore, we'll delve into normalization techniques to address technical factors and clustering methods to group cells based on expression similarity, facilitating the interpretation of results and characterization of heterogeneity._
[**Lecture: Quality Control**](https://github.com/viniciusmaracaja/HCA-LATAM_2023/blob/main/2023_10_23_HCA_LatinAmerica_qualitycontrol.pdf).

- [Notebook 03 - Differential expression, cell type annotation and functional data analysis](https://colab.research.google.com/drive/17IGUqvipvqForM5_o3eDUfhZfQc2_Cux?usp=sharing):
_Identifying the set of features (genes/transcripts) that show distinct patterns of expression when comparing different conditions is an essential part of scRNA-seq analysis. This enables one to explore what processes might be involved in the differentiation between these circumstances. 
In this notebook, we will discuss mechanisms of analysis that combine differential expression, cell type annotation, and functional analyses to address this issue._
[**Lecture: Identifying Cell Subsets:**](2023_10_24_HCA_LatinAmerica_cell_subsets.pdf) and [**Lecture: Differential Expression And Biological Interpretation:**](2023_10_24_HCA_LatinAmerica_DE_And_BiologicalInterpretation.pdf).

- [Notebook 04 - Integrating single-cell transcriptomes from multiple samples](https://colab.research.google.com/drive/1NHO_B7ofyP4F3aklre_QyeGQcbqFohle?usp=sharing):
_With the increasing complexity of single-cell data, the integration of multiple datasets has become common. However, it is crucial to account for batch effects resulting from technical and biological variations to perform accurate analyses. These batch effects can stem from differences in sample handling, experimental protocols, sequencing platforms, as well as biological factors like the donor's genetic background and tissue origin. 
By employing computational methods to address these variations when comparing multiple samples, unwanted sources of variation can be eliminated, allowing researchers to focus on biologically meaningful signals. The process of removing batch effects involves making two important choices: selecting the appropriate method and parameterization, and determining the batch covariate. While the parameters are specific to the chosen method, the selection of the batch covariate depends on the goal of the integration task. This notebook will cover the key concepts and methods related to data integration and batch-effect correction, followed by hands-on activities that illustrate the integration of multiple datasets using methods from Seurat and Harmony._
[**Lecture: Batch Correction and Data Integration**](2023_10_24_HCA_LatinAmerica_batchcorrection.pdf).

### Authorship and Acknowledgments:
This comprehensive material has been a result of collaborative efforts since 2021 and has been successfully employed in numerous courses organized by esteemed institutions like the Human Cell Atlas, LatinCells initiative, and Wellcome Connecting Sciences. We extend our heartfelt gratitude to all the individuals listed below, who have actively contributed to the development and refinement of this material over the years. Their dedication and expertise have been instrumental in making this resource valuable for the bioinformatics community.

We appreciate the continuous support and feedback from participants, mentors, and institutions that have made this endeavor possible. Together, we strive to advance the understanding and application of single-cell genomics in Latin America and the Caribbean.

**List of Contributors - Listed Alphabetically:**
- Adolfo Rojas
- Benilton S. Carvalho
- Bruno Vinagre
- Carlos Alberto Oliveira de Biagi Júnior
- Cesar Prada
- Cristóvão Antunes
- Daniela Russo
- Erick Armingol
- Gabriela Guimarães
- Leandro Santos
- Joyce Karoline Silva
- Mariana Boroni
- Orr Ashenberg
- Patricia Severino
- Raúl Arias-Carrasco
- Ricardo Khouri
- Sebastián Urquiza-Zurich
- Sergio Triana
- Vinicius Maracaja-Coutinho
- Yesid Cuesta

## Citations and Reuse
We encourage the reuse and adaptation of the materials in this repository for teaching, research, or project development. The datasets and notebooks included here are designed to be modular and easily extendable to a variety of research questions. Many of the original notebooks used in this course, as well as additional workflows developed by our team over the years, are available in our main repository: [https://github.com/integrativebioinformatics/SingleCell-Notebooks](https://github.com/integrativebioinformatics/SingleCell-Notebooks). We invite you to explore, fork, and build upon these resources to advance your own work in single-cell analysis and beyond.

## License
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
