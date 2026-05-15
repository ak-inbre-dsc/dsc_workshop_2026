![header](assets/images/Header.png)

# Materials for the 2026 Alaska INBRE Data Science Core Genomics Workshop 

Welcome! This repository contains the materials that we used during our 2026 workshop. The easiest way to access all the materials is to [download the whole repository](https://github.com/ak-inbre-dsc/dsc_workshop_2026/archive/refs/heads/main.zip). 


## ![](assets/images/ppt_icon.png) [Lectures](lectures)  

1. [Introduction to Nanopore Sequencing](lectures/DSC_Workshop2026_Mod_1_2_IntroNanopore.pdf)
2. [Data Generation & Mock Communities](lectures/DSC_Workshop2026_Mod_1_3_DataGeneration.pdf)
3. [Cloud Computing and HPCs](lectures/DSC_Workshop2026_Mod_2_1_CloudComputing.pdf)
4. [Intro to Command Line](lectures/DSC_Workshop2026_Mod_2_2_IntroCommandLine.pdf)
5. [Google Colab](lectures/DSC_Workshop2026_Mod_2_3_Colab.pdf)
6. [Reproducible Research Principles & Git](lectures/DSC_Workshop2026_Mod_3_1_Reproducible_Research_Principles_Git.pdf)
7. [Reproducible Research Tools & Github](lectures/DSC_Workshop2026_Mod_3_2_Reproducible_Research_Tools_Github.pdf)

##  :notebook: [Jupyter Notebooks](notebooks/)

### 1. Nanopore Analysis
* [Epi2me setup](notebooks/Nanopore_Analysis/DSC_Module_2_Epi2meSetup.ipynb)  
* [Epi2me bacterial-genomes workflow](notebooks/Nanopore_Analysis/DSC_Module_2_wf-bacterial-genomes.ipynb)  
* [Epi2me metagenomics workflow](notebooks/Nanopore_Analysis/DSC_Module_2_wf-metagenomics.ipynb)  
* [Walkthrough of the get_all_stats.sh script](notebooks/Nanopore_Analysis/DSC_Module_4_get_stats.ipynb) 
* [Walkthrough of the install_bioinfo_tools.sh script](notebooks/Nanopore_Analysis/DSC_Module_4_install_bioinfo_tools.ipynb)
* [Adaptive sampling analysis pipeline](notebooks/Nanopore_Analysis/DSC_Module_4_process_AS.ipynb)


### 2. Version Control with Git
* Lesson 1: [Git basics](notebooks/Git/DSC_Module_3_Lesson1_Git.ipynb)  
* Lesson 2: [Git & Github](notebooks/Git/DSC_Module_3_Lesson2_Git.ipynb)  
* Lesson 3a: [Collaborating with Github: Collaborator 1](notebooks/Git/DSC_Module_3_Lesson3_Collaborating_Collaborator1.ipynb)  
* Lesson 3b: [Collaborating with Github: Collaborator 2](notebooks/Git/DSC_Module_3_Lesson3_Collaborating_Collaborator2.ipynb) 
* Lesson 4: [Using Git with RStudio Server](notebooks/Git/DSC_Module_3_Lesson4_RStudioServer_Git.ipynb)  


## ![](assets/images/code_icon.png) [Scripts](scripts/)

* [Install bioinformatics tools](scripts/install_bioinfo_tools.sh) on a Google Cloud workbench instance.
* [Process and analyze nanopore adaptive sampling data](scripts/as_processing_cloud_v2.sh)
* [Collect SeqKit stats](scripts/get_all_stats.sh) for various FASTQ outputs from the adaptive sampling analysis pipeline.
* Visualize sequencing data in R through [violin plots](scripts/violinplot_treatments_isolates.R) 
* Create [bar plots](scripts/plot_treatments_isolates.R) in R to compare different sequencing metrics.


## :bookmark_tabs: [Nanopore Handouts](handouts)  
Descriptions of the mock communities and different library prepapration methods 

* [Mock Communities](handouts/Mock_Communities)
* [Sequencing protocols & Information](handouts/Protocols)


*Alaska INBRE is an Institutional Development Award (IDeA) from the National Institute of General Medical Sciences of the National Institute of Health (NIH) under grant number P20GM103395.*


## License
This project is licensed under the [Creative Commons Attribution (CC BY-NC-SA)](LICENSE).
