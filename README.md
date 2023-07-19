# ColabFold for Protein-CyclicPeptide Docking (WIP)

This repository is based on the ColabFold on [GitHub](https://github.com/sokrypton/ColabFold/tree/main).

## Protein-Cyclic Peptide Complex Prediction

### Google Colab

<a href="https://colab.research.google.com/github/ohuelab/ColabFold-cycpep-dock/blob/colab/AlphaFold2-cycpep-dock.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

### How do I predict protein-cyclic peptide complexes?

The same input format can be used as when predicting complexes with ColabFold. However, you can predict protein-cyclic peptide complexes by using the target protein sequence as input before ":" and the cyclic peptide sequence after ":" as in TARGETPROTEINSEQ:CYCLICPEPTIDESEQ and check the set_cyclic option.

### PDB structures included in AlphaFold training dataset

AlphaFold training dataset has not been processed to remove cyclic peptides, but there is a cutoff based on the number of amino acid residues. In the latest version of the alphafold2_multimer_v3 model training set, peptides less than 4 amino acid residues were excluded. However,　the alphafold2_ptm model and the alphafold2_multimer_v2 model training set, peptides less than 16 amino acid residues were excluded (confirmed with the AlphaFold Team at DeepMind). 

| moldels | Length of residues | Released date for PDB structures |
| :--------: | :--------: | :--------: |
| alphafold2_ptm | 16 or more residues| before 2018-04-30 |
| alphafold2_multimer_v1 | 16 or more residues | before 2018-04-30 |
| alphafold2_multimer_v2 | 16 or more residues | before 2018-04-30 |
| alphafold2_multimer_v3 | **4 or more residues** | **before 2021-09-30** |
