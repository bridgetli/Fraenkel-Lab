# Fraenkel-Lab
Code I've written for my undergraduate research position in the Fraenkel Lab at MIT.

### Code use:
Please see .ipynb files for code and descriptions about what the code does. .ipynb files that start with SNF do SNF and spectral clustering. Other .ipynb files are for downstream analysis of clusters. The rest of the files in each folder are inputs or outputs.

### Project summary:
Amyotrophic lateral sclerosis (ALS) is a neurodegenerative disease that affects upper
and lower motor neurons. The genetic makeup of ALS is not well understood, and no effective treatment exists. There is substantial heterogeneity in disease progression, age of onset, nonmotor symptoms, and underlying genetics. Therefore, it is important to understand different subtypes of ALS and their molecular signatures.

This project uses similarity network fusion (SNF) and spectral clustering to identify subtypes of ALS. SNF constructs networks of samples for each available data type, then fuses them into one network that represents the full spectrum of underlying data. We used datasets of different omics groups, including bulk proteomics, bulk RNA-seq (transcriptomics), and bulk ATAC-seq (epigenomics). In addition, we incorporated patient metadata, such as sex, age at symptom onset, race, site of onset, progression data, reported mutations, and more. This data is all available through Answer ALS.

Clusters were then analyzed to determine clinical
phenotypes, differentially expressed genes and proteins, and gene ontology.
This analysis can lead to the identification of molecular signatures for each subtype. We identified a biological covariate, s100b, that was causing noise in clustering. The batch effect from s100b was removed using regression and PCA. 

See "ALS Subtype Discovery.pdf" for overview and results.
