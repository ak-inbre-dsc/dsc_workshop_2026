---
title: "Module 2_4: Git Module Setup"
layout: page
permalink: /tutorials/Git_Startup/
date: 2026-05-10
nav_order: 4
---

# Getting started with Git

## 1. Start your small (e2-standard-4) instance & open JupyterLab.

## 2. Remove the old workshop repository (if present). In the **Terminal**, run:
```bash
rm -r dsc_workshop_2026/
```

## 3. Clone the workshop Git repository

### GUI method 

1. In the top menu, choose **Git → Clone a Repository…**  
2. Paste `https://github.com/ak-inbre-dsc/dsc_workshop_2026.git` and click **Clone**.  
3. The repo appears in the file browser inside `~/dsc_workshop_2026/`.

### Terminal alternative

```bash
cd ~
git clone https://github.com/ak-inbre-dsc/dsc_workshop_2026.git
```
---

## 4. Work through the workshop notebooks

Open the **`notebooks/Git`** folder inside the cloned repo and run the notebooks **in this order**:

| # | Notebook                                  
|---|---------------------------------------------|
| 1 | `DSC_Module_3_Lesson1_Git.ipynb`           
| 2 | `DSC_Module_3_Lesson2_Git_and_Github.ipynb`  
| 3 | `DSC_Module_3_Lesson3_Collaborating_Collaborator1.ipynb / DSC_Module_3_Lesson3_Collaborating_Collaborator2.ipynb`   
| 2 | `DSC_Module_3_Lesson4_RStudioServer_Git.ipynb`  

