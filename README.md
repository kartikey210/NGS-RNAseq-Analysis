 End-to-end RNA-Seq analysis pipeline using real sequencing data
# NGS RNA-Seq Analysis Pipeline

## Overview
This project demonstrates a complete RNA-Seq data analysis workflow, starting from raw sequencing data to alignment and visualization. It replicates real-world bioinformatics pipelines used in research and industry.

---

## Workflow

SRA → FASTQ → Quality Control → Trimming → Alignment → BAM → Visualization

---

## Dataset

- Source: NCBI SRA  
- Accession: SRR390728  
- Type: RNA-Seq (single-end)  
- Total Reads: ~7 million  

---

## Tools Used

- SRA Toolkit  
- Falco (FastQC alternative)  
- Trimmomatic  
- Bowtie2  
- SAMtools  
- IGV  

---

## Pipeline Steps

### Data Acquisition
- Downloaded sequencing data using SRA Toolkit  
- Converted SRA → FASTQ format  

### Quality Control
- Performed QC using Falco  
- Identified low-quality bases at read ends  

### Trimming
- Applied Trimmomatic  
- Removed low-quality bases to improve read quality  

### Alignment
- Aligned reads to human reference genome (hg38) using Bowtie2  

### Alignment Evaluation
- Used SAMtools flagstat  
- Achieved **93.5% mapping rate**  

### Visualization
- Visualized BAM file using IGV  
- Verified correct read alignment and coverage  

---

## Results

- Total Reads: ~7.1 million  
- Mapped Reads: ~93.5%  
- High-quality alignment confirmed  

---

## Results Visualization

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

---

## Conclusion

The pipeline successfully processed RNA-Seq data, demonstrating effective preprocessing, high-quality alignment, and accurate visualization of genomic reads.

This project reflects hands-on experience with real bioinformatics workflows used in research and industry.

---

## Author

**Kartikeya Sharma**  
Bioinformatics Student
