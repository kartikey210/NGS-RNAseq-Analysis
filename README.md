# NGS RNA-Seq Analysis Pipeline

## Overview
This project demonstrates a complete RNA-Seq data analysis pipeline from raw sequencing data to visualization.

---

## Workflow
SRA → FASTQ → QC → Trimming → Alignment → BAM → Visualization

---
## Dataset
- Source: NCBI SRA
- Accession: SRR390728
- Type: RNA-Seq (single-end)

---

## Tools Used
- SRA Toolkit
- Falco / FastQC
- Trimmomatic
- Bowtie2
- SAMtools
- IGV

---

## Steps

### 1. Data Download
Downloaded RNA-Seq data using SRA Toolkit and converted to FASTQ.

### 2. Quality Control
Performed QC using Falco and identified low-quality bases.

### 3. Trimming
Applied Trimmomatic to remove low-quality reads.

### 4. Alignment
Aligned reads to human genome (hg38) using Bowtie2.

### 5. Evaluation
Used SAMtools flagstat → **93.5% mapping rate**

### 6. Visualization
Visualized BAM file using IGV.

---

## Results
- Total reads: ~7 million  
- Mapping rate: **93.5%**

---

## Conclusion

The pipeline successfully processed RNA-Seq data and demonstrated high-quality alignment and visualization.

This project demonstrates hands-on experience with real RNA-seq data analysis workflows used in bioinformatics research and industry.

---


## Screenshots

### IGV Visualization (TP53 Gene)
![IGV Result](screenshots/igv_tp53_alignment.png)

The IGV visualization shows aligned RNA-seq reads mapped to the TP53 gene region, with clear coverage peaks indicating successful alignment.

---

### Quality Control (Falco)

#### Per Base Sequence Quality
![Per Base Quality](screenshots/per_base_sequence_quality.png)

#### GC Content
![GC Content](screenshots/per_sequence_gc_content.png)

#### Adapter Content
![Adapter Content](screenshots/adapter_content.png)
