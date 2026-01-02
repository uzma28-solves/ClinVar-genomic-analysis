# ClinVar-genomic-analysis
Genomic analysis of clinically annotated human genetic variants from ClinVar to identify disease-associated genes, and explore patterns of pathogenicity in breast cancer genes.

## Overview
This project starts by performing an exploratory genomic analysis using publicly available ClinVar data and uses those insights to filter and study breast cancer–associated pathogenic variants. The aim is to demonstrate core computational biology skills by handling large-scale variant data, performing biologically motivated filtering, and extracting interpretable insights from genomic coordinates.


## Biological Motivation
Breast cancer susceptibility is strongly influenced by genes such as BRCA1, BRCA2, TP53, and ATM. Many disease-causing variants are not uniformly distributed across genes but tend to cluster in functionally important regions (constrained regions/mutation hotspots).

By analyzing positional distributions and variant densities, we can infer patterns of functional constraint and mutation tolerance directly from data.

## Data Source
- **ClinVar Variant Summary**
- Source: NCBI ClinVar
- Genome build: GRCh38
- Format: Tab-delimited text (.txt.gz)


## Project Workflow

### 1. Data Acquisition
- Download ClinVar variant summary
- Load compressed data directly into Python
- Select only GRCh38-mapped variants

### 2. Data Cleaning & Preprocessing
- Filter for breast cancer–associated genes
- Clean and standardize clinical significance labels
- Retain variants with valid genomic positions
- Export a processed dataset for reproducibility

### 3. Pathogenic Variant Characterization
- Focus on pathogenic and likely pathogenic variants
- Compare variant counts across breast cancer genes
- Interpret differences in disease relevance

### 4. Within-Gene Positional Clustering
- Analyze genomic position distributions within each gene
- Compute descriptive statistics (min, median, quartiles, max)
- Identify genes with strong positional concentration of variants

### 5. Variant Density Comparison
- Calculate variant density as variants per genomic span
- Compare pathogenic vs benign variant densities
- Interpret results in terms of functional constraint and tolerance

## Key Insights
- High-risk genes (BRCA1, BRCA2) show strong positional clustering of pathogenic variants
- Moderate-risk genes exhibit broader and more tolerant variant distributions
- Benign variants tend to occupy wider genomic regions, reflecting reduced functional constraint
- Variant density provides a size-normalized measure of biological importance


## Tools & Technologies
- Python
- pandas, numpy
- matplotlib
- Jupyter Notebook


---

## Future Extensions
- Integration of population-specific allele frequencies
- Functional annotation using external databases
- Machine learning–based pathogenicity modeling

---

## Author
**Uzma Alia** 
-Self-directed learner


