---
title: "Module 2_3: Nanopore data analysis using EPI2ME"
layout: page
permalink: /tutorials/EPI2ME-workbench/
date: 2026-05-10
description: "Spin up an e2‑standard‑8 notebook instance, mount the dsc‑epi2me‑demo bucket, and clone the workshop repo—Console‑only."
nav_order: 3
---

> **Why an e2‑standard‑8?** The 8 vCPU / 32 GB RAM VM gives faster I/O and more head‑room for assembly tasks compared with the default e2‑standard‑4.

This guide walks through creating the instance in the Google Cloud Console, opening JupyterLab, mounting a Cloud Storage bucket, cloning the workshop’s GitHub repo, and running the example notebooks.

---

## 1 · Prerequisites

- A Google Cloud project with **billing enabled**.
- Project‑level **Editor** (or higher) permissions.
- The **Notebooks**, **Agent Platform API**, and **Compute Engine API** APIs enabled.

---

## 2 · Create the e2‑standard‑16 instance

1. Open **Agent Platform → Notebooks → Workbench**.  
2. Click **Create New** and scroll down to click **Advanced Options**.  
3. Complete the form:

   | Field            | Value                                                   |
   | ---------------- | ------------------------------------------------------- |
   | **Name**         | `dsc-workshop-e2-16`                                 |
   | **Region**       | the same region you used before (e.g., `us-central1`)   |
   | **Machine type** | **e2-standard-16** (16 vCPU / 64 GB RAM)                |


4. Leave permissions and everything else unchanged and click **Create**. Wait until the status is **RUNNING**.

---

## 3 · Open JupyterLab

 Once the instance is running, click **Open JupyterLab** next to the instance name. A new browser tab launches your notebook environment.

---

## 4 · Mount the `dsc‑epi2me‑demo` bucket

### Using **Mount Shared Storage** (JupyterLab 3 GUI)

1. In the **File Browser** pane, click the **Mount Shared Storage** icon (triangle above a line).  
2. Choose **Cloud Storage bucket**, enter `dsc-epi2me-demo`, and click **Mount**.  
3. The bucket now appears as a top‑level folder and is available at `/home/jupyter/dsc-epi2me-demo/`.

### Terminal alternative (optional!)

```bash
# In a JupyterLab Terminal tab
mkdir -p ~/dsc-epi2me-demo
gcsfuse dsc-epi2me-demo ~/dsc-epi2me-demo
```

*(gcsfuse is pre‑installed on Workbench VMs.)*

---

## 5 · Clone the workshop Git repo

### GUI method (Git menu)

1. In the top menu, choose **Git → Clone a Repository…**  
2. Paste `https://github.com/ak-inbre-dsc/dsc_workshop_2026.git` and click **Clone**.  
3. The repo appears in the file browser inside `~/dsc_workshop_2026/`.

### Terminal alternative

```bash
cd ~
git clone https://github.com/ak-inbre-dsc/dsc_workshop_2026.git
```

---

## 6 · Work through the workshop notebooks

Open the **`notebooks/Nanopore_Analysis`** folder inside the cloned repo and run the notebooks **in this order**:

| # | Notebook                                    | Purpose                                                                    |
|---|---------------------------------------------|----------------------------------------------------------------------------|
| 1 | `DSC_Module_2_Epi2meSetup.ipynb`            | Configure the Epi2me environment and verify data access.                   |
| 2 | `DSC_Module_2_wf-metagenomics.ipynb`        | Execute the **wf-metagenomics** workflow and explore classification output |
| 3 | `DSC_Module_2_wf-bacterial-genomes.ipynb`   | Run the **wf-bacterial-genomes** workflow and inspect assembly results     |

**Running tips**

1. Double‑click a notebook to open it.  
2. Use the ▶ **Run** button or **Shift + Enter** to execute each cell.  
3. Follow in‑notebook instructions and fill in any TODOs.  
4. Save progress frequently (**File → Save and Checkpoint**).

---

## 7 · Cost‑saving reminder

When you’re finished, return to the **Instances** list (Agent Platform → Notebooks → Workbench), check your notebook VM, and click **Stop**. Billing pauses while the instance is stopped.
