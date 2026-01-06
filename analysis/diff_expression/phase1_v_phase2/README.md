# Phase 1 vs. Phase 2
Analysis of oysters that only experienced phase 1 compared to those that additionally experienced phase 2

## Comparison Info
Investigating how GE changes *across ontogeny*
- C vs. CC
- W vs. WC
- H vs. HC
- B vs. BC

See the [phase2_v_phase2 directory](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2) to further investigate how GE changes across multiple exposures at two timepoints

## File Info
- [deseq_p1.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase2/deseq_p1.v.p2.ipynb) - using `DESeq2` to identify DEGs - outputs are located in [deseq_res_files](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase2/deseq_res_files)
- [volcano_p1.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase2/volcano_p1.v.p2.ipynb) - using `ggplot` to make volcano plots from DESeq2 results
- [venn_p1.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase2/venn_p1.v.p2.ipynb) - using `ggvenn` and `UpSetR` to identify unique/shared DEGs across pairwise comparisons
- [gene_ontology_p1.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase2/gene_ontology_p1.v.p2.ipynb) - using workflow from [Roberts lab](https://robertslab.github.io/resources/bio-Annotation/) to match GOslim terms to DEGs

## Plots
Plots generated from the above notebooks can be found [here](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase2/plots)