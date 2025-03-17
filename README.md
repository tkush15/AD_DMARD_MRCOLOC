# AD_DMARD_MRCOLOC
Statistical code used for the paper, "Assessing the Causal Relevance of Actionable DMARD Targets and Alzheimer’s Disease: A pQTL-Based Mendelian Randomization and Genetic Colocalization Analysis"

## Environment details
R version 4.2.3

## Analysis overview
Multiple two sample Mendelian randomization and colocalization analyses were performed using the following data.
### Instrument-exposure data
To instrument the selected DMARD targets — PLA2G1B, NFKB1, ACE2, LTA, FCGR2A, FCGR2B, FCGR3B, TNF, IL6R — we pulled lead SNVs from the UK BioBank Pharma Proteomics Project via synapse.org (project ID: syn51364943).

The .tar files for each target were manually downloaded and read into R using Mac Terminal. The data was then cleaned and reorganized to match the required structure for MR analysis (e.g., adding GRCh38 IDs, transforming -log10 p values, correcting column labels). GRCh38 ID data was sourced from Dr. Emma Anderson at the University of Bristol/University College London but may be downloaded from the NCBI as a .zip file.

If you want to skip these steps, a file is included in this project containing the clumped SNVs that were used in MR analyses.

### AD outcome data
Outcome data was sourced from a large-scale GWAS on AD risk loci. Permission for access may be requested via The National Institute on Aging Genetics of Alzheimer’s Disease Data Storage Site repository (ID: NG00075).
