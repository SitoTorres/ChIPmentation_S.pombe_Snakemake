# ChIPmentation_S.pombe_Snakemake

Snakemake-based pipeline for basic ChIPmentation analysis in S. pombe

Requires cutadapt, BWA, samtools (view, sort, index), deepTools (bamCoverage and bamCompare) to be in your $PATH (or modifiy Snakefile to indicate full path to tool)

To run the pipeline:

For individual input and IP bigwigs:

snakemake --snakefile STG_Snakefile_ChIPmentation_Sp_2024 /working/dir/{sample1,sample2,sampleX}_{input,IP}.bw

For normalised ratios IP/input:

snakemake --snakefile STG_Snakefile_ChIPmentation_Sp_2024 /working/dir/{sample1,sample2,sampleX}.bw

# input file names should follow the pattern:

sample1_input_R1.fq.gz
sample1_input_R2.fq.gz
sample1_IP_R1.fq.gz
sample1_IP_R2.fq.gz

sample2_input_R1.fq.gz
sample2_input_R2.fq.gz
sample2_IP_R1.fq.gz
sample2_IP_R2.fq.gz

sampleX_input_R1.fq.gz
sampleX_input_R2.fq.gz
sampleX_IP_R1.fq.gz
sampleX_IP_R2.fq.gz

