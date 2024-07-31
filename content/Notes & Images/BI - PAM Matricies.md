##### Questions
- ***What are PAM Matricies?***
	- PAM (**Point Accepted Mutation**) matrices are score matrices commonly used in bioinformatics for comparing amino acid sequences. <br>They were originally developed by Margaret Dayhoff and her colleagues in the 1970s, based on empirical observations of the frequency of amino acid substitutions in related protein sequences.
	- ==The PAM matrix provides a way to score alignments between two sequences based on the likelihood of each amino acid substitution occurring, given the frequency of observed substitutions between related sequences==. <br>*The PAM1 matrix represents the substitutions that are expected to occur after one unit of evolutionary divergence, while PAM250 represents substitutions that are expected to occur after 250 units of divergence*.
	- ==The PAM matrices are based on a model of sequence evolution, assuming that the probability of a substitution occurring between two amino acids is proportional to the probability of a random mutation occurring at that position==. <br>==*For example, if two amino acids have similar physicochemical properties, such as both being hydrophobic, then it is more likely that a substitution between them will occur compared to two amino acids with different properties*==.
	- The PAM matrices are widely used in sequence alignment algorithms, such as the Needleman-Wunsch or Smith-Waterman algorithms, to identify regions of homology or similarity between two protein sequences. <br>They have been superseded by more accurate and more versatile matrices, such as the BLOSUM matrices, which are based on a larger and more diverse set of protein sequences. <br>However, PAM matrices are still widely used in bioinformatics and can provide a useful tool for sequence analysis and comparison.
- ***What is a unit of divergence?***
	- In bioinformatics, a "unit of divergence" typically refers to the amount of evolutionary change that has occurred between two related sequences. <br>It is a measure of evolutionary distance or time, indicating how long ago two sequences shared a common ancestor.
	- ==The concept of a unit of divergence is often used in the context of amino acid substitutions, where a **single substitution is assumed to represent a single unit of evolutionary divergence**==. <br>*For example, if two sequences differ by 10 amino acid substitutions, they are said to have diverged by 10 units*.
	- The exact definition of a unit of divergence can vary depending on the context and the specific method of sequence analysis being used. <br>For example, in the context of PAM matrices, a unit of divergence is defined as the amount of evolutionary time required for a given amino acid substitution to occur with a certain probability, based on empirical observations of substitution frequencies in related sequences.

---
##### IMPORTANTE

> #IMPORTANTE [Youtube](https://www.youtube.com/watch?v=dcd-tDETXLM)

> #IMPORTANTE ***PAM Matricies***:
> **Point** or **Percent** **Accepted Mutation**
> Developed studying closely related proteins, mutations within superfamilies of proteins.
> It was clear that ==some amino acids substitutions occur more frequently than others==.
> And ==homologous proteins do not need to be necessarily constituted by the same amino acids in each positions==.

> #IMPORTANTE ***PAM Unit***:
> Two proteins are “distant” 1 PAM unit if they differ for a single amino acid out of 100, and the substitution is **accepted** (does not result in a loss of functionality).

> #IMPORTANTE ***Mutation Probability Matrix***
> $M$ is the Mutation Probability Matrix and also the base of all PAM Matricies.
> $M^{(1)}$ refers to a $20 \times 20$ matrix where (20 amino acids) where each element of the matrix depends on how many times that substitution has occurred (for example from R⇒E)
> The diagonal is the observed number of times that amino acid did not change.
> ==To create the $M^{(n)}$ matrix we multiply $M^{(1)}$ by itself $n$ times==.

> #IMPORTANTE ***PAM n Matrix***
> To create the PAM$^{(n)}$ matrix we take the $M^{(n)}$ and scale it according to the frequency of the residue $i$.
> 
> The PAM$^{(1)}$ matrix represents the substitutions that are expected to occur after one unit of evolutionary divergence.
> While PAM250 represents substitutions that are expected to occur after 250 units of divergence.
>
>The concept of a “**unit of divergence**” is often used in the context of amino acid substitutions, ==where a single substitution is assumed to represent a single unit of evolutionary divergence==. 
>*For example, if two sequences differ by 10 amino acid substitutions, they are said to have diverged by 10 units*.

> #IMPORTANTE ***Value of the PAM Matrix***
> $P_{ij} > 0$ more frequent than a random mutation
> $P_{ij} = 0$ frequent as a random mutation
> $P_{ij} < 0$ less frequent than a random mutation
---
##### Slides with Notes
![[Lecture 2-026.png]]

> #IMPORTANTE ***PAM Matricies***:
> **Point** or **Percent** **Accepted Mutation**
> Developed studying closely related proteins, mutations within superfamilies of proteins.
> It was clear that ==some amino acids substitutions occur more frequently than others==.
> And ==homologous proteins do not need to be necessarily constituted by the same amino acids in each positions==.

![[Lecture 2-027.png]]

> #IMPORTANTE ***PAM Unit***:
> Two proteins are “distant” 1 PAM unit if they differ for a single amino acid out of 100, and the substitution is **accepted** (does not result in a loss of functionality).


![[Lecture 2-028.png]] ![[Lecture 2-029.png]] ![[Lecture 2-030.png]] ![[Lecture 2-031.png]] ![[Lecture 2-032.png]] ![[Lecture 2-033.png]] ![[Lecture 2-034.png]] ![[Lecture 2-035.png]]  ![[Lecture 2-036.png]] ![[Lecture 2-037.png]]

> #IMPORTANTE ***Mutation Probability Matrix***
> $M$ is the Mutation Probability Matrix and also the base of all PAM Matricies.
> $M^{(1)}$ refers to a $20 \times 20$ matrix where (20 amino acids) where each element of the matrix depends on how many times that substitution has occurred (for example from R⇒E)
> The diagonal is the observed number of times that amino acid did not change.
> ==To create the $M^{(n)}$ matrix we multiply $M^{(1)}$ by itself $n$ times==.

![[Lecture 2-038.png]] ![[Lecture 2-039.png]]

> #IMPORTANTE ***PAM n Matrix***
> To create the PAM$^{(n)}$ matrix we take the $M^{(n)}$ and scale it according to the frequency of the residue $i$.
> 
> The PAM$^{(1)}$ matrix represents the substitutions that are expected to occur after one unit of evolutionary divergence.
> While PAM250 represents substitutions that are expected to occur after 250 units of divergence.
>
>The concept of a “**unit of divergence**” is often used in the context of amino acid substitutions, ==where a single substitution is assumed to represent a single unit of evolutionary divergence==. 
>*For example, if two sequences differ by 10 amino acid substitutions, they are said to have diverged by 10 units*.

![[Lecture 2-040.png]] ![[Lecture 2-041.png]]

> #IMPORTANTE ***Value of the PAM Matrix***
> $P_{ij} > 0$ more frequent than a random mutation
> $P_{ij} = 0$ frequent as a random mutation
> $P_{ij} < 0$ less frequent than a random mutation