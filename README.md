# Whelan_scRNA_Esophagus_Dec21

This repository contain R scripts used for the Whelan Lab publication on the single-cell biology of the murine epithelium.
Please download the 10X FASTQ files or the processed .txt matrices from the GEO accession []. Alternatively, feel free to use 
the Seurat R object aging.epi.clean.Robj, also provided in the GEO accession. 

The core dependencies for these scripts:
1. R 4.0 https://www.r-project.org/

2. Seurat 4.0 https://satijalab.org/seurat/

3. Monocle 3 https://cole-trapnell-lab.github.io/monocle3/

For the supplementary verification of epithelial vs. stromal expression in our single-cell dataset, the following are also
necessary:

4. Rsubread 2.8 https://bioconductor.org/packages/release/bioc/html/Rsubread.html

5. DESeq2 1.34 https://bioconductor.org/packages/release/bioc/html/DESeq2.html

For the main topics of our publication, the following pipeline of scripts was followed to create the files and figures 
discussed:

1. PreProcess_And_Cluster details the creation of the Seurat object, integration pipeline, and exclusion of 
   non-epithelial cells in our dataset.

2. Epithelial_Figures delves further into the epithelial dataset and performs the analyses discussed in the 
   paper.
   
3. Pseudotime_Monocle3 shows the process of trajectory inference as well as gene module calculation using Monocle 3.
