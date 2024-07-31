##### Questions
- ***?***

---
##### IMPORTANTE

> #IMPORTANTE ***Smith-Waterman Algorithm***
> **Objective**: find the best matching subsequence.
> 
> - Initialize the first row and first columns to $0$
> - Set the miss match penalty to $-1$
> - Enter a $0$ in the table whenever all other routes would return a negative score 
>  
> Once the matrix is built:
> - Find the maximum score in the matrix
> - Proced backward and reconstruct the alignment until a $0$ is reached, this will be the ==best matching subsiquence==
> 
> *~Ex.: Rules*<br>![[Lecture 2-074 - Copy.png]]
> 
> *~Ex.: Algorithm* <br>![[Lecture 2-075 - Copy.png]]


---
##### Slides with Notes
![[Lecture 2-072.png]] ![[Lecture 2-073.png]] ![[Lecture 2-074.png]] ![[Lecture 2-075.png]] ![[Lecture 2-076.png]]

> #IMPORTANTE ***Smith-Waterman Algorithm***
> **Objective**: find the best matching subsequence.
> 
> - Initialize the first row and first columns to $0$
> - Set the miss match penalty to $-1$
> - Enter a $0$ in the table whenever all other routes would return a negative score <br>![[Lecture 2-074 - Copy.png]]
> 
> Once the matrix is built:
> - Find the maximum score in the matrix
> - Proced backward and reconstruct the alignment until a $0$ is reached, this will be the ==best matching subsiquence==
> 
> *~Ex.: Algorithm* <br>![[Lecture 2-075 - Copy.png]]
