# Phase 2 vs. Phase 2 using the [new reference genome](https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_053477285.1/)
This folder contains the same analyses as [phase2_v_phase2](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2), but using the new reference genome.

## File Info
- [deseq_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/deseq_p2.v.p2.ipynb) - using `DESeq2` to identify DEGs - outputs are located in [deseq_res](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/deseq_res) (all outputs and just DEGs)
- [volcano_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/volcano_p2.v.p2.ipynb) - using `ggplot2` to make volcano plots from DESeq results
- [upset_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/upset_p2.v.p2.ipynb) - using `UpSetR` to identify unique and shared DEGs across pairwise comparisons
- [targetGenes_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/targetGenes_p2.v.p2.ipynb) - pulling out genes and pathways of interest and looking at DEGs/TPM/VST
- [gsea_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/gsea_p2.v.p2.ipynb) - using `GSEA` from the `clusterProfiler` package to identify enriched GO terms in pairwise comparisons

#### [WGCNA](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/wgcna) directory
contains notebooks, CSVs, and plots for weighted gene co-expression network analysis
- [newRef_wgcna_p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/wgcna/newRef_wgcna_p2.ipynb) - WGCNA following [Gurr script](https://github.com/SamGurr/Pgenerosa_OA_TagSeq/blob/main/TagSeq/Analysis/Scripts/Day0_WGCNA_all.R) and using `WGCNA`
- [GO_wgcna_p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/wgcna/GO_wgcna_p2.ipynb) - over-representation analysis using `enricher` from the `clusterProfiler` package to identify enriched GO terms
- [ouputs](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/wgcna/outputs) directory - contains CSVs from WGCNA analyses
- [plots](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/new_refGenome/wgcna/plots) directory - contains .png from WGCA analyses