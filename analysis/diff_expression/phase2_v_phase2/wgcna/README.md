# WGCNA
weighted gene co-expression network

used to identify modules of highly correlated genes, relate them to sample traits, and find hub genes that are functionally related

**Idea**: genes with similar expression patterns are functionally associated - part of the same complexes, involved in the same pathway, influence each other
> gene regulatory network: gene 1 influences the expression of gene 2 which influences the expression of gene 3 ...

### Inputs:
- gene expression matrix - I'm using vst expression generated from `DESeq2`
    - [vst expression](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/deseq_rawLFC/deseq_vstCounts.csv) generated in [deseq_p2.v.p2.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/analysis/diff_expression/phase2_v_phase2/deseq_p2.v.p2.ipynb)
- meta data - [treatment information](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/metaData/sample_metaData.csv) and [growth data](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/metaData/growth_phase2.1_weights.csv)

### Detailed workflow:
1. build correlation matrix from *normalized* gene expression matrix
    - measures the relationship/connection between two variables
    - can be *signed* or *unsigned*
        - **unsigned** = values are abs. values of correlation - make biological interpretation difficult bc you do not know regulation direction
        - **signed** = sign of correlation values are considered - takes into account up- or down-regulation
4. create weighted adjacency matrix - highlight the important connections and reduce noise by applying threshold
    - **soft** threshold - weighted network - use correlation values and raise to a power term (stronger connections are emphasized, weaker are suppressed)
    - **hard** threshold - unweighted network - sensitive to threshold bc results in loss of co-expr. information (doesn't tell you how strong/weak the connection is)
6. hierarchical clustering using proximity measure to identify modules
    - topological overlap measure (TOM) similarity matrix - if two genes have high similarity, it will have high TOM and low dissimilarity
    - then generate TOM dissimilarity matrix - distance of a gene from every other gene in the system
    - this is used to create gene dendogram
8. identify clusters of genes with similar expression patterns (modules)
    - merge modules with similar co-expression profiles into more meaningful modules
9. downstream analysis
    - correlate modules with phenotypes/traits - create graphical representations for module-trait relationships
    - identify driver genes in the module correlated with the phenotype/trait of interest
        - look at intramodular connectivity (how well the node is connected within its assigned module) or module membership - look for genes with expression that is highly correlated with the module eigengene
     

#### Resources used:
- [Bioinformagician YouTube videos](https://www.youtube.com/watch?v=BzYfg1lO3jw)
- [Gurr et al 2021 code notebook](http://github.com/SamGurr/Pgenerosa_OA_TagSeq/blob/main/TagSeq/Analysis/Scripts/Day21_WGCNA_all.R)
- [Hovrath Tutorial Dropbox](https://www.dropbox.com/scl/fo/4vqfiysan6rlurfo2pbnk/h?dl=0&e=2&rlkey=thqg8wlpdn4spu3ihjuc1kmlu)