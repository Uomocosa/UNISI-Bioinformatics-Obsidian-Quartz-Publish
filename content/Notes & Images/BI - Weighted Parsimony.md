##### Questions
- ***What is Weighted Parsimony?***
	- ==Weighted parsimony is a method of phylogenetic inference that allows different character state changes (i.e., substitutions, insertions, and deletions) to have different costs based on their type or location==. <br>In contrast to unweighted parsimony, which assumes that all changes are equally likely, weighted parsimony takes into account the fact that some changes may be more or less likely to occur than others.
	- In weighted parsimony, the cost of each character state change is assigned a weight based on prior knowledge or assumptions about the evolutionary process. <br>*For example, transitions (i.e., changes from a purine to another purine or from a pyrimidine to another pyrimidine) may be assigned a lower cost than transversions* (i.e., changes from a purine to a pyrimidine or vice versa) because transitions are more common than transversions. Alternatively, indels (i.e., insertions or deletions) may be assigned a higher cost than substitutions because indels are generally less likely to occur than substitutions.
	- The goal of weighted parsimony is to find the tree with the minimum total weighted cost of character state changes. <br>This can be done using a variety of search algorithms, such as branch-and-bound, heuristic search, or stochastic search. The choice of algorithm and the weights assigned to different character state changes can have a significant impact on the resulting tree topology and the confidence of the phylogenetic inference.
	- Weighted parsimony is a more complex method of phylogenetic inference than unweighted parsimony, but it can improve the accuracy of the analysis by taking into account the variation in evolutionary rates and patterns across different regions of the sequences. <br>However, it still has some limitations, and more complex models of evolution, such as maximum likelihood and Bayesian inference, are often used in combination with parsimony to improve the accuracy of phylogenetic inference.
- ***What is an Autapomorphy?***
	- ==An autapomorphy is a derived character state that is **unique** to a single taxon or group of taxa (i.e., it is not found in any other taxa)==. <br>utapomorphies are sometimes also referred to as "unique derived characters" or "synapomorphies for a single taxon".
	- Autapomorphies are important in phylogenetic analysis because they can help to define and identify the boundaries between different taxa. <br>If two taxa share an autapomorphy, it suggests that they are more closely related to each other than to any other taxa. <br>However, if a taxon has an autapomorphy that is not shared by any other taxa, it may be difficult to place that taxon in a phylogenetic tree, because there are no other taxa with which it shares a common ancestor.
	- It is important to note that not all derived character states are autapomorphies. <br>A derived character state that is shared by two or more taxa is called a synapomorphy, and it indicates that those taxa share a common ancestor that had the derived character state. <br>In contrast, an autapomorphy is a derived character state that is unique to a single taxon or group of taxa, and it does not provide any information about the relationships among other taxa.
	- Autapomorphies can be identified through the process of character coding in phylogenetic analysis, which involves assigning character states to different taxa based on their observable traits or genetic sequences.
	- ==*For Example the human ability to walk upright on two legs (**bipedalism**). <br>Bipedalism is a derived character state that evolved in the lineage leading to humans, and it is not found in any other living primates*==
- ***What is a Synapomorphy?***
	- ==A synapomorphy is a derived character state that is shared by two or more taxa (i.e., it is not found in their common ancestor)==. Synapomorphies are sometimes also referred to as "shared derived characters" or "synapomorphic characters".
	- Synapomorphies are important in phylogenetic analysis because they provide evidence of shared ancestry among the taxa that possess them. If two or more taxa share a synapomorphy, it suggests that they share a more recent common ancestor with each other than with any other taxa that do not possess the synapomorphy.
	- ==*For example, the presence of feathers is a synapomorphy for birds and their closest living relatives, the theropod dinosaurs*. <br>*Feathers are not found in the common ancestor of birds and theropod dinosaurs*== (which was likely a small, bipedal, non-flying dinosaur), but they are a derived character state that evolved in the lineage leading to birds and was inherited by all of their descendants.
	- Synapomorphies can be identified through the process of character coding in phylogenetic analysis, which involves assigning character states to different taxa based on their observable traits or genetic sequences. Synapomorphies are particularly useful for inferring the relationships among closely related taxa, where there may be relatively few informative characters to distinguish between them. However, it is important to consider both synapomorphies and other types of characters (such as autapomorphies and plesiomorphies) in phylogenetic analysis, in order to build a robust and accurate tree.
