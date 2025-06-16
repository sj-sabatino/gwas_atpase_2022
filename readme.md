# 🧬 sjs_pipeline

A Snakemake pipeline for processing paired-end FASTQ files using common bioinformatics tools such as FastQC, Trimmomatic, BWA, Samtools, and Picard.

---

## 📦 Requirements

- [Snakemake](https://snakemake.readthedocs.io/)
- Python 3.7+
- Bioinformatics tools:
  - `fastqc`
  - `trimmomatic`
  - `bwa`
  - `samtools`
  - `picard`

---

## 📁 Directory Structure

```bash
.
├── Snakefile
├── config.yaml
├── samples.csv
├── data/                     # Input FASTQ files
├── ref/                      # Reference genome files
├── adapters/                 # Adapter sequences for Trimmomatic
├── logs/                     # Logs per step per sample
├── trimmed/
├── aligned/
├── bam/
├── results/
├── metrics/
└── qc/

##Docker
Docker pull sabatino75/fastq_to_bam_v1
