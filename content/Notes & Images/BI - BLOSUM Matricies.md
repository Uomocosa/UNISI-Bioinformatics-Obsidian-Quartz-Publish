##### Questions
- ***What are BLOSUM Matricies?***
	- BLOSUM (**BLOcks SUbstitution Matrix**) matrices are a family of scoring matrices used in sequence alignment, which are based on blocks of conserved protein sequences. <br>These matrices are used to score the similarity between two amino acid sequences by assigning a numerical score to each possible alignment between the sequences.
	- ==BLOSUM matrices are derived from the observation that certain amino acid substitutions are more common than others in conserved regions of proteins. <br>The matrices are constructed by comparing large sets of related protein sequences and identifying blocks of highly conserved sequences that are at least a certain length. <br>The frequency of each possible substitution within each block is then calculated, and these frequencies are used to construct a substitution matrix==.
	- ==BLOSUM matrices are typically designated by a number indicating the percentage identity between the sequences used to derive the matrix. <br>*For example, the BLOSUM62 matrix is based on sequences that are 62% identical to each other. Higher numbers indicate more closely related sequences, while lower numbers represent more distantly related sequences*==.
	- BLOSUM matrices are commonly used in protein sequence alignment algorithms, such as BLAST and PSI-BLAST, to calculate the statistical significance of sequence matches and identify related sequences.

---
##### IMPORTANTE

> #IMPORTANTE ***BLOSUM Matricies (BLOcks amino acid SUbstitution Matricies)***
> Created to substuite the PAM matricies, making better use of the increased amount of information available.
> 
> ==The element of a BLOSUM are proportional to the **substitution frequency of amino acid $i$ and $j$** which are observed homologous proteins==.
> ==The element of a BLOSUM are invertially proportional to the **expected substitution frequency of amino acid $i$ and $j$**==.
> 
> BLOSUM matrices are typically designated by a number indicating the percentage identity between the sequences used to derive the matrix. <br>==*For example, the BLOSUM62 matrix is based on sequences that are 62% identical to each other. Higher numbers indicate more closely related sequences, while lower numbers represent more distantly related sequences*==


---
##### Slides with Notes
![[Lecture 2-042.png]]

> #IMPORTANTE ***BLOSUM Matricies (BLOcks amino acid SUbstitution Matricies)***
> Created to substuite the PAM matricies, making better use of the increased amount of information available.
> 
> ==The element of a BLOSUM are proportional to the **substitution frequency of amino acid $i$ and $j$** which are observed homologous proteins==.
> ==The element of a BLOSUM are invertially proportional to the **expected substitution frequency of amino acid $i$ and $j$**==.
> 
> BLOSUM matrices are typically designated by a number indicating the percentage identity between the sequences used to derive the matrix. <br>==*For example, the BLOSUM62 matrix is based on sequences that are 62% identical to each other. Higher numbers indicate more closely related sequences, while lower numbers represent more distantly related sequences*==

![[Lecture 2-043.png]] ![[Lecture 2-044.png]] 
