# DESeq Results Files
## Phase 1 vs. Phase 1
All CSVs in this directory are generated from [deseq_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/deseq_p1.v.p1.ipynb). 

**Note**: The second listed pair in the filename is the 'baseline'

### [all_genes](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/deseq_res_files/all_genes)
Direct output from DESeq, contains information for all genes.

### [DEGs](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/deseq_res_files/DEGs)
Filtered CSVs in all_genes to include *only* DEGs (adjusted p-value < 0.05, |log2FoldChange| > 1). Code to do this can be found at the top of [volcano_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/volcano_p1.v.p1.ipynb)