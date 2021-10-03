# TCGA-Breast-Cancer-Classifier
The Cancer Genome Atlas (TCGA) is a database with multi-omic information on cancer and normal patients. This project is a spin-off of an African Society of Bioinformatics and Computational Biology (ASBCB) June 2021 Codeathon project, that aimed to combine TCGA Copy Number Variation (CNV), DNA Methylation and Gene Expression data, and build machine learning models for classifying breast cancer subtypes. Unfortunately, that project could not be completed during the codeathon. Here, attempts were made to complete the project post-codeathon by downloading corresponding CNV, DNA Methylation and Gene Expression Data for building the classification models. However, the TCGA CNV data has no clinical information (eg: whether sample is cancerous or normal) and had to be disregarded. And the DNA Methylation and Gene Expression Data had no patients in common, so only the DNA Methylation Data was used for building the models. 
Elastic Net and k-Nearest Neighbor models were developed with pre-normalized DNA Methylation beta-values and used to classify unseen TCGA Breast Cancer samples as either tumor or normal samples. Interestingly, the relevant genes for the Elastic Net classification showed differential methylation when the tumor and normal samples were hierarchically clustered on a heatmap. This work was enabled by the 'Analysis of Cancer Genome Atlas in R' tutorial by Ivan Costa's Computational Genomics group at RWTH AACHEN University. Many thanks to the Costa Lab for the wonderful tutorial. Feel free to modify the code for your own interests. New collaborations are highly welcomed!
