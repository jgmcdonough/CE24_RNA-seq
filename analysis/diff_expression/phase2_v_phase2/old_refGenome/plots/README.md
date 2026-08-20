# Phase 2 vs. Phase 2 Plots
## Plot Info

Plots related to WGCNA can be found in a [different plot directory](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/wgcna/plots)

### DEGs
Visualizing and identifying DEGs in each pairwise comparison. Generated in [volcano_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/volcano_p2.v.p2.ipynb).
#### Volcano plots
1. Effect of single exposure after a period of recovery: [comp1_volcano.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/comp1_volcano.pdf)
2. Effect pf single exposure only experienced later in life: [comp2_volcano.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/comp2_volcano.pdf)

#### UpSet plots
Shared/unique DEGs when comparing timing/repeated exposure to the same stressor against control (CC) oysters:
>ex: comparing CC vs. WC, CW, WW
- Warming: [warming_upset.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/warming_upset.pdf)
- Hypoxia: [hypoxia_upset.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/hypoxia_upset.pdf)
- Both warming and hypoxia: [both_upset.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/both_upset.pdf)

### Frontloaded Genes
Stress-inducible genes that are frontloaded in 'primed' oysters and have a reduced reaction upon a subsequent stress exposure. Generated in [vst_frontloading.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/frontloading/vst_frontloading.ipynb)
#### up-regulated frontloaded genes
- Warming: [warmUp_frontloadedGenes.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/warmUp_frontloadedGenes.pdf)
- Hypoxia: [hypoxicUp_frontloadedGenes.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/hypoxicUp_frontloadedGenes.pdf)
- Both: [bothUp_frontloadedGenes.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/bothUp_frontloadedGenes.pdf)


### Other Plots
- [chitin.genes_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/chitin.genes_bar.pdf) - DEGs that are associated with GO terms related to **chitin** (chitin synthase activity, chitinase activity, chitin binding)
- [chitin.genesDETAILED_bar.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/chitin.genesDETAILED_bar.pdf) - same as above, but bars are split and labeled for which treatment has the higher expression for those genes
- [hsp70_normExpr_boxplot.pdf](https://github.com/jgmcdonough/CE24_RNA-seq/tree/main/analysis/diff_expression/phase2_v_phase2/plots/hsp70_normExpr_boxplot.pdf) - boxplot of normalized expression for each treatment combo for the HSP70 gene
