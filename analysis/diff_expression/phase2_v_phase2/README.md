# Phase 2 vs. Phase 2
Analysis of oysters that experienced both phase 1 and phase 2

Jump to [File Info](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2#file-info)

## Comparison Info
Investigating **multiple stressors** across **two timepoints** in oysters

### Control Comparisons
#### 1. Effect of exposure after period of recovery
- CC vs. WC
- CC vs. HC
- CC vs. BC

#### 2. Effect of exposure only experienced later in life
- CC vs. CW
- CC vs. CH
- CC vs. CB

#### 3. Effect of timing of initial stress exposure
- CW vs. WC
- CH vs. HC
- CB vs. BC

#### 4. No stress vs. most stress
- CC vs. WW
- CC vs. HH
- CC vs. BB

#### 5. Effect of initial exposure on response in later exposure
**A. matched priming**
- WW vs. CW
- HH vs. CH
- BB vs. CB

**B. semi-matched priming: in context of later *single* stress**
- CH vs. BH
- CW vs. BW

**C. semi matched priming: in context of later *multiple* stress**
- CB vs. WB
- CB vs. HB

#### 6. Effect of initial exposure on subsequent response to stress
- WW vs. WC
- HH vs. HC
- BB vs. BC

### Interactions Between Stressors
#### 7. Effect of initial single/multiple stress on response in ...
>continuation of priming

**A. ...later *single* stress**
- BH vs. HH
- BW vs. WW

**B. ...later *multiple* stressors**
- HB vs. BB
- WB vs. BB

#### 8. Shared/unique responses among stressors with ...
**A. different *early* stressors**
>similar to [phase 1 vs. phase 1](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1), can check for long-term trends/GE
- WC vs. HC
- BC vs. HC
- BC vs. WC

**B. different *late* stressors**
- CW vs. CH
- CB vs. CH
- CW vs. CB

#### 9. Effect of order of stresses on GE
>Does the order of when stress is experienced matter? Maybe one stressor is an informative cue for a later environment?
- WH vs. HW
- WB vs. BW
- HB vs. BH

## File Info
- [deseq_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/deseq_p2.v.p2.ipynb) - using `DESeq2` to identify DEGs
      - outputs are located in [deseq_res_files](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/deseq_res_files)
- [volcano_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/deseq_p2.v.p2.ipynb) - using `ggplot` to make volcano plots from DESeq results
- [upset_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/upset_p2.v.p2.ipynb) - using `UpSetR` to identify unique/shared DEGs across pairwise comparisons
- [targetGenes_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/targetGenes_p2.v.p2.ipynb) - pulling out genes/pathways of interest and looking at DEGs and TPM

#### [gene_ontology](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology) directory
contains notebooks for gene ontology analysis:
- [goSlim_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology/goSlim_p2.v.p2.ipynb) - using workflow from [Roberts Lab](https://robertslab.github.io/resources/bio-Annotation/) to match GOSlim terms to DEGs
- [gsea_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology/gsea_p2.v.p2.ipynb) - using `gsea` from `clusterProfiler` to identify enriched GO terms via gene set enrichment analysis
- [ora_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology/ora_p2.v.p2.ipynb) - using `enricher` from `clusterProfiler` to do over-represented analysis and identify enriched GO terms
- [kegg_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology/kegg_p2.v.p2.ipynb) - using `gseKEGG` to identify enriched pathways

#### [frontloading](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/frontloading) directory
contains notebooks for identifying transcriptional frontloading
- [frontloading_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/frontloading/frontloading_p2.v.p2.ipynb) - following workflow from Gurr et al., 2022
- [collins_frontloading.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/frontloading/collins_frontloading.ipynb) - following workflow from Collins et al, 2021

#### [WGCNA](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/wgcna) directory
contains notebooks for weight gene co-expression network analysis
- [wgcna_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/wgcna_p2.v.p2.ipynb) - weighted gene co-expression network analysis following [Gurr script](https://github.com/SamGurr/Pgenerosa_OA_TagSeq/blob/main/TagSeq/Analysis/Scripts/Day0_WGCNA_all.R) and using `WGCNA`


## Plots
Plots generated from the above notebooks can be found [here](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/plots)

  