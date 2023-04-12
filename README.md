# SARS-CoV-2 Genomes and Phylogenetics

## Reference

Kandeel, Mahmoud, Maged E. M. Mohamed, Hany M. Abd El-Lateef, Katharigatta N.
Venugopala, Hossam S. El-Beltagi, “Omicron variant genome evolution and phylogenetics,”
Medical Virology 2022; 94:1627-1632. 

## Introduction

I will be reproducing the phylogenetic trees in Kandeel *et. al.* 2022. To achieve this, I will SARS-CoV-2 genomes obtained from the GISAID EPI-COV database. GISAID is a database of genome sequences compiled by labs all over the world to help research and combat emerging epidemics, and can be found at https://gisaid.org/. 

Kandeel et. al. set out to establish a lineage and relationship between the then-emerging Omicron strain and other known variants at the time. To achieve this, they used the UPGMA and Neighbor Joining methods to put forward a preliminary model that related Omicron to other strains sourced from a variety of geographic locations. The authors obtained all of their data through GISAID.

My goal was to re-assess their data utilizing Maximum Likelihood methods instead, and compare my results to theirs. To achieve this, I acquired a more geographically diverse array of sequences and increased the sample size from 8 to 401. The 8 samples used in Kandeel *et al* 2022 were included in my dataset.

## Figure to Reproduce

![Figures to Reproduce](https://i.imgur.com/OVo6aSL.png)

## Materials and Methods

### Data
I obtained all of my genomes from the aforementioned GISAID database. Due to the GISAID database's data sharing regulations, I cannot make the raw sequence data publicly available. RAxML identified 103 identical sequences in the alignment and these were removed for the final tree construction. The full list of EPI_ISL identifiers to download the .fasta sequences I utilized is provided in the ./Materials and Methods/ folder, along with the reduced list.

### Methods
I used Nextalign to generate my alignments as 401 genomes proved to be too computationally intensive for CLUSTAL to align. For the reference genome, I used the Wuhan Hu-1 sequence. This alignment was then used in RAxML to generate a tree using Bayesian Maximum Likelihood methods. The sequences were bootstrapped 100 times using the RAxML rapid bootstrap method. The output .tre file was acquired from RAxML and used in conjunction with FigTree to construct the phylogenetic tree.

## Figures
The branches and taxa names highlighted in red represent the sequences used by Kandeel *et. al.* 2022. A comparison of the two trees indicates that the Botswana Omicron sequence represented as an outgroup may not be accurate. 
![My Figure](https://i.imgur.com/BUwJkRn.jpg)
