# COVID-19 Genomes and Phylogenetics

## Reference

Kandeel, Mahmoud, Maged E. M. Mohamed, Hany M. Abd El-Lateef, Katharigatta N.
Venugopala, Hossam S. El-Beltagi, “Omicron variant genome evolution and phylogenetics,”
Medical Virology 2022; 94:1627-1632. 

## Introduction

I will be reproducing the phylogenetic trees in Kandeel et. al. To achieve this, I will use data on COVID genomes collected by my lab and outside COVID genomes from
GISAID. Kandeel et. al. set out to establish a lineage and relationship between the then-emerging Omicron strain and other known variants at the time. To achieve this,
they used relatively simple methods to put forward a preliminary phylogeny that related Omicron to other strains sourced from a variety of geographic locations. The 
authors obtained all of their data through GISAID. The phylogenetic trees were created using simple methods to connect operational taxonomic units (OTUs) and to
estimate the evolutionary distance between nodes on the tree. The authors used both the UPGMA and Neighbor-Joining methods to make the trees, and used the Jukes-Cantor
substitution method and the Kimura 80 substitution method to estimate distances. All of these rely on simple algorithms to be calculated but lose a great amount of
nuance as a result.

## Figure to Reproduce

![Figures to Reproduce](https://i.imgur.com/OVo6aSL.png)

## Materials and Methods

I will be utilizing COVID-19 genomes which will be provided to me by my lab. I intend to also obtain genomes from geographic locations outside of North America to try
and create some inferences as to the region of origin of the genomes which were sequenced by my lab. I will use CLUSTAL to generate my alignments as it is the same 
software which the authors used and my lab has access to it. To generate the pairwise comparative matrices, I intend to use R, as it is the best tool for creating and 
analyzing spreadsheets of data and is the most easily scaled in comparison to something like Excel. I also want to learn how to use R as the majority of my statistics 
work has been in Excel and Python up to this point.

The phylogenetic trees will likely be created using Geneious or PhyML. My current goal is to utilize the same software which the authors used, including the  
generation of pairwise comparative matrices. To create the trees themselves, I intend to use the Neighbor Joining Method (NJM) and  Kimura 80 to estimate evolutionary 
distance between the nodes. I would like to try and hand-calculate either UPGMA or NJM to gain a better 
understanding of how these simpler algorithms actually work.

If I find that the alignments and creation of the trees take shorter than expected, I will consider incorporating more samples into my tree and using a more 
complicated method, such as a maximum likeliness method or a Bayesian method. I think that comparing the outcomes of a maximum likeliness method to the simplistic NJM
would be very interesting, but as I have absolutely no experience with any of these methods or software I do not want to get in over my head. 
