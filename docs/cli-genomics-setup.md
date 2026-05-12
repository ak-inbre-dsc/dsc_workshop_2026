---
title: "Module 2_2: Setup Data for ‘Introduction to the Command Line for Genomics’"
layout: page
permalink: /tutorials/cli-genomics-setup/
date: 2026-05-10
description: "Download and unpack the Data Carpentry shell_data files on your Google Cloud instance (or any Linux terminal)."
nav_order: 2
---

> This tutorial was designed by the fine folks from Data Carpentry - a non-profit organization that teaches fundamental data management and analysis skills to researchers. You will be following their  *Introduction to the Command Line for Genomics* lesson today.

---
### Before you begin:
If your instance is not yet powered up, start it following these steps
1. Navigate to **Agent Platform → Notebooks → Workbench**.
2. Make sure you're in the **Instances** view.
3. Select the checkbox next to your instance and click **Start**. Once the instance shows a green checkmark (you may need to refresh if this takes long), open **JupyterLab**.
4. Open a new **Terminal**
---

### 1 · Navigate to Your Home Directory
Always keep workshop data in a tidy location (e.g., `$HOME`).

```bash
cd ~    # jump to your home directory
```

---

### 2. Create a folder for your data files

```bash
mkdir shell_data
cd shell_data
```

---

### 3 · Download the dataset from a Google Cloud Storage Bucket
```bash
gcloud storage cp --recursive gs://data_workshop_cli/* .
```

You should see sub-folders called `sra_metadata/` and `untrimmed_fastq/` in your `shell_data` folder. 

---

### 4. The lesson starts in your home directory, so navigate back there
```bash
cd ~
```
---

### Next steps

Today you will cover the 6 topics below using Data Carpentry's *Introduction to the Command Line for Genomics* tutorial. As we are working from Jupyter Lab on our Google Cloud instance, you can **skip the crossed-out sections**:

1. Introducing the Shell
- What is a shell and why should I care?
- ~~How to access the shell~~
- ~~How to access the remote server~~
- Navigating your file system
- Summary
2. Navigating Files and Directories
3. Working with Files and Directories
4. Redirection
5. Writing Scripts and Working with Data
6. Project Organization

## [Click here to open the tutorial](https://datacarpentry.github.io/shell-genomics/01-introduction.html)!

---
  
**If you are already comfortable with basic commandline**, [this page](https://jayconrod.com/posts/103/intermediate-linux-command-line-tutorial) walks through additional useful commands for intermediate level users. 


