# CICICA Central American Course in Single-cell Cancer Analysis
## July 7-11 2025, Centro de Investigación en Cirugía y Cáncer (CICICA), Universidad de Costa Rica, San José, Costa Rica.
## Course Overview
This course offers a comprehensive introduction to the entire workflow of a single-cell RNA sequencing (scRNA-seq) experiment, with a particular focus on cancer research. Through theoretical modules and hands-on activities, participants will gain a deeper understanding of the principles, challenges, and advantages of single-cell technologies in biomedical research.

By performing each step of the scRNA-seq analysis pipeline, from raw data processing to biological interpretation, students will build practical skills and develop critical thinking around the design and application of single-cell studies. Emphasis is also placed on the use of publicly available datasets and databases as powerful resources to explore hypotheses and generate new insights in molecular cell biology and beyond.

## Bioinformatics Team
- [Benilton S. Carvalho](https://scholar.google.com/citations?user=44vQTS4AAAAJ&hl=en), Universidade Estadual de Campinas (UNICAMP), Brazil
- [Mariana Boroni](https://scholar.google.com.br/citations?user=oAEL6TAAAAAJ&hl=pt-BR), Instituto Nacional do Câncer, Brazil
- [Raúl Arias-Carrasco](https://scholar.google.com/citations?user=WRPcvtMAAAAJ&hl=en), Universidad Tecnológica Metropolitana, Chile
- [Ricardo Chinchilla-Monge](https://scholar.google.com/citations?user=BNQ9LNAAAAAJ&hl=es), Universidad de Costa Rica, Costa Rica
- [Vinicius Maracaja-Coutinho](https://scholar.google.com.br/citations?user=T_dpe84AAAAJ&hl), Advanced Center for Chronic Diseases (ACCDiS), University of Chile, Chile
- [Yesid Cuesta-Astroz](https://scholar.google.com/citations?hl=en&user=q0hiAjEAAAAJ), Universidad de Antioquía, Colombia

## Hands-On Bioinformatics Training Material

Below, you will find the links to slides  and Google Colab notebooks for the practical modules. 

### Module 01 - Introduction to Notebooks and processing raw scRNA-seq data:
_This module provides an introduction to Jupyter Notebooks and Google Colaboratory, exploring their features and structure, including code cells and text cells. Additionally, this notebook introduces essential command-line operations in Linux and R language, covering fundamental commands that are broadly applicable across programming languages with minimal adaptations. These foundational skills will support efficient data management and analysis in computational biology. Additionally, we will explore the key steps in processing raw sequencing reads into count matrices using Cell Ranger, discussing its main outputs and role in single-cell transcriptomics. Processing scRNA-seq data is a crucial step in single-cell analysis. The chosen library preparation method determines whether RNA sequences are captured from transcript ends (e.g., 10X Genomics, Drop-seq) or full-length transcripts (e.g., Smart-seq), directly influencing downstream analysis and biological insights._

- **Slides 01:** [A general overview on single cell data analysis and resources](https://docs.google.com/presentation/d/17ne2BEegrhlEmZlFSC_HcpiS8B___osI/edit?usp=drivesdk&ouid=101776043777005105119&rtpof=true&sd=true).
- **Slides 02:** [From processing raw sequences to count tables](https://docs.google.com/presentation/d/1OzVR9uag4LM4kL6M2B1z4KC8vIRGQXJH/edit?usp=drivesdk&ouid=101776043777005105119&rtpof=true&sd=true).
- **Notebook 01:** [Introduction to Notebooks and processing raw scRNA-seq data](https://colab.research.google.com/drive/121Mq5L0s58DqzBYCY29e-bTqTuanr739).
- **Notebook 02:** [Basic introduction to R](https://colab.research.google.com/drive/18YPsnmYStIoSmvEjVYhnWkb_KW9l1i76).


### Module 02 - Data structure in single-cell data analysis:
_In this Notebook, participants will explore the foundational aspects of how single-cell RNA sequencing (scRNA-seq) data is structured, stored, and accessed throughout an analysis pipeline. The session introduces the key data formats used in single-cell bioinformatics (e.g., MatrixMarket, HDF5, and AnnData/Seurat objects), with a focus on understanding how gene expression matrices, metadata, and dimensionality reduction results are organized._

- **Notebook 03:** [Data structure in single-cell data analysis](https://colab.research.google.com/drive/1mujj_pOciQCRfiAQHZYyFztbJ2TD0mvP).
  

### Module 03 - Quality control of scRNA-seq data:
_This notebook focuses on the key aspects of quality control (QC) in scRNA-seq data using the Seurat package. Participants will learn how to assess and interpret QC metrics critical for ensuring reliable downstream analysis. Topics covered include:  (a) Detection and filtering of low-quality cells based on features such as gene counts and total UMIs; (b) Evaluation of mitochondrial gene expression as a proxy for cell stress or damage; (c) Identification of potential doublets and multiplets; (d) Exploration of ambient RNA contamination and strategies to address it; (e) Preliminary visualizations (e.g., violin plots, scatter plots) to guide QC decisions. This module serves as a foundation for understanding the quality and integrity of single-cell data prior to any normalization, clustering, or advanced analysis. Proper QC is essential for minimizing technical artifacts and maximizing biological signal in scRNA-seq experiments._

- **Slides 03:** [Quality control in scRNA-seq](https://docs.google.com/presentation/d/16bkFOq6RWNSXvfdwJsP4P1Epe1hPMDLy/edit?usp=drivesdk&ouid=101776043777005105119&rtpof=true&sd=true).
- **Notebook 04:** [Quality control in scRNA-seq](https://colab.research.google.com/drive/1lzzksyJQEUOcwEJ5NoBnNqnr1RdLTOWW).


### Module 04 - From data normalization to cell-type annotation:
_In this section, we will use apply normalization techniques to mitigate technical variability, and implement clustering methods to group cells based on gene expression patterns. Furthermore, we will do differential expression analysis, cell type annotation, and functional enrichment techniques to uncover gene regulation mechanisms, identify key markers, and explore pathways involved in cellular differentiation and disease states. Together, these approaches provide a comprehensive framework for interpreting single-cell transcriptomics data and extracting meaningful biological insights._

- **Slides 04:** [Normalization and clustering of scRNA-seq data](https://benilton.github.io/wcs-rio/norm_clust.html).
- **Slides 05:** [Differential Expression and Annotation](https://benilton.github.io/wcs-rio/de_annot.html).
- **Statistics recommended book** [here](https://www.huber.embl.de/msmb/)
- **Notebook 05:** [From data normalization to cell-type annotation](https://colab.research.google.com/drive/1DW4svCcfd70AIJeW888LJC4g5ERcVNUG).


### Module 05 - Integrating single-cell transcriptomes from multiple samples:
_As single-cell data complexity grows, integrating multiple datasets has become standard. However, batch effects—arising from technical and biological variations—must be corrected for accurate analysis. These effects stem from differences in sample handling, protocols, sequencing platforms, and biological factors like donor background or tissue origin. Computational methods help eliminate unwanted variation, ensuring biologically meaningful signals. Batch correction requires two key decisions: selecting the appropriate method and its parameters, and defining the batch covariate based on the integration objective. In this notebook, we explore core concepts and methods for data integration and batch correction, with hands-on activities using Seurat and Harmony. Additionally, we perform benchmarking to compare integration strategies, helping select the most effective method while preserving biological relevance._

- **Slides 06:** [scRNA-seq data integration](https://docs.google.com/presentation/d/1ddQ7hdIWOztGC_UNT9qHhX-S-xDJQmf6/edit?usp=drivesdk&ouid=101776043777005105119&rtpof=true&sd=true).
- **Notebook 06:** [scRNA-seq data integration](https://colab.research.google.com/drive/1_V_jFYIgRkAYjDySD_jBYRsFM9nmaqBb).


## Module 06 - Exploring public scRNA-seq repositories:
_In this module we cover key public databases for single-cell data and other databases for gene expression, containing information for humans and other organisms. To enhance learning, we provide hands-on exercises for accessing, exploring, and analyzing these databases, allowing users to develop essential skills in biological data manipulation._

- **Notebook 07:** [Exploring public scRNA-seq repositories](https://colab.research.google.com/drive/1dMNwVvf15EomkxbZmL0zo4wqmX7_G9vW).


## Authorship and Acknowledgments:
This comprehensive material has been a result of collaborative efforts since 2021 and has been successfully employed in numerous courses organized by esteemed institutions like the Human Cell Atlas, LatinCells, and Wellcome Connecting Sciences. We extend our heartfelt gratitude to all the individuals listed below, who have actively contributed to the development and refinement of this material over the years. Their dedication and expertise have been instrumental in making this resource valuable for the bioinformatics community.

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
