##### Questions
- ***How do Folding Algorithms work?***
	- ==Protein folding algorithms use computational methods to predict the three-dimensional structure of a protein from its amino acid sequence==. <br>==The algorithms typically work by **searching through the conformational space of possible protein structures** and identifying the structure that has the lowest potential energy==.
	- There are several types of protein folding algorithms, including **ab initio methods**, **homology modeling**, and **molecular dynamics simulations**.
		- **Ab initio methods** ==use simplified physical models== and computational heuristics to explore the conformational space of possible protein structures and identify low-energy conformations.
		- **Homology modeling methods** ==use existing protein structures== with similar sequences as a template to predict the structure of a new protein.
		- While **molecular dynamics simulations** ==use physical force fields== to simulate the folding process and predict the final conformation of the protein.
	- ==Protein folding algorithms typically start by generating an initial conformation of the protein and then use iterative optimization techniques to search for the low-energy state==. <br>The algorithms explore the conformational space of the protein by making small changes to the structure and evaluating the resulting change in energy. <br>The algorithms may use various optimization techniques, such as gradient descent, Monte Carlo sampling, or genetic algorithms, to search through the conformational space and identify the low-energy states.
	- The accuracy of protein folding algorithms depends on many factors, such as the quality of the force fields used, the accuracy of the starting conformation, and the complexity of the protein structure. <br>Moreover, predicting the structure of large or complex proteins can be challenging, and it may require combining multiple computational methods and experimental data to achieve high accuracy.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE **Folding Algorithms**
> 1. Select a protein folding model: **Lattice Models**, **Off-Lattice Models**
> 2. Define how to describe every possible conformation
> ~Ex.: *for lattice models* encoding the direction (R, L, U, D, …)
> ~Ex.: *for off-lattice models* listing the degrees ($\phi$, $\psi$ of $C_{\alpha}$)
> 3. Choose an energy function to evalueate how much a given conformation is favorable.
> 4. Selct an optimization method (Monte Carlo, Search All, Neural Networks, …).

##### —————————————————————
##### Slides with Notes

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-70 1.png]]

> #IMPORTANTE **Folding Algorithms**
> 1. Select a protein folding model: **Lattice Models**, **Off-Lattice Models**
> 2. Define how to describe every possible conformation
> ~Ex.: *for lattice models* encoding the direction (R, L, U, D, …)
> ~Ex.: *for off-lattice models* listing the degrees ($\phi$, $\psi$ of $C_{\alpha}$)
> 3. Choose an energy function to evalueate how much a given conformation is favorable.
> 4. Selct an optimization method (Monte Carlo, Search All, Neural Networks, …).

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-71 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-72 1.png]]
