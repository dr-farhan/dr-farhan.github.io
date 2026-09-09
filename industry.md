---
layout: page
title: "Research Software"
subtitle: "Public workflows for single-cell analysis and repeat genomics"
css:
  - "/css/profile.css"
---

<section markdown="1" class="profile-section compact-top">
These public repositories document the inputs, methods, and outputs of my computational workflows. They combine established bioinformatics tools with analysis organization and reporting for specific research questions.
</section>

<section markdown="1" class="profile-section research-case" id="leukemia-projection">
<p class="entry-meta">R · Python · Snakemake · Single-cell RNA-seq</p>

## Reference-guided leukemia projection

**Purpose.** Map leukemia single-cell profiles onto the healthy BoneMarrowMap reference to examine lineage relationships.

**Implementation.** A modular workflow organizes reference projection, mapping quality checks, lineage annotation, pseudotime transfer, native clustering, and reporting. It builds on BoneMarrowMap, Symphony, and Seurat, with attribution in the repository.

**Inputs → outputs.** Raw-count Seurat objects → annotated Seurat objects, per-cell and cluster tables, PDF/PNG figures, logs, and recorded configuration.

**Reproducibility.** Installation instructions, an R dependency lockfile, preflight checks, local/LSF profiles, and automated configuration and syntax checks are included. A public-dataset configuration is available; input data and reference assets are obtained separately.

[Source & quick start](https://github.com/dr-farhan/Reference-guided-scRNA-seq-Leukemia-Projection) · [Installation](https://github.com/dr-farhan/Reference-guided-scRNA-seq-Leukemia-Projection/blob/main/INSTALL.md) · [Example dataset configuration](https://github.com/dr-farhan/Reference-guided-scRNA-seq-Leukemia-Projection/blob/main/config/gse223844.yaml) · [Output guide](https://github.com/dr-farhan/Reference-guided-scRNA-seq-Leukemia-Projection#results)
</section>

<section markdown="1" class="profile-section research-case" id="te-expression">
<p class="entry-meta">Snakemake · RNA-seq · TE quantification</p>

## TE family and locus expression

**Purpose.** Quantify transposable-element expression at both family and individual-locus resolution across samples.

**Implementation.** A Snakemake workflow runs the established TEcount and TElocal tools and collects per-sample results into count matrices.

**Inputs → outputs.** Coordinate-sorted RNA-seq BAM files, a sample sheet, and compatible gene/TE annotations → family- and locus-level count matrices with retained per-sample tables.

**Reproducibility.** The repository includes a Conda environment, sample-sheet template, configurable annotation paths, and dry-run instructions. Users supply sequencing files and compatible annotations.

[Source & run instructions](https://github.com/dr-farhan/TE-family-and-locus-expression-analysis-using-TEtranscript) · [Sample-sheet template](https://github.com/dr-farhan/TE-family-and-locus-expression-analysis-using-TEtranscript/blob/main/config/samples.tsv) · [Environment](https://github.com/dr-farhan/TE-family-and-locus-expression-analysis-using-TEtranscript/blob/main/envs/te-transcripts.yaml)
</section>

<section markdown="1" class="profile-section research-case" id="cpg-density">
<p class="entry-meta">Python · BEDTools · Genomic sequence annotation</p>

## CpG density of genomic intervals

**Purpose.** Characterize the CpG composition of TE loci or other genomic regions.

**Implementation.** A Python script uses pybedtools/BEDTools to extract reference-sequence composition and calculate CpG per base, CpG per C/G base, and the CpG observed/expected ratio.

**Inputs → outputs.** A reference FASTA and three-column BED intervals → three BED-like metric files. These are sequence-composition measurements, not measurements of DNA methylation.

**Reproducibility.** The README specifies formulas, dependencies, coordinate conventions, undefined-value handling, and output examples. Small FASTA/BED test fixtures and tests are included.

[Source & usage](https://github.com/dr-farhan/TE_CpG_density) · [Example inputs](https://github.com/dr-farhan/TE_CpG_density/tree/main/tests/fixtures) · [Output examples](https://github.com/dr-farhan/TE_CpG_density#usage) · [Tests](https://github.com/dr-farhan/TE_CpG_density/blob/main/tests/test_annotate_cpg_density.py)
</section>

<section markdown="1" class="profile-section">
[View all public repositories](https://github.com/dr-farhan?tab=repositories) · [Discuss a collaboration]({{ site.baseurl }}/contact)
</section>
