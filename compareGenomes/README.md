# Compare Genomes
Recently, I realized a new reference genome was released for *Crassostrea virginca* at the end of 2025. This has led me down a rabbit hole to determine which genome I should be using for my analysis. In this, I found out about the [haplotig masked genome](https://urldefense.com/v3/__https:/github.com/The-Eastern-Oyster-Genome-Project/2023_Eastern_Oyster_Haplotig_Masked_Genome__;!!NcNAlj2UIVkjDA!6yx3IwtBB36qYgt7CqhfevvTw71M3RhSIHMclq6De6P3iKEJ2or40osj_OamQ33JkuS_tqVVTkZK-n_hOhOUw3u_EV4p$) from Dr. Jon Puritz at URI. 

To determine which genome I should use for analysis, I am going to align my sequences with both genomes, generate counts matrix, and compare annotations and outputs.

## [BUSCO](https://busco.ezlab.org/) analysis

- reference.masked.fast = **haplotig masked 2017 genome**
- GCF_053477285.1_ASM5347728v1_genomic.fna = **new 2025 genome**
- GCF_002022765.2_C_virginica-3.0_genomic.fna = **old 2017 genome**

![BUSCO plot](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/compareGenomes/busco_figure.png)

plot generated in [busco.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/compareGenomes/busco.ipynb)