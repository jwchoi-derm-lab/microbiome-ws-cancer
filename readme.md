# 🦠 Skin Cancer Multi-Omics: Microbiome & Microbial Dark Matter (MDM)

![Ubuntu](https://img.shields.io/badge/Ubuntu-24.04-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-4.4+-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?style=for-the-badge&logo=docker&logoColor=white)

> **Investigating the tumorigenic role of the microbiome and unclassified microbial dark matter in skin cancers through the integration of shotgun metagenomics and LC-MS/MS-based quantitative proteomics.**

---

## 🔬 Project Overview
This repository contains bioinformatics pipelines and analysis codes to explore the microbial ecosystems of basal cell carcinoma, squamous cell carcinoma, and melanoma. By integrating genomic and proteomic data, we aim to identify cancer-associated microbial communities, discover their unique protein expressions, and uncover how these factors interact with the host tumor microenvironment.

## 📊 Data and Methodology
- **Samples:** Paired tumor and adjacent normal tissues, alongside non-invasive tape-stripping samples.
- **Genomics:** Shotgun metagenomic sequencing to build **Metagenome-Assembled Genomes (MAGs)** for identifying unclassified MDM.
- **Proteomics:** High-resolution mass spectrometry (LC-MS/MS) for capturing limited protein biomass.
- **Integration:** Customized proteogenomic pipelines mapping mass spectra against specific microbial databases to accurately identify microbe-derived proteins.

## 💻 Environment & Infrastructure
These workflows are explicitly optimized for a **high-performance local Ubuntu workstation**, bypassing the need for cluster workload managers like Slurm or Swarm. 

- **OS:** Ubuntu 24.04.4 LTS
- **Hardware:** Lenovo ThinkPad P16 Gen 3 (Intel Core Ultra 9, 24 Cores)
- **Memory / Storage:** 192GB RAM / 12TB Storage

## 📂 Repository Structure
```text
📦 skin-cancer-microbiome
 ┣ 📂 01_qc_preprocessing    # DNA quality control and host read depletion (Bash/Python)
 ┣ 📂 02_mag_assembly        # Contig assembly, binning, and refinement (Bash)
 ┣ 📂 03_proteogenomics      # LC-MS/MS spectra mapping and database construction (Python)
 ┣ 📂 04_integration         # Multi-omics cross-validation and network analysis (R)
 ┗ 📜 README.md
```

## 🚀 Quick Start
Since this pipeline runs natively on a local workstation, you can execute the scripts directly without submitting jobs to a scheduler.

```bash
# 1. Clone the repository
git clone https://github.com/username/skin-cancer-microbiome.git
cd skin-cancer-microbiome

# 2. Run the preprocessing script (Example)
bash 01_qc_preprocessing/run_qc.sh --input ./data/raw --output ./data/clean
```

## 📬 Contact / Author
**Jeewoong Choi**
- Dermatologist & Microbiome Researcher
- [GitHub Profile](https://github.com/username)
