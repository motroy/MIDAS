# PhyloCNV
PhyloCNV is an integrated pipeline and for estimating the abundance, gene content, and phylogeny of microbial species from metagnomic data.  PhyloCNV leverage a database of 30,000 Bacterial genomes that have been clustered into species groups using a panel of 30 universal-single-copy genes.  PhyloCNV consists of three main modules: 
* Species Abundance Estimation  
 -rapidly map reads to db of universal genes & probabalistally assign reads to species groups  
 -estimate genome coverage of species-groups   
* Pan Genome Alignment and Coverage  
 -build a bowtie2 database of pangenomes from abundant species    
 -use bowtie2 to map reads to pangenome database  
 -compute normalized coverage of genes  
* Single Nucleotide Variant Prediction  
-build a bowtie2 database of representative genomes from abundant species  
-use bowtie2 to map reads to genome database  
-call SNVs and estimate allele frequencies     

## Table of Contents
1. [Requirements and Dependencies] (https://github.com/snayfach/PhyloCNV/blob/master/docs/requires.md)
2. [Download, Installation, and Testing] (https://github.com/snayfach/PhyloCNV/blob/master/docs/install.md)
3. Run PhyloCNV on a single sample:
* [Estimate species abundance] (https://github.com/snayfach/PhyloCNV/blob/master/docs/species.md)
* [Call gene copy-number variants] (https://github.com/snayfach/PhyloCNV/blob/master/docs/cnvs.md)
* [Call single-nucleotide variants] (https://github.com/snayfach/PhyloCNV/blob/master/docs/snvs.md)
4. Merge results across samples:
* [Merge species abundance] (https://github.com/snayfach/PhyloCNV/blob/master/docs/merge_species.md)
* [Merge copy-number variants] (https://github.com/snayfach/PhyloCNV/blob/master/docs/merge_cnvs.md)
* [Merge single-nucleotide variants] (https://github.com/snayfach/PhyloCNV/blob/master/docs/merge_snvs.md)

## Citation
If you use this tool, please cite:
Nayfach, S. and Pollard, KS. PhyloCNV: an integrated, high-resolution pipeline for quantifying strain-level variation from shotgun metagenomes (In Preparation).
