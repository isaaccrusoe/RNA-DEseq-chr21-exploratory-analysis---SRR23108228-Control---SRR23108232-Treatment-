# Methods

## Data Acquisition
Public RNA-seq datasets were obtained from NCBI SRR23108228 (control) and SRR23108232 (Treated). Due to hardware limitations,
analysis was restricted to chromosome 21 to allow full pipeline execution.

## Quality Control and Trimming
Raw FASTQ files were processed using **Trimmomatic** to remove adapters and low-quality bases.
This step ensured high-quality reads for downstream alignment.

## Alignment
Reads were aligned to a chromosome 21 reference using **HISAT2 / STAR**.
BAM files were sorted and indexed.

## Gene Counting
Gene-level counts were generated and compiled into a count matrix for downstream analysis.

## Differential Expression Analysis
DESeq2 was used to:
- Normalize counts
- Estimate dispersion
- Compute log2 fold changes

Due to the absence of biological replicates, full statistical inference was limited.
However, the workflow and interpretation steps were fully learned and implemented.

## Visualization
- MA plot
- Log2 fold change vs mean expression plot
- Heatmap of expression patterns
