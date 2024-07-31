##### Questions
- ***Can you Explain the Heuristic Search for Quick Search Stragtegies?***
	- Heuristic search is a common approach for quickly searching through a large number of possible tree topologies in phylogenetic analysis. <br>==The basic idea behind heuristic search is to use a set of rules or strategies to guide the search process and quickly identify promising solutions without exhaustively evaluating all possible solutions==.
	- There are many different heuristic search strategies that have been proposed for phylogenetic analysis, but some of the most commonly used ones include:
	  1. **Nearest Neighbor Interchange** (**NNI**): This strategy involves ==swapping branches in the initial tree topology to generate new tree topologies==. <br>The search process continues by evaluating the likelihood or parsimony score of each new topology and choosing the topology with the best score. <br>This process is repeated, swapping different branches in the new topology, until a tree with the optimal score is found.
	  2. **Subtree Pruning and Regrafting** (**SPR**): This strategy involves ==pruning a subtree from the initial tree and then re-grafting it onto a different part of the tree to generate a new topology==. <br>The search process continues by evaluating the likelihood or parsimony score of each new topology and choosing the topology with the best score. <br>This process is repeated, pruning different subtrees and re-grafting them in different ways, until a tree with the optimal score is found.
	  3. **Tree-bisection-reconnection** (**TBR**): This strategy involves ==dividing the initial tree into two parts by cutting a branch and then reconnecting the two parts in a different way to generate a new topology==. <br>The search process continues by evaluating the likelihood or parsimony score of each new topology and choosing the topology with the best score. <br>This process is repeated, cutting different branches and reconnecting them in different ways, until a tree with the optimal score is found.
	- These heuristic search strategies are often combined with other techniques, such as simulated annealing, genetic algorithms, or Bayesian methods, to further improve the efficiency and accuracy of the search process.
	- Overall, heuristic search is a powerful tool for quickly searching through a large number of possible tree topologies and identifying promising solutions in phylogenetic analysis. <br>However, it is important to note that these methods do not guarantee that the optimal tree will be found, and the results should always be carefully evaluated and compared to other methods to ensure their accuracy and reliability.

##### —————————————————————
> #IMPORTANTE **Heuristic Search** for construction of phylogenetic trees:
> Dato un albero iniziale, gli algoritmi eurirstici si occupano di “migliolarlo”, attraverso uno o più di 3 metodi:
> **Nearest Neighbor Interchange**.
> **Subtree Pruning and Regrafting**.
> **Tree Bisectoon and Reconnection**.
> ![[Pasted image 20230109162905.png]]
> ![[Pasted image 20230109162925.png]]
> ![[Pasted image 20230109162941.png]]
> 
> Solitamente a ogni passo di un algoritmo euristico si cerca sempre di migliorare lo score dell’albero, ma è possibile fare un cambiamento permettendo mosse sfavorevoli, sperando che dopo un paio di mosse sfavorevoli si trovi un albero con uno score molto migliore, o di smuoversi da un minimo locale, in cerca di un miglior minimo locale o del minimo globale.
> ![[Pasted image 20230109163232.png]]

---
- Heuristic Algorithm start with a complete tree (chosen arbitrarily) and then perform changes to said tree, some example are:
	- **Nearest Neighbour Iterchange**
	- **Subtree Pruning and Regrafting**
	- **Tree Bisection and Reconnection**

> **NOTE**: 
> Heuristic Searches Algorithms actually work well if the “initial” tree is a good approximation of the most parsimonious tree


- In a Heuristic Search we can also decide how many “**bad decision**” are allowed, the more we allow the more trees we examine, but the algorithm will be slower, we can find a sweet spot on the amount of bad decision allowed.
  Or allow none at all, finding a pretty good final tree in the shortest amount of time and **try with different starting tree**.
  Or if we have some we can code into the algorithm some ***a priori* knowledge**.
##### —————————————————————
##### Slides with Notes
![[BI - Lecture 5-35 2.png]]![[BI - Lecture 5-36 2.png]]![[BI - Lecture 5-37 2.png]]![[BI - Lecture 5-38 2.png]]![[BI - Lecture 5-39 2.png]]![[BI - Lecture 5-40 2.png]]![[BI - Lecture 5-41 2.png]]![[BI - Lecture 5-42 2.png]]![[BI - Lecture 5-43 2.png]]![[BI - Lecture 5-44 2.png]]![[BI - Lecture 5-45 2.png]]