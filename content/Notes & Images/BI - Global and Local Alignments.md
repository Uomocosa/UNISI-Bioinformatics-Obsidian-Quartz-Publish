##### Questions
- ***?***

---
##### IMPORTANTE

> #IMPORTANTE ***Global and Semi-Global Alignments***:
> The Needleman-Wunsch Algorithm preferes the global alignment, but we can change it to make it return the optimal solution for local alignment: <br>![[Lecture 2-066 - Copy.png]]
> ***NOTE***: How the two alignments are extreamly different.
> 
> 
> We can add two new rules that states
> - The orizontal steps at the last row do not add a malus $-1$ to the score
> - Both rows and columns are initialized at $0$
>  
> With these rules we are basicly removing the malus given to initial and final gaps.<br>![[Lecture 2-070 - Copy.png]]

---
##### Slides with Notes
![[Lecture 2-064.png]] ![[Lecture 2-065.png]] ![[Lecture 2-066.png]] ![[Lecture 2-067.png]] ![[Lecture 2-068.png]] ![[Lecture 2-069.png]] ![[Lecture 2-070.png]] ![[Lecture 2-071.png]]

> #IMPORTANTE ***Global and Semi-Global Alignments***:
> The Needleman-Wunsch Algorithm preferes the global alignment, but we can change it to make it return the optimal solution for local alignment: <br>![[Lecture 2-066 - Copy.png]]
> ***NOTE***: How the two alignments are extreamly different.
> 
> 
> We can add two new rules that states
> - The orizontal steps at the last row do not add a malus $-1$ to the score
> - Both rows and columns are initialized at $0$
>  
> With these rules we are basicly removing the malus given to initial and final gaps.<br>![[Lecture 2-070 - Copy.png]]