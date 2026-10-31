# PRJNA1002351: Microplastic-associated microbiome reanalysis

Computational reanalysis of publicly available 16S rRNA sequencing data from NCBI BioProject **PRJNA1002351** (SRA Study **SRP453394**).

## Manuscript

**Microbial Community Structure in Microplastic-Associated Biofilms: A Computational Reanalysis of Publicly Available 16S rRNA Data**

This repository accompanies a single-BioProject reanalysis comparing DNA-derived and RNA-derived 16S rRNA profiles. DNA/RNA status is interpreted as a proxy for total versus more transcriptionally active community membership, not as a direct measurement of activity. The analysis does not establish polymer-specific effects or causal effects of plastic exposure.

## Data source

- NCBI BioProject: [PRJNA1002351](https://www.ncbi.nlm.nih.gov/bioproject/PRJNA1002351)
- SRA Study: [SRP453394](https://www.ncbi.nlm.nih.gov/sra/?term=SRP453394)
- Original study: Garrison et al. (2024), *Environmental Microbiology*. [https://doi.org/10.1111/1462-2920.16563](https://doi.org/10.1111/1462-2920.16563)

## Computational workflow

Sequence processing used QIIME 2 / q2-dada2 (2026.1.0), with quality-guided paired-end denoising, chimera removal, representative-sequence generation, and taxonomic classification against SILVA 138. Downstream analyses included alpha diversity, Bray–Curtis beta diversity and ordination, PERMANOVA/PERMDISP, and an exploratory genus-level CLR/Wilcoxon screen.

Key DADA2 settings included forward truncation at 260 bp, reverse truncation at 180 bp, maximum expected errors of 2 for each read, minimum overlap of 12 bp, and consensus chimera removal. Full parameters and provenance are intended to accompany the supplementary files.

## Supplementary materials

The supplementary package is being prepared for deposit in this repository. Planned contents include:

- Sample/accession metadata crosswalk
- Per-sample DADA2 denoising statistics
- Taxonomy assignments
- Genus-level differential-abundance results
- Feature table and representative sequences
- QIIME 2 provenance and environment information
- Supplementary methods and a file manifest

## Reproducibility and interpretation

The genus-level DNA/RNA comparison is exploratory and was not adjusted for collection date. A date-restricted community-level PERMANOVA was conducted using samples from collection dates containing both DNA and RNA groups. Results should be interpreted in light of the metadata limitations and small effect sizes.

## Citation

Please cite the associated manuscript and the original dataset publication. A persistent DOI will be added here after Zenodo archival is completed.

## Deposit status

The repository has been created. Supplementary files and the Zenodo DOI have not yet been deposited or assigned.
