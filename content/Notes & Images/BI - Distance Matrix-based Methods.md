##### Questions
- ***What is the UPGMA?***
	- **UPGMA** stands for ***Unweighted Pair Group Method with Arithmetic Mean***. <br>==It is a distance-based method used in phylogenetic analysis to construct a tree from a distance matrix==. <br>UPGMA assumes that the rate of evolution is constant throughout the entire tree and that the distance between two sequences is proportional to the time since they diverged from a common ancestor.
	- ==The UPGMA method starts by considering each sequence as an individual cluster and gradually merges them into larger clusters based on their pairwise distances==. <br>==At each step, the two closest clusters are joined, and the distance between the new cluster and the other clusters is calculated as the average distance between the individual sequences in each of the merged clusters==. <br>This process continues until all sequences are clustered into a single group, forming a **rooted tree**.
	- **UPGMA** is a popular method because it is **simple**, **fast**, and **easy to implement**. <br>However, ==it has several limitations, such as the assumption of a constant rate of evolution== and the inability to handle certain types of data, such as sequences with unequal rates of evolution or sequences that have undergone convergent evolution.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE **UPGMA**: Unweighted-Pair-Group Method with Arithmetic Mean
> ![[Pasted image 20230107164301.png]]
> Prendiamo le due distanze minime e le sostituiamo con la loro media, che diventerà una nuova distanza, es:
> ![[Pasted image 20230107164441.png]]
> ![[Pasted image 20230107164349.png]]
> I primi archi dell’albero saranno:
> ![[Pasted image 20230107164457.png]]
> E la matrice si ridurra in:
> ![[Pasted image 20230107164514.png]]
> Iterando l’algoritmo otterremo:
> ![[Pasted image 20230107164634.png]]

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 4-59.png]] ![[BI - Lecture 4-60.png]] ![[BI - Lecture 4-61.png]] ![[BI - Lecture 4-62.png]] ![[BI - Lecture 4-63.png]] ![[BI - Lecture 4-64.png]] ![[BI - Lecture 4-65.png]] ![[BI - Lecture 4-66.png]] ![[BI - Lecture 4-67.png]] 

> #IMPORTANTE **UPGMA**: Unweighted-Pair-Group Method with Arithmetic Mean
> ![[Pasted image 20230107164301.png]]
> Prendiamo le due distanze minime e le sostituiamo con la loro media, che diventerà una nuova distanza, es:
> ![[Pasted image 20230107164441.png]]
> ![[Pasted image 20230107164349.png]]
> I primi archi dell’albero saranno:
> ![[Pasted image 20230107164457.png]]
> E la matrice si ridurra in:
> ![[Pasted image 20230107164514.png]]
> Iterando l’algoritmo otterremo:
> ![[Pasted image 20230107164634.png]]

![[BI - Lecture 4-68.png]] ![[BI - Lecture 4-69.png]] 
