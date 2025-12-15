# Processing
This directory contains scripts to process raw sequences prior to analysis and pipeline counts.


Total RNA was sent to Novogene for library preparation (poly A enrichment) and sequenced on NovaSeq X Plus Series (PE150, 30M depth).


### [processing_seqs.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/processing/processing_seqs.ipynb)
- includes scripts to process sequences using [`trim-galore`](https://github.com/FelixKrueger/TrimGalore), [`fastQC`](https://www.bioinformatics.babraham.ac.uk/projects/fastqc/), [`hisat2`](https://daehwankimlab.github.io/hisat2/), [`samtools`](https://www.htslib.org/doc/samtools-view.html), and [`featureCounts`](https://subread.sourceforge.net/featureCounts.html)

### [pipeline_counts.ipynb](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/processing/pipeline_counts.ipynb)
- script to keep track of number of reads at each step of workflow

### [qc_outputs](https://github.com/jgmcdonough/CE24_RNA-seq/blob/main/processing/qc_outputs)
- directory for storing code outputs (multiqc html report, novogene qc summary, etc.)