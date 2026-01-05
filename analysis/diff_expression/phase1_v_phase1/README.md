# Phase 1 vs. Phase 1 
Analysis of oysters that only experienced phase 1 

## Comparison Info
Investigating the difference between each environmental stressor at a **single timepoint** in oysters that are naive to prior stress
- **W/H vs. C** - effect of single stress 
- **B vs. C** - effect of simultaneous stressors 
- **W/H vs. B** - effect of single vs. simultaneous stressors (when one of the stressors is shared)
- **W vs. H** - effect of different single stressors

## File Info
- [deseq_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/deseq_p1.v.p1.ipynb) - using `DESeq2` to identify DEGs
      - outputs are located in [deseq_res_files](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1/deseq_res_files)
- [volcano_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/volcano_p1.v.p1.ipynb) - using `ggplot` to make volcano plots from DESeq2 results
- [venn_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/venn_p1.v.p1.ipynb) - using `ggvenn` and `UpSetR` to identify unique/shared DEGs across pairwise comparisons
- [gsea_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/gsea_p1.v.p1.ipynb) - using `gsea` and `enricher` from `clusterProfiler` to do GSEA and ORA analyses
- [gene_ontology_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/gene_ontology_p1.v.p1.ipynb) - using workflow from [Roberts lab](https://robertslab.github.io/resources/bio-Annotation/) to match GOslim terms to DEGs
- [kegg_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/kegg_p1.v.p1.ipynb) - using `enrichKEGG` from `clusterProfiler` to do KEGG enrichment analyses

## Plots
Plots generated from the above notebooks can be found [here](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1/plots)