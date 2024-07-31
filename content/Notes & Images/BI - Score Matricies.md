##### Questions
- ***What are Score Matricies?***
	- Score matrices, also known as substitution matrices, are used in bioinformatics to score alignments between two or more sequences. They are typically used in pairwise sequence alignment algorithms such as the Needleman-Wunsch or Smith-Waterman algorithms, which are commonly used for sequence comparison and alignment.
	- Score matrices are used to assign a score to each possible pair of residues aligned in the sequences being compared. The score assigned to each pair reflects the likelihood of that pair occurring in related sequences based on empirical observations of the frequency of substitutions between different amino acids or nucleotides. In other words, the matrix provides a way to quantify the similarity or dissimilarity between two sequences.
	- The most commonly used score matrix in bioinformatics is the BLOSUM matrix, which stands for "Blocks Substitution Matrix". BLOSUM matrices are derived from alignments of closely related protein sequences and are available in several versions ranging from BLOSUM 30 to BLOSUM 90, with higher values indicating greater sequence divergence. Other commonly used score matrices include the PAM matrix and the JTT matrix, which are also derived from empirical data.
	- Score matrices are an essential tool in bioinformatics, as they provide a quantitative measure of sequence similarity that can be used for a variety of applications, including identifying conserved domains or motifs, predicting protein structure and function, and identifying homologous sequences.

---
##### IMPORTANTE

> #IMPORTANTE ***Gap Penality for Amino Acids Interchange***: <br>![[Lecture 2-020 - Copy.png]] ![[Lecture 2-021 - Copy.png]] 

> #IMPORTANTE ***Score Matricies for Nucleotides*** <br>![[Lecture 2-022 - Copy.png]]

> #IMPORTANTE ***Amino Acid Score Matrix***
> Several Criteria can be considered in seting up a score matrix for amino acid sequence alignments:
> - Physico-Chemical Similarity: **Size**, **Charge** (positive or negative pH), and **Electronegativity** (Polar, hydrophilic, …)
> - Genetic Similarity
> - Observed Replacement Frequencies

> #IMPORTANTE The most common method to derive score matricies consists in observing the actual frequencies of amino acid susbtitutions in Nature.

---
##### Slides with Notes
![[Lecture 2-020.png]] 

> #IMPORTANTE ***Gap Penality for Amino Acids Interchange***: <br>![[Lecture 2-020 - Copy.png]] ![[Lecture 2-021 - Copy.png]] 

![[Lecture 2-021.png]] ![[Lecture 2-022.png]]

> #IMPORTANTE ***Score Matricies for Nucleotides*** <br>![[Lecture 2-022 - Copy.png]]

![[Lecture 2-023.png]]

> #IMPORTANTE ***Amino Acid Score Matrix***
> Several Criteria can be considered in seting up a score matrix for amino acid sequence alignments:
> - Physico-Chemical Similarity: **Size**, **Charge** (positive or negative pH), and **Electronegativity** (Polar, hydrophilic, …)
> - Genetic Similarity
> - Observed Replacement Frequencies

![[Lecture 2-024.png]] ![[Lecture 2-025.png]]  

> #IMPORTANTE The most common method to derive score matricies consists in observing the actual frequencies of amino acid susbtitutions in Nature.

