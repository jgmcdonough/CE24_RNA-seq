# CE24_RNA-seq

Repository for *Crassostrea virginica* gill tissue RNA-seq processing and analysis for the Caryover Effects ORCC 2024 Project 
  >Sample and extraction information is stored on [this repo](https://github.com/GWLab-UML/CE_ORCC/tree/main/2024/genetics)


## Sample Name Code
| Treatment    | Temperature | Dissolved Oxygen |
| -------- | ------- | ------- |
| Control | ambient | normoxic |
| Both  | warm    | hypoxic |
| Hypoxic | ambient     | hypoxic |
| Warm    | warm    | normoxic

also see [sample_metaData.csv](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/sample_metaData.csv) for more detailed sample treatment information.

## Repo Contents
- ### [processing](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/processing): raw sequences to analysis-ready
    - [pipeline_counts.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/processing/pipeline_counts.ipynb): code to keep track of reads at each step of workflow
    - [processing_seqs.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/processing/processing_seqs.ipynb): code to process raw seqs from trimming to generating counts matrix as input for DESeq2
    - [qc_outputs](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/processing/qc_outputs): directory containing outputs from processing_seqs.ipynb and novogene
  

- ### [analysis](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis): differential expression and alternative splicing

    - #### [diff_expression](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression): directory for code, outputs, and plots for differential expression
        - [phase1_v_phase1](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1): comparisons of oysters that only experienced phase 1
    - #### [alt_splicing](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/alt_splicing): directory for code, outputs, and plots for alternative splicing


