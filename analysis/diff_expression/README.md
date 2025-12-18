# Differential Expression Analysis
differentially expressed genes identified with [`DESeq2`](https://bioconductor.org/packages/release/bioc/vignettes/DESeq2/inst/doc/DESeq2.html)

### Phase 1 Comparisons ([dir](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1))
Comparing oysters that only experienced phase 1 - looking at the effect of a treatment at ***one timepoint***
- DESeq analysis [code](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/deseq_phase1.v.phase1.ipynb)
- output CSVs in [deseq_res_files](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/deseq_res_files)

### Phase 1 to Phase 2 Comparisons ([dir](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase2))
Comparing oysters that only experienced phase 1 to those that experienced phase 1 *and* 2 - changes in gene expression ***over time*** (from treatment at one timepoint to at two timepoints)

### Phase 2 ([dir](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2))
Comparing oysters that experienced both phase 1 and phase 2 - looking at the effect of an early environment on gene expression in a later evironment - ***two timepoints***