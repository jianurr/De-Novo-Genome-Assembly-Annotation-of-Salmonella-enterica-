# Genome Assembly and Annotation of Salmonella enterica

This repository contains the complete workflow I followed to assemble and annotate the genome of Salmonella enterica using Illumina paired-end sequencing data from the NCBI SRA (accession number: SRR2584863). The goal of this project was to understand the full bacterial genome analysis process, from raw sequencing reads to an annotated genome. All major output folders from SPAdes, QUAST, and Prokka are included.

---------------------------------------------------------------------

## Project Summary

This project follows a standard microbial genome analysis workflow. Raw Illumina reads were assembled into contigs using SPAdes, the assembly quality was assessed using QUAST, and genome annotation was performed using Prokka. The repository is organized so that anyone can follow the workflow or inspect each step's results.

---------------------------------------------------------------------

## Dataset Information

Organism: Salmonella enterica  
SRA Accession: SRR2584863  
Platform: Illumina  
Data Type: Paired-end whole-genome sequencing  

FASTQ files are not included due to size limitations, but all analysis was performed using this dataset.

---------------------------------------------------------------------

## Tools Used

SPAdes – de novo genome assembly  
QUAST – assembly quality evaluation  
Prokka – genome annotation  

All tools were installed and executed through Conda environments.

---------------------------------------------------------------------

## Workflow Overview

Raw FASTQ reads  
→ Genome assembly using SPAdes  
→ Assembly quality assessment using QUAST  
→ Genome annotation using Prokka  

Each stage produced output files that are stored in separate directories.

---------------------------------------------------------------------

## Results Summary

QUAST Assembly Results:  
Total contigs: 421  
Contigs ≥ 1000 bp: 214  
Largest contig: 151,779 bp  
Assembly size: 4,597,936 bp  
GC content: 52.16%  
N50: 46,503 bp  
L50: 30  

Prokka Annotation Results:  
Protein-coding genes (CDS): 4,256  
tRNA genes: 93  
rRNA genes: 4  
tmRNA: 1  
Repeat regions: 2  

These results indicate a complete and good-quality bacterial genome assembly and annotation.

---------------------------------------------------------------------

## Repository Structure

README.md  
spades_output/    (SPAdes assembled contigs)  
quast_res/        (QUAST quality assessment reports)  
prokka_output/    (Prokka annotation files)  

---------------------------------------------------------------------

## Reproducibility

This workflow can be reproduced by installing SPAdes, QUAST, Prokka, and SRA Toolkit and running the steps in the same order. The pipeline runs smoothly on Linux-based systems such as Ubuntu or WSL.

---------------------------------------------------------------------

## Purpose of This Work

This project was carried out for hands-on learning in bacterial genome assembly and annotation. The workflow and results in this repository may be helpful for students or researchers learning microbial genomics.

---------------------------------------------------------------------

## Author

Khandakar Jianur Islam  
Bioinformatics | Genomics | NGS Analysis | Linux

---------------------------------------------------------------------

## License

This project is released under the MIT License.