- ***What is a Plesiomorpy?***
	- ==A plesiomorphy is a primitive character state that is shared by two or more taxa and is also present in their common ancestor==. Plesiomorphies are sometimes also referred to as "ancestral characters" or "primitive characters".
	- Plesiomorphies are important in phylogenetic analysis because they can be used to distinguish between groups of taxa that share a common ancestor further back in time. <br>==For example, the presence of hair is a plesiomorphic character state shared by all mammals, and it indicates that all mammals share a common ancestor that had hair==.
	- In contrast, a derived character state that is shared by two or more taxa but is not present in their common ancestor is called a synapomorphy. Synapomorphies are useful in phylogenetic analysis because they provide evidence of shared ancestry among closely related taxa.
	- It is important to consider both plesiomorphies and synapomorphies (as well as other types of characters, such as autapomorphies and homoplasies) in phylogenetic analysis, in order to build a robust and accurate tree. <br>By analyzing a combination of different types of characters, phylogeneticists can infer the evolutionary relationships among taxa and reconstruct the patterns of evolutionary history that have led to the diversity of life on Earth.
- ***What is an Homoplasy?***
	- ==Homoplasy is a term used in evolutionary biology to describe a similarity in the traits of different organisms that is **not due to common ancestry**==. Homoplastic characters have evolved independently in different lineages, either through convergent evolution (where similar traits evolve independently in distantly related organisms due to similar selective pressures), parallel evolution (where similar traits evolve independently in closely related organisms due to shared ancestry), or reversal (where a trait reverts to its ancestral state after evolving a derived state in a previous ancestor).
	- Homoplasy can be contrasted with homology, which refers to a similarity in traits that is due to shared ancestry. Homologous characters are derived from a common ancestor and can be used to infer the evolutionary relationships among different organisms.
	- ==*Examples of homoplasy include the wings of bats, birds, and insects, which evolved independently in each group but serve a similar function of flight; and the streamlined body shape of sharks and dolphins, which evolved independently in each group but is adaptive for efficient swimming in water*==.
	- Homoplasy can present a challenge for phylogenetic analysis, as it can lead to incorrect or conflicting tree topologies if homoplastic characters are incorrectly inferred to be homologous. Careful analysis and consideration of all available evidence, including molecular data, can help to distinguish between homologous and homoplastic characters and build accurate phylogenetic trees.

##### —————————————————————
> #IMPORTANTE **Weighted Parsimony**:
> ![[Pasted image 20230109153819.png]]

> **Autapomorphy**: A subclass of Apomorphy ![[Pasted image 20230109161743.png]]
> **Synapomorphy**: ![[Pasted image 20230109161803.png]]
> **Pleisomorphy** o **Symplesiomorphy**: ![[Pasted image 20230109161829.png]]
> **Homoplasy**: ![[Pasted image 20230109161851.png]]
> **Online resource**: [Youtube](https://www.youtube.com/watch?v=8K2Ydcy8jgw)

- Despite having established the general principle that “mutations are rare events”, inferring from this that all mutations are equivalent is an oversimplification (e.g., substitutions vs. indel events, indel length, transitions vs. transversions, etc.)
- If we could associate a value to the relative probability of different mutation events, these values would be translated into weights and used by parsimony algorithms, but it can be difficult to define a single set of weights with universal validity or otherwise usable by many different sets of data, because:
	- Some sequences (for example, non−coding sequences with tandem repeats) are more prone to indel events than others.
	- The functional importance differs greatly from gene to gene and from species to species also for homologous genes.
	- The predisposition to “soft” substitutions (e.g. GC with AT, or between codons that specify the same amino acid) usually varies from gene to gene and from species to species.
- The best choice for the weights is related to a **particular set of empirical data**.
  ***~Example:*** If, **for a particular multiple alignment** (we study the weights of particular alignments, and not one weight for all), comparisons between each single sequence and a consensus sequence indicate that the transitions are three times more common than transversions, then: values equal to 1 and 0.33 must be, respectively, associated to transversions and transitions.
  At the end of the analysis, the tree predicting the smallest number of the most common mutation events is the most parsimonious.

##### —————————————————————
# Original Files
![[BI - Lecture 5-24 2.png]]![[BI - Lecture 5-25 2.png]]