# Fungal communities across a surface water permanence gradient in a non-perennial prairie stream network.
### Bioinformatics and Data analysis
This repository contains code for replicating an analysis of fungal communities collected from an intermittent stream network, associated with a manuscript (Bond et al. In Review). 

This research was conducted as part of the AIMS Project (Aquatic Intermittency effects on Microbiomes in Streams), supported by an NSF EPSCoR Track II Grant # OIA 2019603

This pipeline is composed of two main components: 
1) Bioinformatics / processing of amplicon sequences to prouce ASVs following the DADA2 pipeline.
2) Analysis of fungal communities with environmental data.
We also include code for generating maps and calculating some environmental parameters from previously published environmental datasets.

### DATA AVAILABILITY.
Links to each dataset are provided below. 

Raw ITS1 Metabarcoding FASTQ sequencing data: 
NCBI SRA repository BioProject accension: PRJNA1047139 
Link: https://dataview.ncbi.nlm.nih.gov/object/PRJNA1047139 

Metadata availability: 
Site physical characteristics: 
Ramos, R., A. Burgin, S. Zipper (2023). Konza_Synoptic_Physical_Characteristics, HydroShare, https://www.hydroshare.org/resource/5de4d9eb2d224290b13d469f58dc882b/

Microbial field sampling metadata: 
Bond, C. T., K. A. Kuehn, L. Zeglin (2023). AIMS_GP_approach3_MIME, HydroShare, http://www.hydroshare.org/resource/6bde27bce59044e9881eb35844efd230  

Chlorophyll-a: 
Bond, C. T., E. Stanley, K. A. Kuehn (2024). AIMS_GP_approach3_CHLA, HydroShare, http://www.hydroshare.org/resource/01135480279340cd8e457a22e7b9208b

Stream Temperature, Intermittency, and Conductivity (STIC) logger data: 
Wheeler, C., S. Zipper (2023). South Fork Kings Creek (Konza) Stream Temperature, Intermittency, and Conductivity Data, HydroShare, http://www.hydroshare.org/resource/d9510181f4164a5eba063d75e3fd1395

StreamDAG connectivity metrics (see konza_full network in R package StreamDAG): 
Aho, K., C. Kriloff, S. E. Godsey, R. Ramos, C. Wheeler, Y. You, S. Warix, D. Derryberry, S. Zipper, R. L. Hale, C. T. Bond, and K. A. Kuehn. 2023. Non-perennial stream networks as directed acyclic graphs: The R-package streamDAG. Environmental Modelling & Software 167:105775.

Long-term burn history data from Konza LTER: 
Blair, J., and P. O’Neal 2024. KFH01 Konza prairie fire history ver 19., Environmental Data Initiative. 


#### Working data
For ease of use, in the phyloseq_tabs folder, I have included a compressed file (fall2023.zip) containing the combined metadata table with all processed environmental data used, along with ASV counts and taxonomy used in the data analysis R markdown document. 


### Outputs
I have posted knitted documents of the current versions of the bioinformatics pipeline (Appendix S1) and data analysis (Appendix S2) on Rpubs for reference.

APPENDIX S1. Bioinformatics pipeline in R with code used to generate ASV count table and taxonomy table from raw FASTQ sequencing data, available online: https://rpubs.com/carbon14bond/kzsynITS_09152023_CTB
APPENDIX S2. Data analysis R code, including statistical tests and figure generation. 
https://rpubs.com/carbon14bond/Appendix_S2_Konza_ITS_data_analysis_Bond_4-15-2025
