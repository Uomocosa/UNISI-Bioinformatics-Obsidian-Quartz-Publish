##### Questions
- ***What is the Chou-Fasman Method?***
	- ==The Chou-Fasman method is a method for predicting the secondary structure of a protein from its amino acid sequence==. <br>It was developed in the late 1970s by Pauling Chou and Gerald Fasman, and is based on the observation that certain amino acids tend to occur more frequently in alpha helices or beta sheets.
	- ==The Chou-Fasman method assigns a score to each amino acid based on its propensity to form an alpha helix or beta sheet. <br>These scores were determined by analyzing the frequency of each amino acid in known protein structures==. <br>*For example, amino acids with high scores for alpha helix formation include alanine, glutamic acid, leucine, and methionine, while those with high scores for beta sheet formation include valine, isoleucine, and phenylalanine*.
	- ==The Chou-Fasman method uses a sliding window algorithm to predict the probability of each secondary structure element (alpha helix, beta sheet, or random coil) at each position along the protein sequence==. <br>The algorithm calculates a score for each amino acid in the window based on its propensity to form each type of secondary structure, and then uses these scores to predict the most likely secondary structure at that position.
	- The Chou-Fasman method was one of the first methods developed for secondary structure prediction, and is still widely used today. <br>However, its accuracy is limited by the fact that it is based on empirical observations, and does not take into account the context in which each amino acid occurs in the protein sequence. More recent methods, such as neural networks and deep learning approaches, have shown improved accuracy in secondary structure prediction.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE **Chou-Fasman Method**:
> ![[Pasted image 20230113145455.png]]
> $P(a)$: Weight (or paremetr) of the amminoacid to be a part of an **$\alpha$-helic**
> $P(b)$: Weight (or paremetr) of the amminoacid to be a part of a **$\beta$-sheet**
> $P(t)$: Weight (or paremetr) of the amminoacid to be a part of a **$\beta$-turn**
> $f(i)$, $\ldots$,  $f(i+3)$: called “turn parameters”, they represent the frequency with which it is observed in the first, second, third or fourth position of an **harpin turn**.
> 
> Let’s see an example to determine $\alpha$-helics and $\beta$-sheets:
> Sequence: 
> ![[Pasted image 20230113150204.png]]
> Using the parameters for $P(a)$ we substitute the amminoacids with their corresponding weights: ![[Pasted image 20230113150329.png]]
> **Algorithm ($\alpha$-helics)**:
> 1. We search for a region where 4 out of 6 contiguos peptides (or residue or amminoacids) have weight **above** $100$ (the first box in red: 70-142-151-67-114-121).
> 2. We then search for **two regions BEFORE and AFTER**  the one just found where there are 4 contiguos peptides that are **under** $100$ (after the end of the blue box: 69-67-57-57)
> 3. Taking this region (the first red box + the blue box, corresponding to: **CAENKLDHVADCCILFMTWDYNG**), we calculate the sum of all the $P(a)$, which is equal to 2134, then we calculate the sum of all $P(b$) of said region, which is equal to 2061, since $\sum P(a) > \sum P(b)$ we say that this is an $\alpha$-helic 
> 4. We repeat the first three step untill we finish all the amminoacid, in fact we do find another chain that respect the first two condition (the second red box: 57-70-108-101, corresponding to: **PCIFID**), tho this is **NOT** an $\alpha$-helics since $\sum P(a)$= 557 is **lower** than $\sum P(b)$ = 686.
> 
> ![[Pasted image 20230113151644.png]]
> **Algorithm ($\beta$-helics)**:
> 1. Same as for the $\alpha$-helics algorithm but it needs to be $3$ out of $5$ peptides with $P(b)>100$ (red regions)
> 2. The “stop” sign for the “extened regions” is $3$ contiguos peptides with $P(b)<100$ (37-89-74, 89-75-55, 89-75-55)
> 3. If $\sum P(b) > \sum P(a)$ ⇒ it’s a $\beta$-sheet.
> 4. Repeat
> 
> #IMPORTANTE If the same region is defined as both an $\alpha$-helics and a $\beta$-sheet, then we calculate its $\sum P(a)$ and $\sum P(b)$, if the first is greater than it’s an helic, otherwise it’s a sheet.

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 10 - Prediction of Protein and RNA Structure-24 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-26 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-27 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-28 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-29 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-30 1.png]]
