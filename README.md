# Genomic Characterisation of *M. tuberculosis* Sub-lineage L4.11

This repository contains the manuscript source files for:

> **Genomic characterisation of *Mycobacterium tuberculosis* sub-lineage 4.11: two geographically distinct clades with convergent drug resistance and metabolic signatures**
>
> Christophe Guyeux et al.

## Repository Structure

```
.
├── main.tex                    # Main manuscript (LaTeX)
├── table_bioprojects.tex       # BioProjects table (included by main.tex)
├── Makefile                    # Build instructions
├── figures/                    # All manuscript figures (PDF + PNG)
│   ├── fig1_l4_phylogeny.*     # Figure 1: L4 context tree
│   ├── fig2_geographic_distribution.*  # Figure 2: Geographic map
│   ├── fig3_molecular_clock.*  # Figure 3: TreeTime clock
│   ├── phylo_tree_l411.*       # L4.11 phylogenetic tree
│   └── ...                     # Additional figures
├── supplementary_materials/    # Supplementary data files
│   ├── S1_phylogenetic_tree.nwk  # Newick tree
│   └── S2_strain_list.csv     # Complete strain metadata
├── .gitignore
└── README.md
```

## Building the manuscript

```bash
make          # Compile with pdflatex + bibtex
make clean    # Remove auxiliary files
```

Or manually:
```bash
pdflatex main.tex
pdflatex main.tex   # Second pass for references
```

## Overleaf

This repository is designed to be imported directly into [Overleaf](https://www.overleaf.com/) for collaborative editing:

1. In Overleaf, go to **New Project → Import from GitHub**
2. Select `cguyeux/article-L4.11`
3. The project will sync bidirectionally with this repository

## Data Availability

Raw sequencing data are available from the NCBI Sequence Read Archive (SRA) under the BioProject accessions listed in Table S2. Analysis scripts and intermediate results are maintained in a separate internal repository.

## License

This work is shared for review purposes. © 2026 Christophe Guyeux, Univ. Bourgogne Franche-Comté.
