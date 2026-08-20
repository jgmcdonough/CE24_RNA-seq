# Gene Ontology
Directory containing various gene ontology analyses.

## Scripts
- [goSlim_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology/goSlim_p2.v.p2.ipynb) - matching gene IDs to broader gene ontology categories (goSlim)
- [gsea_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology/gsea_p2.v.p2.ipynb) - gene set enrichment analysis (provide list of all genes, ordered by log fold change)
    - are there some pathways/gene sets that are enriched (grouped higher/lower more than expected)
- [ora_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology/ora_p2.v.p2.ipynb) - over-representation analysis (provide list of DEGs and background/universal gene list)
    - are there gene sets that are over-represented in your list of interest, more than expected
- [kehh_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/gene_ontology/kegg_p2.v.p2.ipynb) - KEGG enrichment analysis (provide list of all genes, ordered by log fold change)