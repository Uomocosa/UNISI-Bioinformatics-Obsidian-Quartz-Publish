##### Questions
- ***What is Database Search and Pairwise Alignments?***
	- Database search and pairwise alignments are two common methods used in bioinformatics to compare and analyze biological sequences, such as DNA, RNA, and protein sequences.
	- Database search involves comparing a query sequence to a large database of known sequences to find similar matches. <br>This is often used in sequence annotation, where a newly discovered sequence is compared to existing sequences to identify its function or potential homologs. <br>==Popular tools for database searching include **BLAST** (Basic Local Alignment Search Tool) and **FASTA**==.
	- ==Pairwise alignment involves comparing two sequences to identify regions of similarity and difference==. <br>This is useful for studying evolutionary relationships between sequences, identifying conserved regions, or detecting **mutations**. <br>==In pairwise alignment, two sequences are aligned based on their similarity, with gaps introduced in one or both sequences to optimize the alignment==. <br>Popular tools for pairwise alignment include **ClustalW** and **MUSCLE**.
	- Both database search and pairwise alignments are essential tools in bioinformatics and can provide valuable insights into the *structure*, *function*, and *evolutionary history* of biological sequences.
- ***Can you make an Example of Pairwise Alignments?***
	- Let's say we have two DNA sequences:
		- Sequence 1: **ATCGCTAGGGCACGACT**
		- Sequence 2: **ATCGCTACGGCACGACT**
	- To align these two sequences, we would look for regions of similarity and difference. <br>We can align them as follows:
		- Sequence 1: **ATCGCTAGGGCACGACT**
		- Sequence 2: **ATCGCTA-CGGCACGACT**
	- In this alignment, we've introduced a **gap** in sequence 2 to align it with sequence 1. <br>We can calculate the percent identity of this alignment by counting the number of identical nucleotides divided by the total number of aligned nucleotides. <br>In this case, the percent identity is $94\%$ (16/17).
	- Pairwise alignments can be useful for identifying mutations or variations in DNA sequences, as well as for studying evolutionary relationships between sequences. <br>They can also be used to identify conserved regions that are important for the function of a protein or RNA molecule.
##### —————————————————————

##### IMPORTANTE
> #IMPORTANTE L’allineamento di sequenze genetiche o del DNA, è usato per:
> 1. Determinare la funzione di nuove sequenze genetiche, appena scoperte, sulla base di simili sequenze già conosciute.
> 2. Determinare la relazione evoluzionistica di due geni, proteine o intere specie.
> 3. Predirre la struttura e la funzione di nuove proteine basandosi su simili proteine, già conosciute.


##### —————————————————————
##### Slides with Notes
![[Lecture 2-003.png]] ![[Lecture 2-004.png]]

> #IMPORTANTE L’allineamento di sequenze genetiche o del DNA, è usato per:
> 1. Determinare la funzione di nuove sequenze genetiche, appena scoperte, sulla base di simili sequenze già conosciute.
> 2. Determinare la relazione evoluzionistica di due geni, proteine o intere specie.
> 3. Predirre la struttura e la funzione di nuove proteine basandosi su simili proteine, già conosciute.

![[Lecture 2-116.png]] ![[Lecture 2-117.png]]
