# 2025 DSC Nanopore Sequencing Workshop Materials

## Scripts
This folder contains R and shell scripts we used during the workshop.  
 
- **install_bioinfo_tools.sh** - Shell script to install bioinformatics tools on a Google Cloud Vertex AI instance. 

- **as_processing_cloud_v2.sh** - Shell script for processing and analyzing nanopore adaptive sampling data. It splits reads by treatment, maps them to a reference, and generates summaries.  

- **get_all_stats.sh** - Shell script to collect SeqKit stats for various FASTQ outputs from the adaptive sampling analysis pipeline, including: the number of sequences, total yield, minimum, average, and maximum sequence lengths, N50, and the average quality score of all bases.  

- **violinplot_treatments_isolates.R** - R script that generates a series of violin plots to visualize sequencing data. It compares the distributions of read length and quality between two different treatments, both for the overall dataset and for reads mapped to specific isolates.  

- **plot_treatments_isolates.R** - R script that creates bar plots to compare overall sequencing metrics like read count and quality between the sequences derived from the control and adaptive sampling portion of the flow cells. It also visualizes how the proportion of reads mapped to different isolates varies between these two treatments.


## Handouts
This folder contains descriptions of the microbial mock communities and library preparation/sequencing protocols used.  

### Mock Communities
- **d6306_zymobiomics_microbial_community_dna_standard.pdf**  
DNA community standard used for the ligation sequencing project (Sequencing protocols 1-3). Contains eight bacteria (three Gram-negative and five Gram-positive) and two yeasts.  

- **d6322_zymobiomics_hmw_dna_standard.pdf**  
DNA community standard used for the rapid sequencing and rapid barcode sequencing  projects. Contains seven bacteria (3 gram-negative and 4 gram-positive) and 1 yeast.

### Protocols  
- **genomic-dna-by-ligation-sqk-lsk114-document-checklist-GridION-en-GDE_9161_v114_revZ_08May2025-60.pdf**  
Full ligation library preparation checklist for beginners.  

- **genomic-dna-by-ligation-sqk-lsk114-document-document-GridION-en-GDE_9161_v114_revZ_08May2025-60.pdf**  
Full library preparation and sequencing protocol for sequencing of a DNA sample using the Ligation Sequencing Kit V14 (SQK-LSK114).  

- **genomic-dna-by-ligation-sqk-lsk114-document-reference-GridION-en-GDE_9161_v114_revZ_08May2025-60.pdf**  
Shortened ligation library preparation protocol for experienced users.  

- **rapid-sequencing-gdna-barcoding-sqk-rbk114-document-checklist-GridION-en-RBK_9176_v114_revQ_27Dec2024-31.pdf**  
Full rapid sequencing DNA V14 - barcoding library preparation protocol for beginners.  

- **rapid-sequencing-gdna-barcoding-sqk-rbk114-document-document-GridION-en-RBK_9176_v114_revQ_27Dec2024-31.pdf**  
Full library preparation and sequencing protocol for sequencing of a DNA sample using the Rapid Sequencing DNA V14 - barcoding kit.  

- **rapid-sequencing-gdna-barcoding-sqk-rbk114-document-reference-GridION-en-RBK_9176_v114_revQ_27Dec2024-31.pdf**  
Shortened Rapid Sequencing DNA V14 - barcoding library preparation protocol for experienced users.  

- **rapid-sequencing-sqk-rad114-document-checklist-GridION-en-RSE_9177_v114_revO_09Jan2025-37.pdf**  
Full Rapid Sequencing Kit V14 - gDNA (SQK-RAD114) library preparation protocol for beginners.  

- **rapid-sequencing-sqk-rad114-document-document-GridION-en-RSE_9177_v114_revO_09Jan2025-37.pdf**  
Full library preparation and sequencing protocol for sequencing of a DNA sample using the Rapid Sequencing Kit V14 - gDNA (SQK-RAD114) kit.  

- **rapid-sequencing-sqk-rad114-document-reference-GridION-en-RSE_9177_v114_revO_09Jan2025-37.pdf**  
Shortened Rapid Sequencing Kit V14 - gDNA library preparation protocol for experienced users.  


## Lectures
This folder contains the main lecture slides. 

- **DSC-Workshop2025_Mod-1-2_IntroNanopore.pdf** - This lecture provides an overview of Nanopore sequencing, tracing the history of DNA sequencing and introducing the core principles of how Nanopore technology works. It explains basecalling, different sequencing kit options and platforms, from the MinION to the PromethION.

- **DSC-Workshop2025_Mod-2_Cloud-Computing-and-HPCs.pdf** - This lecture introduces students to cloud computing and High-Performance Computing (HPCs). It defines what cloud computing is, explains the different service models (IaaS, PaaS, and SaaS), and provides an introduction to the Google Cloud Platform.

- **DSC-Workshop2025_Mod-3_VersionControl.pdf** - This module introduces the core concepts of version control, explaining its utility for tracking file changes and managing project histories. It provides a detailed look at the Git system and its components, as well as its integration with platforms like GitHub.

- **DSC-Workshop2025_Mod-3_pipelines-workflows-containers.pdf** - This lecture focuses on computational tools for enhancing research reproducibility. It explains what pipelines, containers and workflow management systems are and provides examples for each.

- **DSC-Workshop2025_Mod-3_Reproducible-Research-Principles.pdf** - Link to Pat Schloss’ Riffomonas tutorial series on reproducible research principles. 


## Notebooks
This folder contains Jupyter notebooks for the nanopore data analysis and the version control with Git module. 

### Nanopore Analysis
- **DSC_Module_2_Epi2meSetup.ipynb** - Install & test Nextflow to use with Epi2me pipelines

- **DSC_Module_2_wf-bacterial-genomes.ipynb** - Runs the Epi2me bacterial-genomes workflow including genome assembly & annotation, and Isolate Characterization.

- **DSC_Module_2_wf-metagenomics.ipynb** - Runs the Epi2me metagenomics workflow including Taxonomic Classification and antimicrobial Resistance (AMR) Detection.

- **DSC_Module_4_get_stats.ipynb** - Walkthrough of the get_all_stats.sh script.

- **DSC_Module_4_install_bioinfo_tools.ipynb** - Walkthrough of the install_bioinfo_tools.sh script.

- **DSC_Module_4_process_AS.ipynb** - This document provides a step-by-step walkthrough of the adaptive sampling analysis pipeline.

### Git
- **Lesson1_Setting_up_git.ipynb** - This notebook includes configuring your git environment.

- **Lesson2_Create_Project_and_View_History_Ignoring_Files.ipynb** - This notebook includes creating your first version-controlled project, learning how to stage and commit a file, make changes to this file, view the history of your project, and create the .gitignore file. 

- **Lesson3_Connecting_to_Github.ipynb** - This notebook includes setting up a new Github profile and connecting your local repository to it. 

- **Lesson4_Branching_merging.ipynb** - This notebook includes how to create a new branch, commit changed to the new branch, and merge it back with the main branch

- **Lesson5_Collaborating.ipynb** - This notebook includes how to collaborate on a project with a colleague by working on the same file and merging into a shared branch.  

- **Lesson6_Managing_Conflict.ipynb** - This notebook includes how to solve a merge conflict during a collaboration.

- **Lesson7_RStudioServer_Git.ipynb** - This notebook includes how to clone your repository into RStudio Server and use RStudio's built-in Git tools to commit and push changes back to your GitHub repository. 
