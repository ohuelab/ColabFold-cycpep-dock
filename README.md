# ColabFold for Protein-CyclicPeptide Docking (WIP)

```diff
+ 12Jun2023: New databases! UniRef30 updated to 2302 and PDB to 230517.
+            We now use PDB100 instead of PDB70 (see notes in the [main](https://colabfold.com) notebook).
+ 12Jun2023: We introduced a new default pairing strategy:
+            Previously, for multimer predictions with more than 2 chains,
+            we only pair if all sequences taxonomically match ("complete" pairing).
+            The new default "greedy" strategy pairs any taxonomically matching subsets.
```

For details of what was changed in v1.5, see [change log](https://github.com/sokrypton/ColabFold/wiki/v1.5.0)!

<p align="center"><img src="https://github.com/sokrypton/ColabFold/raw/main/.github/ColabFold_Marv_Logo.png" height="250"/></p>

### Making Protein folding accessible to all via Google Colab!

| Notebooks | monomers | complexes | mmseqs2 | jackhmmer | templates   |
| :-------- | -------  | --------- | ------- | --------- | ----------- |
| [AlphaFold2_mmseqs2](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb) | Yes | Yes | Yes | No | Yes | 
| [AlphaFold2_batch](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/batch/AlphaFold2_batch.ipynb) | Yes | Yes | Yes | No | Yes | 
| [AlphaFold2](https://colab.research.google.com/github/deepmind/alphafold/blob/main/notebooks/AlphaFold.ipynb) (from Deepmind) | Yes | Yes | No | Yes | No | 
| [relax_amber](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/beta/relax_amber.ipynb) (relax input structure) | | | | | | 
| [ESMFold](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/ESMFold.ipynb) | Yes | Maybe | No | No| No |
||
| **BETA (in development) notebooks** | | | | | |
| [RoseTTAFold2](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/RoseTTAFold2.ipynb) | Yes | Yes | Yes | No | WIP | 
| [OmegaFold](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/beta/omegafold.ipynb) | Yes | Maybe | No | No| No |
||
| **OLD retired notebooks** | | | | | |
| [RoseTTAFold](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/RoseTTAFold.ipynb) | Yes | No | Yes | No | No | 
| [AlphaFold2_advanced](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/beta/AlphaFold2_advanced.ipynb) | Yes | Yes | Yes | Yes | No |
| [AlphaFold2_complexes](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/beta/AlphaFold2_complexes.ipynb) | No | Yes | No | No | No | 
| [AlphaFold2_jackhmmer](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/beta/AlphaFold_wJackhmmer.ipynb) | Yes | No | Yes | Yes | No |
| [AlphaFold2_noTemplates_noMD](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/verbose/alphafold_noTemplates_noMD.ipynb) |
| [AlphaFold2_noTemplates_yesMD](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/verbose/alphafold_noTemplates_yesMD.ipynb) |

