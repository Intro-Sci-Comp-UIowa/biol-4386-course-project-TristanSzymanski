# COVID-19 Genomes and Phylogenetics

## Reference

Kandeel, Mahmoud, Maged E. M. Mohamed, Hany M. Abd El-Lateef, Katharigatta N.
Venugopala, Hossam S. El-Beltagi, “Omicron variant genome evolution and phylogenetics,”
Medical Virology 2022; 94:1627-1632. 

## Introduction

I will be reproducing the phylogenetic trees in Kandeel et. al. To achieve this, I will use data on COVID genomes collected by my lab and outside COVID genomes from
the GISAID database. GISAID is a database of genome sequences compiled by labs all over the world to help research and combat emerging epidemics.  Kandeel et. al. set 
out to establish a lineage and relationship between the then-emerging Omicron strain and other known variants at the time. To achieve this, they used relatively simple 
methods to put forward a preliminary model that related Omicron to other strains sourced from a variety of geographic locations. The authors obtained all of their data 
through GISAID. The phylogenetic trees were created using simple methods to connect operational taxonomic units (OTUs) and to estimate the evolutionary distance 
between nodes on the tree. The authors used both the UPGMA and Neighbor-Joining methods to make the trees. To estimate distance, they used the Jukes-Cantor 
substitution method and the Kimura 80 substitution method to estimate distances, which use the fixed rate of transitions and transversions occurring in DNA to evaluate 
how much time has passed between two sequences. All of these rely on simple algorithms to be calculated and lose a great amount of nuance as a result.

## Figure to Reproduce

![Figures to Reproduce](https://i.imgur.com/OVo6aSL.png)

## Materials and Methods

I obtained all of my genomes from the aforementioned GISAID database. I will use CLUSTAL to generate my alignments as it is the same  software which the authors used 
and my lab has access to it. To generate the pairwise comparative matrices which are required for the relatedness models I am using, I intend to use R.

The phylogenetic trees will likely be created using Geneious or PhyML. My current goal is to utilize the same software which the authors used, including the  
generation of pairwise comparative matrices. To create the trees themselves, I intend to use the Neighbor Joining Method (NJM) and  Kimura 80 to estimate evolutionary 
distance between the nodes. I would like to try and hand-calculate either UPGMA or NJM to gain a better understanding of how these simpler algorithms actually work.

If I find that the alignments and creation of the trees take shorter than expected, I will consider incorporating more samples into my tree and using a more 
complicated method, such as a maximum likeliness method or a Bayesian method. I think that comparing the outcomes of a maximum likeliness method to the simplistic NJM
would be very interesting, but as I have absolutely no experience with any of these methods or software I do not want to get in over my head. 
