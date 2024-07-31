##### Questions
- ***What are the difference of distance and characters based phylogenetic reconstruction methods?***
	- Distance-based and character-based phylogenetic reconstruction methods differ in how they represent and analyze the evolutionary information contained in molecular sequence data.
	- Distance-based methods use pairwise distances between sequences to construct a distance matrix, which is then used to infer the phylogenetic tree. <br>The distance matrix is usually based on a model of nucleotide or amino acid substitution, which describes the rate at which different nucleotide or amino acid states change over time. <br>The distance matrix is then used to construct the phylogenetic tree using algorithms such as neighbor-joining or **UPGMA**.
		- Distance-based methods are often faster and more computationally efficient than character-based methods, but they may be less accurate and less effective in handling complex evolutionary processes such as indels, multiple substitutions, and convergent evolution.
		- Character-based methods, on the other hand, use the actual sequence data, and their alignment, to infer the phylogenetic tree. <br>Character-based methods rely on models of nucleotide or amino acid substitution, which describe the probability of observing different nucleotide or amino acid states at each position in the sequence alignment. <br>These models can be used to calculate the likelihood of different trees given the sequence data, and the tree with the highest likelihood is chosen as the best estimate of the true phylogeny. <br>Character-based methods are generally more accurate and more effective in handling complex evolutionary processes, but they may also be more computationally intensive and require larger data sets than distance-based methods.
	- In summary, distance-based methods are based on pairwise distances between sequences and can be faster and more computationally efficient, but may be less accurate in handling complex evolutionary processes. <br>Character-based methods use the actual sequence data and can be more accurate and effective in handling complex evolutionary processes, but may be more computationally intensive and require larger data sets. <br>The choice of method depends on the specific data set and the research question being addressed.
- ***What are the main Comparisons among Phylogenetic Methdos?***
	- There are several factors that researchers consider when comparing different phylogenetic methods. Some of the main comparisons include:
	  1. **Accuracy**: The most important factor is the accuracy of the method, which is typically measured by comparing the inferred tree with a known true tree (if available) or with other independent sources of evidence.
	  2.  **Speed**: Another important consideration is the speed of the method, which is important when analyzing large datasets or when comparing multiple methods.
	  3.  **Robustness**: A method is considered robust if it is able to recover the same topology (or a similar topology) under different conditions, such as different alignment methods, different models of nucleotide or amino acid substitution, and different methods of tree inference.
	  4.  **Sensitivity to model assumptions**: Different phylogenetic methods make different assumptions about the evolutionary process, and the choice of model can affect the accuracy and robustness of the method. Some methods are more sensitive to model assumptions than others.
	  5.  **Handling of missing data**: Phylogenetic methods may be affected by missing data, such as gaps or ambiguous bases in the sequence alignment. Some methods are better able to handle missing data than others.
	  6.  **Scalability**: Some methods may not be scalable to large datasets, or may require significant computational resources to analyze large datasets.
	  7.  **Ease of use**: Finally, researchers may consider the ease of use of the method, including the availability of user-friendly software, documentation, and support.

##### —————————————————————
##### IMPORTANTE
> #IMPORTANTE What have pylogenetic trees brought us?
> Se una medicina funziona contro un infezione, portata da un organismo, è **probabile** che funzioni anche con altre infezioni portate da organismi della stessa famiglia
> Possiamo caratterizzare meglio se due organismi sono di due specie differenti, proteggendo una specie in particolare se serve.
> Costruzione dell’albero della vita (da cui abbiamo scoperto la distinzione in **eucarioti**, **procariti** e **archea**)

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 5-59 2.png]]

- ***What are the difference of distance and characters based phylogenetic reconstruction methods?*** 
	- ***Distance Based Method***: Simpler Methods (not computationally heavy), cannot reconstuct ancenstor DNA, always gives us a **rooted tree**, so we can always find the common ancenster.
	- ***Character Based Method***: Mainly focus on the parsimony principle, and can provide potentially useful inferences about the sequence of long extinct ancestors of all the living organisms.
	  However parsimony approaches can be computationally heavy.
	  It will give us **unrooted trees** most of the time.

![[BI - Lecture 5-60 2.png]]![[BI - Lecture 5-72 2.png]] ![[BI - Lecture 5-73 2.png]]