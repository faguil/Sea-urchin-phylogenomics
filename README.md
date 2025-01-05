# Phylogenomic analyses of echinoid diversification prompt a re-evaluation of their fossil record - Supplementary Data

This GitHub repository provides the supplementary data referenced in the publication cited below.

## How to use and cite these files 

All files are publicly available and can be used for further research or other applications. However, if you utilize these resources in your work, we kindly request that you cite our original publication.

**Phylogenomic analyses of echinoid diversification prompt a re-evaluation of their fossil record.** Nicolás Mongiardino Koch, Jeffrey R Thompson, Avery S Hiley, Marina F McCowin, A Frances Armstrong, Simon E Coppard, Felipe Aguilera, Omri Bronstein, Andreas Kroh, Rich Mooi, Greg W Rouse. *eLife* **11**:e72460 (2022). https://elifesciences.org/articles/72460

**Abstract**

Echinoids are key components of modern marine ecosystems. Despite a remarkable fossil record, the emergence of their crown group is documented by few specimens of unclear affinities, rendering their early history uncertain. The origin of sand dollars, one of its most distinctive clades, is also unclear due to an unstable phylogenetic context. We employ 18 novel genomes and transcriptomes to build a phylogenomic dataset with a near-complete sampling of major lineages. With it, we revise the phylogeny and divergence times of echinoids, and place their history within the broader context of echinoderm evolution. We also introduce the concept of a chronospace – a multidimensional representation of node ages – and use it to explore methodological decisions involved in time calibrating phylogenies. We find the choice of clock model to have the strongest impact on divergence times, while the use of site-heterogeneous models and alternative node prior distributions show minimal effects. The choice of loci has an intermediate impact, affecting mostly deep Paleozoic nodes, for which clock-like genes recover dates more congruent with fossil evidence. Our results reveal that crown group echinoids originated in the Permian and diversified rapidly in the Triassic, despite the relative lack of fossil evidence for this early diversification. We also clarify the relationships between sand dollars and their close relatives and confidently date their origins to the Cretaceous, implying ghost ranges spanning approximately 50 million years, a remarkable discrepancy with their rich fossil record.

## Author contact

- [Nicolás Mongiardino Koch](mailto:nmongiardinokoch@ucsd.edu) (corresponding author)
- [Felipe Aguilera](mailto:f.aguilera@uq.edu.au) (senior author - Assistant Professor)

## How to download data files

The files in this repository are ready for use. Simply click on the file, and you will be directed to the GitHub webpage to save it to your device.

## Index of data file contents

[01-Assemblies.tar.gz](https://drive.google.com/file/d/1ninmuyKmNu6Kf_nB9Imal9HSXnqDm-Na/view?usp=sharing) contains the genomic or transcriptomic assemblies (as gzipped fasta files), for all 66 terminals used to build the supermatrix and phylogenies on which this manuscript is based. SRA for the raw read files can be found in the manuscript.

[02-Chronospaces.tar.gz](https://drive.google.com/file/d/1FKM-gZE9ttfcni8fmoDNr7srl_34vBFS/view?usp=sharing) contains consensus and posterior topologies obtained from the 80 time-calibrated runs performed using PhyloBayes, and used to build chronospaces (all files are in Newick format). Posterior topologies can be uploaded and analyzed in R using the accompanying R code. Consensus trees can be visualized using FigTree. Files are organized in nested folders that specify the conditions under which the time-calibrated runs were performed using:

- Cauchy/uniform: refers to the type of prior distribution enforced on calibrated nodes.
- LN/UGAM: refers to the type of clock enforced (LN: autocorrelated log-normal; UGAM: uncorrelated gamma)
- CATGTR/GTR: refers to the model of molecular evolution applied (CARGTR: site-heterogeneous; GTR: site-homogeneous; both unpartitioned)

Within each of these folders the files corresponding to the all conditions of the fourth factor tested, i.e. the loci sampling strategy, can be found (with five conditions: clock/occupancy/random/signal/usefulness).

[03-Phylogenomics_dataset.tar.gz](https://github.com/faguil/Sea-urchin-phylogenomics/blob/main/Phylogenomic_datasets.tar.gz) contains the supermatrices and partition files of the phylogenomic datasets used for tree inference (i.e., the full matrix as well as those subsampled to 100 and 500 loci using genesort.R. Matrices are provided in fasta format, and partition files follow RAxML style.
