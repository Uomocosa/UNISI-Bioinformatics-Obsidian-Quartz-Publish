##### Questions
- ***What are Lattice Models?***
	- ==Lattice models are simplified models of protein folding that represent the protein as a chain of connected beads or points on a lattice==. <br>In a lattice model, the protein is assumed to be constrained to move only along the lattice points, which simplifies the calculations required to model protein folding.
	- ==In a lattice model, the protein is represented by a sequence of connected lattice points, with each point representing an amino acid residue==. <br>The interactions between adjacent lattice points are described by a simplified energy function that takes into account the local geometry of the protein chain.
	- Lattice models are useful for exploring the folding of small proteins and for studying the basic principles of protein folding, such as the role of hydrophobic interactions and the formation of secondary structures. <br>They are **computationally efficient** and allow for the rapid exploration of large conformational spaces.
	- However, lattice models also have limitations. <br>They are highly simplified and do not take into account the full complexity of protein folding, such as the effects of solvent interactions and the role of non-local interactions in guiding the folding process. <br>Therefore, while lattice models can provide insight into the basic principles of protein folding, they may not be suitable for modeling the folding of larger or more complex proteins.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE ***What are Lattice Models?***:
> ==The protein folding is represnted in a 2D or 3D **grid**==
> The lattice statistical model **seeks to recreate protein folding by minimizing the free energy of the contacts between hydrophobic amino acids** (respecting principaly the “*hydrophobic rule*”).
> #IMPORTANTE **Ground Truth**: the ground truth for comparing actual protein folding, with the results from lattice models are given by the **X-ray Crystallography**:
> ![[Pasted image 20230114115216.png]]

> #IMPORTANTE **H-P Model** (Hydrophobic-Polar) : the simplest lattice model.
> ![[Pasted image 20230114115325.png]]
> The configuration score which we wish to minimize is given by the number of hydrophobi contact in the grid (each contatct values $-1$, so **the more contacts the better**)

> #IMPORTANTE For the **H-P Model** it was suggested that a possible mechanism for the secondary structure to maximize the number of contacts was to form **U-turns in antiparallel $\beta$-sheets**:
> ![[Pasted image 20230114115700.png]]

> #IMPORTANTE As the **Levinthal Paradox** states it’s impossible to try each possible combination, so **soft computing models** are necessary, such as:
> **Monte Carlo methods**
> **Machine Learning**
> **Genetic Algorithms**
> $\ldots$

> #IMPORTANTE One benefit of Lattice Models is the absolute representation of the direction, using the following names: R (Right), D (down), $\ldots$, we can create: ![[Pasted image 20230114120124.png]] 
> Or we can use the **relative representation**, (relative to the previous residue): ![[Pasted image 20230114120259.png]]
> #IMPORTANTE We need to avoid **steric collision**, for example if we go like L, L, L, L, in the relative representation we will return to the (0,0) starting point creating a collision of two residues (calld a *steric collision*).
> We can avoid steric collisions using an an **injective method** during the creation of the lattice model (this creation is also called **protein embedding** #NOT_SURE_ABOUT_THIS ) where we add one residue at the time avoiding a collision every time.
> Or we can assing a really high value to the configuration where we find a collision.

##### —————————————————————
##### Slides with Notes

> #IMPORTANTE ***What are Lattice Models?***:
> ==The protein folding is represnted in a 2D or 3D **grid**==
> The lattice statistical model **seeks to recreate protein folding by minimizing the free energy of the contacts between hydrophobic amino acids** (respecting principaly the “*hydrophobic rule*”).
> #IMPORTANTE **Ground Truth**: the ground truth for comparing actual protein folding, with the results from lattice models are given by the **X-ray Crystallography**:
> ![[Pasted image 20230114115216.png]]

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-53 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-54 1.png]]

> #IMPORTANTE **H-P Model** (Hydrophobic-Polar) : the simplest lattice model.
> ![[Pasted image 20230114115325.png]]
> The configuration score which we wish to minimize is given by the number of hydrophobi contact in the grid (each contatct values $-1$, so **the more contacts the better**)

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-55 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-56 1.png]] 

> #IMPORTANTE For the **H-P Model** it was suggested that a possible mechanism for the secondary structure to maximize the number of contacts was to form **U-turns in antiparallel $\beta$-sheets**:
> ![[Pasted image 20230114115700.png]]

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-57 1.png]]

> #IMPORTANTE As the **Levinthal Paradox** states it’s impossible to try each possible combination, so **soft computing models** are necessary, such as:
> **Monte Carlo methods**
> **Machine Learning**
> **Genetic Algorithms**
> $\ldots$

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-58 1.png]]

> #IMPORTANTE One benefit of Lattice Models is the absolute representation of the direction, using the following names: R (Right), D (down), $\ldots$, we can create: ![[Pasted image 20230114120124.png]] 
> Or we can use the **relative representation**, (relative to the previous residue): ![[Pasted image 20230114120259.png]]
> #IMPORTANTE We need to avoid **steric collision**, for example if we go like L, L, L, L, in the relative representation we will return to the (0,0) starting point creating a collision of two residues (calld a *steric collision*).
> We can avoid steric collisions using an an **injective method** during the creation of the lattice model (this creation is also called **protein embedding** #NOT_SURE_ABOUT_THIS ) where we add one residue at the time avoiding a collision every time.
> Or we can assing a really high value to the configuration where we find a collision.

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-59 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-60 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-61 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-62 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-63 1.png]]
