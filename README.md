# CE24_RNA-seq

Repository for *Crassostrea virginica* gill tissue RNA-seq processing and analysis for the Caryover Effects ORCC 2024 Project 
  >Sample and extraction information is stored on [this repo](https://github.com/GWLab-UML/CE_ORCC/tree/main/2024/genetics)


## Sample Name Code
| Treatment    | Code| Temperature | Dissolved Oxygen |
| -------- | ---|---- | ------- |
| Control | C|ambient | normoxic |
| Both  | B|warm    | hypoxic |
| Hypoxic | H|ambient     | hypoxic |
| Warm    | W|warm    | normoxic

also see [sample_metaData.csv](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/metaData/sample_metaData.csv) for more detailed sample treatment information.

## Repo Contents
- ### [metaData](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/metaData): treatment info and growth
    - [sample_metaData.csv](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/metaData/sample_metaData.csv): contains information on treatment exposures and tank replicates for phase 1 and phase 2
    - [growth_phase1_weights.csv](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/metaData/growth_phase1_weights.csv): weights for oysters after phase 1
    - [growth_phase2.1_weights.csv](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/metaData/growth_phase2.1_weights.csv): weights for oysters after phase 2
      >both growth CSVs come from [CE_ORCC project repo](https://github.com/GWLab-UML/CE_ORCC/tree/main/2024/oyster_data)

- ### [processing](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/processing): raw sequences to analysis-ready
    - [pipeline_counts.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/processing/pipeline_counts.ipynb): code to keep track of reads at each step of workflow
    - [processing_seqs.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/processing/processing_seqs.ipynb): code to process raw seqs from trimming to generating counts matrix as input for DESeq2
    - [qc_outputs](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/processing/qc_outputs): directory containing outputs from processing_seqs.ipynb and novogene
  

- ### [analysis](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis): code and outputs for various analyses, organized into 6 folders
    - alternative splicing
    - differential expression
    - growth
    - methylation toolkit
    - perkinsus
    - variant calling

- ### [compareGenomes](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/compareGenomes): compare the new and old genome releases
    - a new *C. virginica* reference genome was released in November 2025 - directory includes comparisons of the old (2017) genome, haplotig-masked genome, and new (2025) genome

