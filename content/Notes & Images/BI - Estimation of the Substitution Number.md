##### Questions
- ***How can we Estimate the Substitution Number?***
	- The substitution number, or the *number of substitutions that have occurred between two DNA or protein sequences*, can be estimated using various methods in molecular evolution, such as maximum likelihood, Bayesian inference, and parsimony methods.
		- ==**Maximum likelihood** and **Bayesian inference** methods use a statistical model of evolution to estimate the most likely number of substitutions that have occurred between two sequences==. <br>These methods consider the frequency of nucleotide or amino acid substitutions, as well as the patterns of substitution that occur at different sites in the sequence.
		- ==**Parsimony** methods, on the other hand, rely on the principle of *Occam's razor* to choose the simplest explanation for the observed differences between two sequences==. <br>This method counts the number of changes that are required to explain the observed differences between the two sequences and estimates the substitution number ==based on the minimum number of changes==.
	- Overall, estimating the substitution number between two sequences is important for understanding their evolutionary relationship and the degree of divergence between them.
- ***What is the James-Cantor Model?***
	- ==The James-Cantor model is a mathematical model used in molecular evolution to estimate the number of nucleotide substitutions that have occurred between two homologous DNA or RNA sequences==. <br>==It assumes that the nucleotide substitution rate is constant over time and that all nucleotide substitutions are equally likely==. <br>The model takes into account the possibility of multiple substitutions at the same site (i.e., parallel substitutions) and incorporates the observed frequencies of the four nucleotides in the two sequences being compared. <br>The model can be used to estimate the number of synonymous and non-synonymous substitutions separately, which can be used to study the evolution of protein-coding genes. <br>The James-Cantor model is one of the simplest nucleotide substitution models and is widely used in phylogenetic analysis and molecular clock studies.
- ***How did the James-Cantor Model Evolve?***
	- The James-Cantor Model is a mathematical model that describes the evolution of DNA sequences over time. It was first proposed by James and Cantor in 1975 and has since undergone several modifications and improvements
	- The original James-Cantor Model assumed that nucleotide substitutions occurred independently at each site in the DNA sequence, and that all four nucleotides had equal probability of being substituted. <br>However, subsequent research has shown that the actual process of nucleotide substitution is more complex and depends on factors such as the chemical properties of the nucleotides and their neighboring bases.
	- ==Therefore, several modifications and extensions to the James-Cantor Model have been proposed, including more sophisticated substitution models that take into account the effects of neighboring nucleotides, as well as models that account for different rates of evolution at different sites in the DNA sequence==. <br>These models have been used extensively in molecular evolution research to estimate evolutionary relationships and divergence times between species, and to identify sites in DNA sequences that are under positive or negative selection.
- ***Can you Explain the Math behind the James-Cantor Model?***
	- The James-Cantor model is a probabilistic model that calculates the expected number of substitutions between two DNA sequences over a given time period. The basic assumptions of the model are that the substitution rates are equal among sites in the sequence and that each site evolves independently. The model also assumes that the nucleotide frequencies are constant over time and that all substitutions are equally likely.
	- The model is based on the use of a rate matrix, which describes the probability of a nucleotide substitution from one base to another. The rate matrix is defined as follows: <br> `Q = { q_ij }`<br>Where:
		- `q_ij` is the rate of substitution from nucleotide `i` to nucleotide `j`. 
		- The diagonal elements `q_ii` are all equal to zero, since a nucleotide cannot substitute for itself. <br>
	- The off-diagonal elements are given by: <br>`q_ij = α_ij * β_j`<br>Where:
		- `α_ij` is the probability of a nucleotide substitution from `i` to `j` and `β_j` is the frequency of nucleotide `j`.<br>
	- The expected number of substitutions between two sequences is then calculated using the following formula: <br>`d = t * S`<br>Where:
		- `d` is the expected number of substitutions
		- `t` is the time in evolutionary units
		- `S` is the number of differences between the two sequences. <br>The value of `S` is usually estimated using methods such as pairwise alignment or multiple sequence alignment.<br>
	- The James-Cantor model can be extended to include more complex evolutionary scenarios, such as changes in the substitution rates over time or among different lineages. However, the basic model provides a useful framework for understanding the evolution of DNA sequences and for estimating the amount of evolutionary change between different sequences.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE **James-Cantor Model**:
