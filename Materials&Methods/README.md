# Materials and Methods

Data was acquired from the GISAID database of COVID genomes. Genomes were collected from the lineages examined by Kandeel et al. In order to better utilize the
fixed-rate dendrogram methods, I collected the closest 49 samples to the genomes listed by Kandeel et. al.  Due to the overrerpresentation of Japanese
sequences in the original dataset, I opted to take samples of my variant lineages from alternative geographic locations for Beta, Delta, and Gamma variant
lineages. In order to evaluate the effectiveness of Kandeel et al's original model, I am retaining their original Japanese samples as well. All of the 
alternative genomes were restricted to samples collecte as close to the Japanese genome as possible.

## Software Methods

Alignments will be created using CLUSTAL, and pairwise comparative matrices generated using R. Phylogenetic analysis will be performed with RAXML phylogenetic software. 
The trees calculated using Neighbor Joining Method & Kimura Method will be done in RAXML. Bayesian trees will be created using RAXML as well.

## Phylogenetics

One issue with the Kandeel et al. article is that the authors utilized a very simplistic method on an incredibly small dataset. For this reason I will be using
the authors' methods on a much larger dataset than the 7 sequences they analyzed to test their model on larger data. I will additionally use Bayesian maximum
likelihood models to create a more accurate tree. All created trees will be compared to the models in Kandeel et. al. Likelihood-based phylogenetic analysis tends to be 
more accurate and powerful than fixed-rate approximations for relatedness and evolutionary distance, and this provides an opportunity to compare the the two.
