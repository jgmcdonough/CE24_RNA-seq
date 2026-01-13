# Phase 1 vs. Phase 1 Plots

## Plot Info

### DEGs
Visualizing and identifying DEGs in each pairwise comparison. Generated in [volcano_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/volcano_p1.v.p1.ipynb)
- **[vs.control_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase1_v_phase1/plots/vs.control_bar.pdf)**: barplots for number of up- and down-regulated DEGs in comparisons with control 
- **[vs.control_volcano.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/vs.control_volcano.pdf)**: volcano plots for comparisons with control
- **[vs.other_volcano.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/vs.other_volcano.pdf)**: volcano plots for comparisons outside of those against control
- **[all.comp_volcano.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/all.comp_volcano.pdf)**: grid of all volcano plots generated from comparing phase 1 oysters
- **[all.comparisons_upset.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/all.comparisons_upset.pdf)**: UpSet plot visualizing overlap of DEGs in *all* pairwise comparisons (generated in [venn_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/venn_p1.v.p1.ipynb))
    - [vs.cont_upset.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/vs.cont_upset.pdf): same as above, but only including comparisons with control conditions
    - [vs.other_upset.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/vs.other_upset.pdf): same as above, but only including comparisons outside of those against control conditions

### GOSlim Barplots
Visualizing the top 20 most abundant GOSlim terms for BP, MF, and CC for each pairwise comparison. Generated in [gene_ontology_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/gene_ontology_p1.v.p1.ipynb)
- **both vs. control**: [topGO.bc_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/topGO.bc_bar.pdf)
- **warm vs. control**: [topGO.wc_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/topGO.wc_bar.pdf)
- **hypoxic vs. control**: [topGO.hc_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/topGO.hc_bar.pdf)
- **hypoxic vs. both**: [topGO.hb_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/topGO.hb_bar.pdf)
- **warm vs. both**: [topGO.wb_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/topGO.wb_bar.pdf)
- **warm vs. hypoxic**: [topGO.wh_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/topGO.wh_bar.pdf)

### ORA Barplots
Are there any gene sets that are over-represented in the identified differential expressed genes (DEGs) than would be expected by chance? Generated in [gsea_p1.v.p1.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/gsea_p1.v.p1.ipynb)
#### All barplots:
includes results from all pairwise comparisons
- both vs. control: [ORA.bc_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.bc_bar.pdf)
- warm vs. control: [ORA.wc_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.wc_bar.pdf)
- hypoxic vs. control: [ORA.hc_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.hc_bar.pdf)
- hypoxic vs. both: [ORA.hb_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.hb_bar.pdf)
- warm vs. both: [ORA.wb_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.wb_bar.pdf)
- warm vs. hypoxic: [ORA.wh_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.wh_bar.pdf)
#### Directional barplots: 
same as above, but separated into up- and down-regulated DEGs (and only for comparisons with control treatment). 
- both vs. control: [ORA.bc.directional_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.bc.directional_bar.pdf)
- warm vs. control: [ORA.wc.directional_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.wc.directional_bar.pdf)
- hypoxic vs. control: [ORA.hc.directional_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/ORA.hc.directional_bar.pdf)

### TPM for Targeted Genes
transcript per million (TPM; controls for gene length and sequencing depth) for genes of interest
- HSP70: [hsp70.tpm_boxplot](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase1_v_phase1/plots/hsp70.tpm_boxplot.pdf)