> La possibilità che un nucelotida diventi un nucelotida diverso è pari a $3\over 4$ mentre la possibiltà che rimanga lo stesso è $1\over 4$. 
> Osservando due specie, il cui fenomeno di speciazione è avvenuto $2t$ fa, la possibilità che continuino a portare lo stesso singolo nucelotida “**C**” è pari a:
> $$P_{C(2t)} = \frac{1}{4} + \left(\frac{3}{4}\right)e^{-8(\alpha t)}$$
> Si considera che il rate di replecemnt frequency di un singolo nucelotida con un altro possibile sia $\alpha$, allora il rate di replacement di tutti i nucleotidi è $3\alpha$.
> Allora, il numero di sostituzioni $K$ sarà uguale a $K = 3\alpha \cdot 2t$
> Per calcolare $\alpha$ prendiamo la frazione di siti che differiscono tra le due specie:
> $$p = (1- P_{C(2t)}) = \frac{3}{4}\left(1- e^{-8(\alpha t)}\right)$$
> Quindi:
> $$8\alpha t = \ln\left(1-\frac{4}{3}p\right)$$
> L’equazione finale sarà:
> $$K = -\frac{3}{4}\cdot\ln\left(1-\frac{4}{3}p\right)$$

> #IMPORTANTE **James-Canter Model**:
> ![[Pasted image 20230106123042.png]]
> Tutte le basi hanno stesso rate di sostituzione $\alpha$.
> 
> #IMPORTANTE **Kimura Model**:
> ![[Pasted image 20230106123134.png]]
> Se sostituiamo una ***Purina*** (**G** & **A**) con l’altra purina, il rate di sostituzione è $\alpha$, lo stesso se sostituiamo una ***Pirimidina*** (**C** & **T**) con l’altra pirimidina.
> Al contrario se passiamo da purina a pirimidina o viceversa, il rate di sostituzione diventa $\beta = \frac{1}{3}\alpha$ (più improbabile).
> 
> #IMPORTANTE **General Time Reversible Model (GTR)**: Tutte le sostituzioni hanno rate diversi.


##### —————————————————————
##### Slides with Notes
![[Lecture 3-46.png]] ![[Lecture 3-47.png]] 
![[Lecture 3-48.png]] 
![[Lecture 3-49.png]] 
![[Lecture 3-50.png]] 
![[Lecture 3-51.png]] 
![[Lecture 3-52.png]] 
![[Lecture 3-53.png]] 
![[Lecture 3-54.png]] 
![[Lecture 3-55.png]]

> #IMPORTANTE **James-Cantor Model**:
> La possibilità che un nucelotida diventi un nucelotida diverso è pari a $3\over 4$ mentre la possibiltà che rimanga lo stesso è $1\over 4$. 
> Osservando due specie, il cui fenomeno di speciazione è avvenuto $2t$ fa, la possibilità che continuino a portare lo stesso singolo nucelotida “**C**” è pari a:
> $$P_{C(2t)} = \frac{1}{4} + \left(\frac{3}{4}\right)e^{-8(\alpha t)}$$
> Si considera che il rate di replecemnt frequency di un singolo nucelotida con un altro possibile sia $\alpha$, allora il rate di replacement di tutti i nucleotidi è $3\alpha$.
> Allora, il numero di sostituzioni $K$ sarà uguale a $K = 3\alpha \cdot 2t$
> Per calcolare $\alpha$ prendiamo la frazione di siti che differiscono tra le due specie:
> $$p = (1- P_{C(2t)}) = \frac{3}{4}\left(1- e^{-8(\alpha t)}\right)$$
> Quindi:
> $$8\alpha t = \ln\left(1-\frac{4}{3}p\right)$$
> L’equazione finale sarà:
> $$K = -\frac{3}{4}\cdot\ln\left(1-\frac{4}{3}p\right)$$

![[Lecture 3-56.png]] 
![[Lecture 3-57.png]] 
![[Lecture 3-58.png]] 
![[Lecture 3-59.png]] 
![[Lecture 3-60.png]] 
![[Lecture 3-61.png]]

> #IMPORTANTE **James-Canter Model**:
> ![[Pasted image 20230106123042.png]]
> Tutte le basi hanno stesso rate di sostituzione $\alpha$.
> 
> #IMPORTANTE **Kimura Model**:
> ![[Pasted image 20230106123134.png]]
> Se sostituiamo una ***Purina*** (**G** & **A**) con l’altra purina, il rate di sostituzione è $\alpha$, lo stesso se sostituiamo una ***Pirimidina*** (**C** & **T**) con l’altra pirimidina.
> Al contrario se passiamo da purina a pirimidina o viceversa, il rate di sostituzione diventa $\beta = \frac{1}{3}\alpha$ (più improbabile).
> 
> #IMPORTANTE **General Time Reversible Model (GTR)**: Tutte le sostituzioni hanno rate diversi.
