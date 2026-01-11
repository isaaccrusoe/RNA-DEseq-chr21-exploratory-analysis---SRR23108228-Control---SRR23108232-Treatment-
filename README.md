
<img width="613" height="304" alt="HeatMap" src="https://github.com/user-attachments/assets/7c103d84-8942-4124-841d-3443247600aa" />




# RNA-Seq Differential Expression Analysis (Chr21 Subset)

This project represents my first complete end-to-end RNA-seq bioinformatics workflow,
from raw FASTQ files to gene-level expression analysis and visualization.

Due to limited local computing resources, the analysis focuses on **human chromosome 21**
as a reduced but biologically meaningful subset.

## 🔬 Workflow Overview
- Quality control and trimming (Trimmomatic)
- Read alignment (HISAT2 / STAR)
- Gene-level counting
- Differential expression analysis (DESeq2)
- Visualization (MA plot, log2FC plot, heatmap)

## 🧬 Technologies Used
- Linux (Ubuntu / WSL)
- R & RStudio
- Trimmomatic
- HISAT2 / STAR
- DESeq2              
- ggplot2 / pheatmap

## 📊 Key Outputs
- Count matrix
- Sample metadata
- Log2 fold change results
- Publication-ready plots
- 
### Differential Expression Visualization

Due to the absence of biological replicates, formal differential expression
testing using DESeq2 could not be completed. As a result, statistical log2 fold
change estimates and volcano plots were not generated, in order to avoid
misleading interpretations.

Instead, exploratory analyses were performed, including:

- Sample-to-sample distance heatmap
- Mean–expression (MA-style) plot

These visualizations were used to assess global expression patterns and data
structure rather than infer statistical significance.

This project demonstrates resilience, problem-solving, and practical RNA-seq analysis skills.
