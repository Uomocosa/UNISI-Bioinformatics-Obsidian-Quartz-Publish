##### Questions

---
##### IMPORTANTE

> #IMPORTANTE ***The Needleman-Wunsch Algorithm***
> ***NOTE***: This is a dynamic algorithm that return the **optimal** alignment of two sequences.
> 
> Rules for constructing the matrix:
> - Initialize the first row to $0 ,\ -1 ,\ -2 ,\ \ldots$
> - Initialize the first column to $0 ,\ -1 ,\ -2 ,\ \ldots$
> - The element $i,j$ is the maximum of the following three rules.
> 	- A diagonal step, is not a malus
> 	- An orizontal or vertical step is a malus of $-1$
> 	- If the row $i$ is equal to the column $j$ it’s a bonus of $+1$, else: $+0$
> 
> Once constructed the matrix, we take the last element, and reconstruct the allignment.
> Watch the example, they are more clear.
> 
> ~Ex.: Rules <br>![[Lecture 2-056 - Copy.png]]
> 
> ~Ex.: Algorithm <br>![[Lecture 2-062 - Copy.png]]<br>![[Lecture 2-063 - Copy.png]]
> 
> ~Ex.: Algorithm II <br>![[Pasted image 20230319161102.png]]


---
##### Slides with Notes
![[Lecture 2-049.png]] ![[Lecture 2-050.png]] ![[Lecture 2-051.png]] ![[Lecture 2-052.png]] ![[Lecture 2-053.png]] ![[Lecture 2-054.png]] ![[Lecture 2-055.png]] ![[Lecture 2-056.png]] ![[Lecture 2-057.png]] ![[Lecture 2-058.png]] ![[Lecture 2-059.png]] ![[Lecture 2-060.png]] ![[Lecture 2-061.png]] ![[Lecture 2-062.png]] ![[Lecture 2-063.png]]

> #IMPORTANTE ***The Needleman-Wunsch Algorithm***
> ***NOTE***: This is a dynamic algorithm that return the **optimal** alignment of two sequences.
> 
> Rules for constructing the matrix:
> - A diagonal step, is not a malus
> - An orizontal or vertical step is a malus of $-1$
> - If the row $i$ is equal to the column $j$ it’s a bonus of $+1$, else: $+0$
> - The element $i,j$ is the maximum of this three rules.
> 
> Once constructed the matrix, we take the last element, and reconstruct the allignment.
> Watch the example, they are more clear.
> 
> ~Ex.: Rules <br>![[Lecture 2-056 - Copy.png]]
> 
> ~Ex.: Algorithm <br>![[Lecture 2-062 - Copy.png]]<br>![[Lecture 2-063 - Copy.png]]
> 
> ~Ex.: Algorithm II <br>![[Pasted image 20230319161102.png]]
