# ChIPmentation_S.pombe_Snakemake
Snakemake-based pipeline for basic ChIPmentation analysis in S. pombe

Requires cutadapt, BWA, samtools (view, sort, index), deepTools (bamCoverage and bamCompare) $PATH (or modifiy Snakefile to indicate full path to tool)

To run the pipeline:

snakemake --snakefile STG_Snakefile_CT_Sp_2024 /working/dir/{sample1,sample2,sampleX}.bw

or

snakemake --snakefile STG_Snakefile_CT_Sp_2024 /working/dir/{sample1,sample2,sampleX}_fragments.bedgraph

# input file names should follow the pattern:

sample1_R1.fq.gz
sample1_R2.fq.gz

sample2_R1.fq.gz
sample2_R2.fq.gz

sampleX_R1.fq.gz
sampleX_R2.fq.gz
