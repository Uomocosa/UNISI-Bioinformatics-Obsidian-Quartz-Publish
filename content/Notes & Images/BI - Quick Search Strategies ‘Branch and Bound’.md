##### Questions
- ***Can you Explain the Branch and Bound Method for Quick Search Stragtegies?***
	- The branch-and-bound method is a heuristic search algorithm commonly used in phylogenetic analysis to quickly search through a large number of possible trees and identify the optimal tree. It is a type of "divide-and-conquer" algorithm that breaks down a large search space into smaller, more manageable subspaces and recursively searches through them.
	- The basic idea behind the branch-and-bound method is to start with an initial tree and evaluate its likelihood score (or parsimony score, depending on the optimization criterion). The algorithm then systematically generates all possible variations of the initial tree by making local modifications (such as swapping branches or changing branch lengths) and evaluates the likelihood or parsimony score of each variant. The variants that do not improve upon the score of the initial tree are pruned (i.e., eliminated from further consideration), while the promising variants are kept and recursively searched.
	- The search process continues until all possible tree topologies have been evaluated and the optimal tree with the highest likelihood or parsimony score has been identified.
	- The branch-and-bound method is a relatively quick search strategy, but it can still be computationally expensive for very large datasets with many taxa or sites. To improve efficiency, various modifications and optimizations to the basic algorithm have been proposed, such as using heuristics to prune un-promising branches early in the search process, or using parallel computing to speed up the search across multiple processors.
	- Overall, the branch-and-bound method is a useful tool for quickly searching through a large number of possible tree topologies and identifying the optimal tree in phylogenetic analysis.
- ***Can you define each step of the Branch and Bound Method for Quick Search Stragtegies?***
	- Sure, here are the steps involved in the basic branch-and-bound method for phylogenetic tree search:
	  1. **Initialize**: Choose an initial tree topology and compute its likelihood or parsimony score.
	  2. **Generate variations**: Systematically generate all possible variations of the initial tree by making local modifications (such as swapping branches or changing branch lengths).
	  3. **Evaluate**: Evaluate the likelihood or parsimony score of each variant.
	  4. **Prune unpromising branches**: Prune (i.e., eliminate from further consideration) any variants that do not improve upon the score of the initial tree.
	  5. **Identify promising variants**: Keep the promising variants (i.e., those that show improvement in the score) and continue recursively searching through them.
	  6. **Repeat steps 2-5**: Continue generating and evaluating variants, pruning unpromising branches, and identifying promising variants until all possible tree topologies have been evaluated and the optimal tree has been identified.
	  7. **Return the optimal tree**: Once the search is complete, return the optimal tree with the highest likelihood or parsimony score.
	- Note that in practice, there are many variations and optimizations of the basic branch-and-bound method, such as using heuristics to prune un-promising branches early in the search process, or using parallel computing to speed up the search across multiple processors. However, the basic steps outlined above provide a general overview of the branch-and-bound approach to phylogenetic tree search.

##### —————————————————————
> #IMPORTANTE **Branch and Bound** for construction of phylogenetic trees:
> Algoritmo **esatto**, troverà la soluzione ottimale, dato abbastanza tempo.
> Preso un primo albero creato a caso, salviamo in memoria la sua lunghezza $L$, in questo caso la lunghezza è il numero di mutazioni all’interno dell’albero, durante la creazione di nuovi alberi, se la loro lunghezza supera $L$ interrompiamo il processo (risparmiando tempo), se invece la loro lunghezza $L’$ è inferiore alla precedente lunghezza, rimpiazziamo $L$ con $L’$ e ripetiamo il processo, adesso che la nuova lunghezza massima è inferiore, risparmieremo ancora più tempo.

- ***Definition of Tree Length***: The length of a tree $L$, is defined as the sum of the minimum numbers of substitutions over all sites for the given topology
- The branch and bound method consists of two steps: 
	1. Fixing an upper bound $L$, for the most parsimonious tree length w.r.t. a certain set of data, note that $L$ **can be estimated**, for example:
		- By randomly choosing a tree that describes the relations among all the sequences to be analysed
		- Or we can build a reasonable approximation of the most parsimonious tree (for example, by UPGMA - **Unweighted Pair Group Method with Arithmetic Mean**)
	2. Construction of each tree, adding a branch at a time, to include all the sequences to be analysed, ending the procedure when the tree reaches the previously established length $L$
- ***Simple Explantation***: Decide on an upper length $L$, then start iterating creating the trees, if a tree reach the length $L$, start with another tree.
  Also, if we finish a tree which has a smaller length than $L$, let’s say $L_1$ (so $L_1 \lt L$) we can update the new maximum length, so the next iteration will be more efficient.

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 5-29 2.png]]![[BI - Lecture 5-30 2.png]]![[BI - Lecture 5-31 2.png]]![[BI - Lecture 5-32 2.png]]![[BI - Lecture 5-33 2.png]]![[BI - Lecture 5-34 2.png]]