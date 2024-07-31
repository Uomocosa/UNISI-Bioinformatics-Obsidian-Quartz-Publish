##### Questions
- ***What are Informative and Non-Informative Sites?***
	- In phylogenetic analysis, informative sites are positions in the aligned DNA or protein sequences of a group of related organisms that differ among the sequences. <br>These differences can reflect evolutionary changes, such as mutations or insertions/deletions (indels), that have occurred over time and can be used to infer the evolutionary relationships among the organisms. <br>==Informative sites are important for phylogenetic inference because they provide data that can distinguish between different possible evolutionary scenarios==.
	- On the other hand, ==non-informative sites are positions in the aligned sequences where all the sequences have the same nucleotide or amino acid==. <br>These sites do not provide any useful information for phylogenetic inference because they do not help to distinguish between different evolutionary scenarios. <br>Non-informative sites can arise due to various reasons, such as the presence of conserved regions in the sequences or the saturation of mutations in rapidly evolving regions.
	- In general, the more informative sites there are in a sequence alignment, the better the phylogenetic analysis will be able to distinguish between different evolutionary scenarios and the more confident we can be in the resulting tree. <br>However, it is also important to consider the quality and completeness of the sequence data, as well as other factors such as model assumptions and the choice of phylogenetic methods, when interpreting the results of a phylogenetic analysis.

##### —————————————————————
> #IMPORTANTE **Informative and non-informative sites**:
> Given a number $n$ sequences, which have to be more than two sequences (we are talking about **multiple allignments**) we call **informative sites** those sites that have at least 2 different nucleotides, and each nucleotide has to be represented at least twice.
> *~Ex.:*
> ![[Pasted image 20230109150858.png]]
> a) 1 nucleotides repeted 4 times (**G**$\times 4$) : **non-informative** site
> b) **G**$\times 3$ ,  **A**$\times 1$ : **non-informative** site
> c) **G**$\times 2$ ,  **A**$\times 1$ ,  **T**$\times 1$ : **non-informative** site
> d) **G**$\times 1$ ,  **A**$\times 1$ ,  **T**$\times 1$  ,  **C**$\times 1$ : **non-informative** site
> e) **G**$\times 2$ ,  **A**$\times 2$ : **INFORMATIVE** site
> f) **G**$\times 2$ ,  **T**$\times 2$ : **INFORMATIVE** site

- In general, in order for a position to be informative, regardless of how many sequences are aligned, it must contain at least two different nucleotides, each of which must be present at least twice.
- The non−informative positions are simply discarded and not considered in the subsequent parsimony analysis.
- Let’s see an example and take these sequences into account:
![[Pasted image 20221114165323.png]]
- **Non-Informative Sites**:
	- “*Column a*”: all the sequences in the column a are “**G**”, **Invariant sites are non-informative**, all possible phylogenetic threes have the same number of mutation:  $0$ ![[Pasted image 20221114165613.png]]
	- “*Column b*”: ![[Pasted image 20221114165658.png]]
	- “*Column c”: ![[Pasted image 20221114165823.png]]
	- “*Column d”: ![[Pasted image 20221114165905.png]]
- **Informative Sites**
	- “*Column e & f*”: ![[Pasted image 20221114165935.png]] ![[Pasted image 20221114165957.png]] 


##### —————————————————————
# Original Files
![[BI - Lecture 5-07 2.png]]![[BI - Lecture 5-08 2.png]]![[BI - Lecture 5-09 2.png]]![[BI - Lecture 5-10 2.png]]![[BI - Lecture 5-11 2.png]]![[BI - Lecture 5-12 2.png]]![[BI - Lecture 5-13 2.png]]![[BI - Lecture 5-14 2.png]]![[BI - Lecture 5-15 2.png]]![[BI - Lecture 5-16 2.png]]