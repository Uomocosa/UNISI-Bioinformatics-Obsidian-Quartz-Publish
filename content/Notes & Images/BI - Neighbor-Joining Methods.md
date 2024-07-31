##### Questions
- ***What are the Neighbor-Joining Methods?***
	- The Neighbor-Joining (NJ) method is a widely used distance-based method for constructing phylogenetic trees. <br>==It is a heuristic algorithm that is efficient and relatively fast for large datasets. The basic idea of the NJ method is to iteratively group the most closely related sequences until the entire tree is constructed==.
	- The NJ method starts by calculating a pairwise distance matrix for all sequences in the dataset. <br>Then, it selects the two sequences with the smallest distance and groups them together into a node. <br>The distance from the new node to all other nodes is calculated as the average of the distances from each of the two original sequences to each node. <br>This process is repeated until all sequences are grouped into a tree.
	- One of the main advantages of the NJ method is its speed, which makes it possible to construct trees for large datasets. <br>==However, the NJ method can also be sensitive to random errors and biases in the distance matrix, and may not always produce the most accurate tree==. <br>Therefore, it is important to evaluate the quality of the NJ tree using statistical methods and/or other tree-building methods.
##### —————————————————————
##### IMPORTANTE

> #NOT_SURE_ABOUT_THIS 
> #IMPORTANTE **Neighbor Joining Methods**:
> Similmente all’**UPMGA** si trovano da un albero a stella iniziale, i due nodi che sono più vicini tra loro:
> ![[Pasted image 20230108131736.png]]
> Mettiamo che per esempio la distanza minima in qesto caso sia $d_{12}$ ⇒
> ![[Pasted image 20230108131834.png]]
> Si ripete il progesso fino a che non otteniamo un **un-rooted tree**.
> ![[Pasted image 20230108131927.png]]
> Da questo poi possiamo prendere il migliore **rooted tree**.
> Ricordiamo che da un *un-rooted tree* di $f$ foglie, si possono creare fino a $2f-3$ *rooted trees*.
> Inoltre invece della semplice distanza tra due folgie possiamo applicare una “trasformazione”, usando le formule per $S$ o $Q$:
> ![[Pasted image 20230108132153.png]]
> **Online resource**: [Youtube](https://www.youtube.com/watch?v=yhR843hHKtk)

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 4-86.png]] ![[BI - Lecture 4-87.png]] ![[BI - Lecture 4-88.png]] ![[BI - Lecture 4-89.png]]

> #NOT_SURE_ABOUT_THIS 
> #IMPORTANTE **Neighbor Joining Methods**:
> Similmente all’**UPMGA** si trovano da un albero a stella iniziale, i due nodi che sono più vicini tra loro:
> ![[Pasted image 20230108131736.png]]
> Mettiamo che per esempio la distanza minima in qesto caso sia $d_{12}$ ⇒
> ![[Pasted image 20230108131834.png]]
> Si ripete il progesso fino a che non otteniamo un **un-rooted tree**.
> ![[Pasted image 20230108131927.png]]
> Da questo poi possiamo prendere il migliore **rooted tree**.
> Ricordiamo che da un *un-rooted tree* di $f$ foglie, si possono creare fino a $2f-3$ *rooted trees*.
> Inoltre invece della semplice distanza tra due folgie possiamo applicare una “trasformazione”, usando le formule per $S$ o $Q$:
> ![[Pasted image 20230108132153.png]]
> **Online resource**: [Youtube](https://www.youtube.com/watch?v=yhR843hHKtk)

![[BI - Lecture 4-90.png]]
