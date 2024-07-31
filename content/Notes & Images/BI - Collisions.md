##### Questions
- ***What we mean by Collision, when talking about a Recursive Neural Networks?***
	- In the context of Recursive Neural Networks (RNNs), ==collision refers to the phenomenon where different paths in the network converge to the same representation, leading to the loss of information==.
	- RNNs are neural networks that operate on sequences of inputs, such as sentences or time series data. <br>Recursive Neural Networks (also called Tree-Structured Neural Networks) are a type of RNN that operates on hierarchical structures such as parse trees, where the inputs are recursively combined to form larger structures.
	- ==When processing a tree structure with an RNN, the network performs a sequence of operations on the nodes of the tree, recursively combining the representations of the child nodes to form the representation of the parent node. <br>However, in some cases, multiple paths in the tree can lead to the same parent node, causing different representations to collide and merge into a single representation==.
	- ==This collision can lead to the **loss of information**==, as the different paths that led to the same node may have carried distinct information that is no longer distinguishable in the merged representation. <br>Several techniques have been proposed to address this issue, including using different weight matrices for each path or using attention mechanisms to weight the contribution of each path.

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 6 - NNSD-089.png]]![[BI - Lecture 6 - NNSD-090.png]]

- ***What are collisions?***
	- Given two different trees, when we apply the same RNN to each tree, the final result is the same
- ***Why are collisions bad?***
	- Not at all, we can use collision as a mean of classificatin, if we have 2 trees that we want to classify with the same class, we need that the final result collides.
- **Terminology**:
	- $l$ : **number of labels**
	- $m$ : **state vector dimension**
	- $k$ : **maximum out-degree of the trees**
	- $v$ : will indicate node number $v$
	- $t_n$ : $n$-th **tree**
	- $a$ : **number of bits** used to represent each component of the state vector
	- $h$ : **maximum height of the trees**

![[BI - Lecture 6 - NNSD-091.png]]