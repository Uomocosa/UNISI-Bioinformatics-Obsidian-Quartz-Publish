##### Questions
- ***What are Off-Lattice Models?***
	- Off-lattice models are a type of computational model used in **protein folding simulations** that represent the protein as a continuous chain of atoms rather than as discrete points on a lattice. <br>==Unlike lattice models, which restrict protein motion to a pre-defined set of lattice points, off-lattice models allow proteins to move freely in three-dimensional space==, giving a more accurate representation of the actual structure of a protein.
	- Off-lattice models use molecular dynamics simulations or other computational methods to explore the folding pathway of a protein, taking into account the full range of interatomic interactions, including **van der Waals forces**, **electrostatic interactions**, **hydrogen bonding**, and **solvation effects**. <br>The simulations use empirical force fields or physical potentials to describe these interactions and to calculate the potential energy of different conformations of the protein.
	- Off-lattice models can provide detailed insight into the folding mechanisms of proteins and the factors that contribute to protein stability and function. <br>However, they are also **computationally intensive** and require large amounts of computational resources to simulate the folding process accurately. <br>Moreover, while off-lattice models provide a more accurate representation of the protein structure, they can be limited by the accuracy of the force fields used in the simulations, and further improvements are needed to fully capture the complexity of protein folding.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE **Off-Lattice Model**: The protein is not represented in a grid, the algorithm must decide every value of the angles $\phi$ and $\psi$ in the $C_{\alpha}$ carbon of each residue.
> #IMPORTANTE The score for off-lattice models is calculated using the **Root Mean Square Error** (RMSD) between the predicted and the observed configuration of $C_{\alpha}$

> #IMPORTANTE Off-Lattice Models may only include the $C_{\alpha}$, all the backbone atoms or even the side chain.
> Side chains (if included) may be **rigid**, **semi-flexible**, or **compleatly-flexible**.
> **Rigid side-chains**: (compleately statistical) using X-ray crystallographyes we use the most common confromation for each type of amminoacid.
> **Semi-Flexible side-chains**: Using the  X-ray crystallographyes and a clustering algorithm we calculate the centroids (called in this case **rotamers**), in the semi-flexible case, each side chain will use any of the rotamers most commonly observed.
> **Completely-Flexible side-chains**: different conformation of **rotamers** are allowed using a modest computation load.

##### —————————————————————
##### Slides with Notes

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-64 1.png]]

> #IMPORTANTE **Off-Lattice Model**: The protein is not represented in a grid, the algorithm must decide every value of the angles $\phi$ and $\psi$ in the $C_{\alpha}$ carbon of each residue.
> #IMPORTANTE The score for off-lattice models is calculated using the **Root Mean Square Error** (RMSD) between the predicted and the observed configuration of $C_{\alpha}$

> #IMPORTANTE Off-Lattice Models may only include the $C_{\alpha}$, all the backbone atoms or even the side chain.
> Side chains (if included) may be **rigid**, **semi-flexible**, or **compleatly-flexible**.
> **Rigid side-chains**: (compleately statistical) using X-ray crystallographyes we use the most common confromation for each type of amminoacid.
> **Semi-Flexible side-chains**: Using the  X-ray crystallographyes and a clustering algorithm we calculate the centroids (called in this case **rotamers**), in the semi-flexible case, each side chain will use any of the rotamers most commonly observed.
> **Completely-Flexible side-chains**: different conformation of **rotamers** are allowed using a modest computation load.

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-65 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-66 1.png]]
