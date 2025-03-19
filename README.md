## INSCRIBE: A scalable approach to in situ readout of the single cell signaling histories

This repository provides analysis resources and demostration pipelines for the manuscript under review, titled **"Genetic recording and in situ readout of single cell signaling histories"**, a modified version of the preprint **"Reconstructing signaling history of single cells with imaging-based molecular recording"**, available [here] https://www.biorxiv.org/content/10.1101/2024.10.11.617908v1

## Code availability
All custom scripts wrote in Python Jupyter Notebook and processed data required to replicate our analysis are included in this repository, which organized as two main folders,

- **Analysis**, contains `.csv` files about the detailed experimental conditions, and Jupyter Notebooks to replicate the results which use the **Processed data** as input.

- **Processed Data**, includes the output data generated from our processing pipeline, two demostration of which is included in the **Demo** folder.

*Note, the subfolder is organized as the annotation of **Figures** corresponding to the manuscript under review.* 

## Running an demo pipeline

The **Demo** folder provides two example analysis pipelines, each with detailed Jupyter Notebooks and datasets:

- **Amplicon Sequencing**  

  - The **alignment pipeline** is demonstrated on the **"reference plasmid"** dataset to generate `.sam` files for further analysis, executed on Google Colab.  

  - The **After-alignment processing pipeline** is demonstrated on the **"WntR_Rep1.sam"** dataset, located in `/Processed data/Fig. 4/Aligned/`.  
  
  *Note, The INSCRIBE barcode array amplicon sequencing raw datasets are deposited in the **NCBI Sequence Read Archive (SRA)** under accession number **PRJNA1232380**.* 

- **Ratiometric Barcode Readout**  

  - A **maximum intensity projection & Cellpose segmentation pipeline** is demostrated for one of the conditions from the **"WNT-BC1 dosage-dependent"** dataset, detailed experimental condition included in `/Demo/Ratiometric_barcode_readout/WNT-BC1_recording_conditions_demo.csv/`. Only the first three fields of view (FOVs) of this condition included here. 

  - A **intensity measurement pipeline** is demostrated on the processed maximum intensity projection images and the corresponding segmentation masks for each channel. The **Ilastik pixel classification workflow** for barcode array spot segmentation is not included here.  
  
  *Note, the ratiometric barcode readout **raw data demo** and all the other **raw imaging data** are available upon request from the corresponding author.* 
