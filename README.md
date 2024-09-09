# Multiplexed detection of TF activity using prime TF reporters

## About
We previously identified prime TF reporters for 60 TFs: https://www.biorxiv.org/content/10.1101/2024.07.26.605239v1. These are essentially transcriptional barcoded reporters with validated TF-specificity. We cloned all of these prime reporters into a mini prime reporter library. This library has a low complexity (we have a library with 1 barcode/TF and a library with 5 barcodes/TF). This low complexity allows to recover TF activities from a small number of cells (e.g. 96-wells) or hard-to-transfect cells (e.g. organoids).

## Repository guide
- The ```barcode_preprocessing_prime_reporters.Rmd``` script contains the computation of the TF activities from the barcode counts and plotting of the TF activities. 
- The ```data/``` folder contains the scripts used for the raw data analysis: in these scripts barcodes are extracted from the fastq sequencing files and printed into a single .tsv file per sample. Moreover, a metadata file can be found in this folder that is needed for the ```barcode_preprocessing_prime_reporters.Rmd``` script.
- The ```library_design/``` folder contains the script used to generate the prime reporter sequences for the oligo library synthesis.
