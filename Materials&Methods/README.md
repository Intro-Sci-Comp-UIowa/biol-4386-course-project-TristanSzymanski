# Materials and Methods

Data was acquired from the GISAID EpiCov database of genomes collected from patients afflicted by COVID-19. Genomes were selected from the lineages examined by Kandeel 
et al. The GISAID database is a global collaboration to collect, track, monitor, and share data on emerging epidemics. Due to this collaborative nature, GISAID prohibits 
its members to share the data itself in any publicly accessible format in order to ensure that its collaborators are properly credited for their contributions to the
database. This is explained in further in the Data/ readme.

In order to better utilize the fixed-rate dendrogram methods, I collected the closest 49 samples to the genomes listed by Kandeel et. al.  Due to the overrerpresentation 
of Japanese sequences in the original dataset, I opted to take samples of my variant lineages from alternative geographic locations for Beta, Delta, and Gamma variant
lineages. In order to evaluate the effectiveness of Kandeel et al's original model, I am retaining their original Japanese samples as well. All of the 
alternative genomes were restricted to samples collecte as close to the Japanese genome as possible.

## Software Methods

Alignments were originally planned to be made using CLUSTAL, as was used by Kandeel et al, however the large volume of data processing proved to be too cumbersome for
Clustal, which is swiftly becoming outdated software. Alignments were instead created using Nextalign, which is the alignment software used by the GISAID database. 
Phylogenetic analysis will be performed with RAXML phylogenetic software. The trees calculated using Neighbor Joining Method & Kimura Method will be done in RAXML. 
Bayesian trees will be created using RAXML as well.

## Phylogenetics

One issue with the Kandeel et al. article is that the authors utilized a method typically used for high volumes of data on an incredibly small dataset. This led to the 
phylogenetic tree depicting an inaccurate Omicron lineage. For this reason I will be using the authors' methods on a dataset of 401 genomes. I will additionally use 
Bayesian maximum likelihood models to create a more accurate tree. All created trees will be compared to the models in Kandeel et. al. Likelihood-based phylogenetic 
analysis tends to be more accurate and powerful than fixed-rate approximations for relatedness and evolutionary distance, and this provides an opportunity to compare the 
the two.
