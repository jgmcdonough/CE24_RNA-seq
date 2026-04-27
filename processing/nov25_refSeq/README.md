# New Reference Genome
I recently discovered that a new *Crassostrea virginica* genome was released in November 2025 ([NCBI link](https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_053477285.1/)).

The biggest difference that I see chromosomal rearrangements and a reduction in duplications (from ~20% to 1.3%). These scripts serve to 1. re-align my sequences to the new reference and 2. compare the outputs from the two genomes.

### scripts:
- [processing_seqs.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/processing/nov25_refSeq/processing_seqs.ipynb): contains bash scripts used to align reads and generate a counts matrix
- [pipeline_counts.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/processing/nov25_refSeq/pipeline_counts.ipynb): generates a [csv](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/processing/qc_outputs/newRef_pipeline_counts.csv) to keep track of reads throughout the processing pipeline
- [compare_genomes.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/processing/nov25_refSeq/compare_genomes.ipynb): visualizes the differences in assignment and alignment rates in the old and new reference genome