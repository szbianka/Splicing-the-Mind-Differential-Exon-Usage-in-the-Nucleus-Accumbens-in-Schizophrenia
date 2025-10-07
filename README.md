# 🧠 Splicing the Mind: Differential Exon Usage in the Nucleus Accumbens in Schizophrenia

*A Master’s Thesis in Cognitive Science*  
**Author:** Bianka Szöllösi
**Institution:** Aarhus University  
**Supervisor:** Per Qvist  
**Year:** 2025 

---

## 🎯 Project Overview

This repository accompanies the Master’s thesis **“Splicing the Mind: Differential Exon Usage in the Nucleus Accumbens in Schizophrenia.”**  
The project bridges cognitive science and molecular psychiatry through the analysis of transcriptomic data.  

The study investigates whether **schizophrenia is associated with differential exon usage (DEU)** in the **nucleus accumbens (NAcc)** — a subcortical brain region central to motivation and reward processing — and evaluates the potential of **curated multi-study resources**, such as **QIAGEN’s OmicSoft DiseaseLand**, to support reproducible splicing analyses.

Using the **DEXSeq** framework in R, the analysis tests for exon-level regulation differences between schizophrenia patients and healthy controls across two publicly available RNA-seq studies.  
Results are integrated with **brain splicing QTLs (sQTLs)** and **genome-wide association study (GWAS)** data to assess genetic plausibility.

Although no genome-wide significant DEU genes were detected, twelve candidate genes were identified in one dataset, several of which (**BRWD1**, **PDE2A**, **SBF2**, **CERT1**) are linked to neurodevelopmental and regulatory processes.  
The project establishes a **transparent, reproducible workflow** for exon-level transcriptomic analysis and highlights the challenges of cross-study heterogeneity in psychiatric genomics.

---

## 📁 Repository Contents

| File / Folder | Description |
|----------------|-------------|
| `tutorial_DEU_notebook.ipynb` | Step-by-step tutorial for performing DEXSeq-based differential exon usage analysis. *(Requires access to QIAGEN OmicSoft)* |
| `requirements_python.txt` | Python dependencies for running preprocessing and data-handling scripts. |
| `requirements_R.txt` | R dependencies for DEXSeq and downstream analysis. |

---

## ⚙️ Installation

### Python environment
Install required Python packages:
```bash
pip install -r requirements_python.txt

### R environment
pkgs <- readLines("requirements_R.txt")
install.packages(sub("==.*", "", pkgs))

## Execution Notes:
- The combined DEU analysis (two-study model) is computationally intensive and may take ~30 hours on a local machine.
Consider using a high-performance or cloud-based environment (e.g., virtual machine or a server with ≥32 GB RAM) for faster execution.

## Data resource
- 🧬 QIAGEN OmicSoft DiseaseLand (licensed)

## 🧠 Research Significance

This project illustrates how cognitive scientists can approach biomedical data analysis with a focus on reproducibility and interpretability.
It emphasizes:
- the importance of open and standardized data curation in psychiatric research,
- the potential of transcriptomic biomarkers to bridge molecular and behavioral levels of explanation, and
- the need for interdisciplinary collaboration between data science, psychiatry, and cognitive neuroscience.

## 🧾 License
This repository is distributed for academic and educational purposes.
Data retrieved from QIAGEN’s OmicSoft DiseaseLand are subject to QIAGEN’s licensing terms and are not publicly redistributable.

## 🙌 Acknowledgements

Special thanks to Per Qvist for his supervision and academic support, and to Dimitrii Kamaev (Qiagen) for technical support.
