# Phase 1 vs. Phase 1 
Analysis of oysters that only experienced phase 1 

## Comparison Info
- **Warm/Hypoxic vs. Control** - effect of single stress at one timepoint
- **Both vs. Control** - effect of multi stressors at one timepoint
- **Warm/Hypoxic vs. Both** - effect of single vs. multi stressors at one timepoint (when one of the stressors is shared)
- **Warm vs. Hypoxic** - effect of different single stressors at one timepoint (shared/unique responses to single stressor)

## File Info
- [deseq_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/deseq_p1.v.p1.ipynb) - using `DESeq2` to identify DEGs
- [volcano_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/volcano_p1.v.p1.ipynb) - using `ggplot` to make volcano plots from DESeq2 results
- [venn_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/gsea_p1.v.p1.ipynb) - using `ggvenn` and `UpSetR` to identify unique/shared DEGs across pairwise comparisons
- [gsea_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/venn_p1.v.p1.ipynb) - using `gsea()` and `enricher` from clusterProfiler to do GSEA and ORA analyses
- [gene_ontology](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/gene_ontology_p1.v.p1.ipynb) - using workflow from [Roberts lab](https://robertslab.github.io/resources/bio-Annotation/) to match GOslim terms to DEGs 
- [deseq_res_files](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1/deseq_res_files) - output CSVs from DESeq2 results