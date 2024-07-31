##### Questions
- ***What are the Proximity Relation Methods?***
	- Proximity relation methods are a family of methods used to construct phenograms, which represent the relationships between species or other taxa based on molecular data. <br>==These methods use the idea that the similarity of the molecular data reflects the degree of evolutionary divergence between the taxa==.
	- ==In proximity relation methods, the pairwise distances between taxa are calculated, and these distances are then used to construct a tree that reflects the relationships between the taxa==. <br>There are several different methods for calculating these pairwise distances, including the Jukes-Cantor model, the Kimura 2-parameter model, and the Tajima-Nei model.
	- ==One common type of proximity relation method is the neighbor-joining method, which is a fast and efficient algorithm for constructing phenograms==. <br>This method begins by calculating the pairwise distances between taxa, and then uses these distances to identify the pairs of taxa that are most closely related. These pairs are then joined together to form internal nodes in the tree, and the process is repeated until the entire tree is constructed.
	- Other proximity relation methods include the Fitch-Margoliash method, which minimizes the sum of squared differences between observed and predicted distances, and the minimum evolution method, which selects the tree that requires the fewest number of evolutionary changes.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE 
> ![[Pasted image 20230107184139.png]]
> La distanza è calcolata nel seguente modo:
> $d_{AC} = a + e + c$
> $d_{BC} = b + e + c$
> $d_{AB} = a + b$
> #IMPORTANTE **Four-Points conditions**:
> ![[Pasted image 20230107184319.png]]
> Si intende che non ci sono scorciatoie e che la distanz $2e$ deve essere **positiva**.
> 
> #IMPORTANTE Il **Proximity relation method** si basa su prendere $f$ foglie.
> 1. Creaiamo tanti *set* di foglie in **tutte le possibili** combinazioni di 4 foglie diverse
> 2. Per ogni set di cui avremo all’interno quindi 4 foglie, che noi chiameremo con $A$, $B$, $C$, $D$, calcoliamo le seguenti somme:
> $$d_{AB} + d_{CD} \kern{10px},\kern{10px} d_{AC} + d_{BD} \kern{10px},\kern{10px} d_{AD} + d_{BC}$$
> 3. #NOT_SURE_ABOUT_THIS Prendiamo solo la somma delle tre con il totale più passo (per esempio mettiamo che per il $i$ set sia $d_{AB}^{i} + d_{CD}^{i}$), fatto questo per tutti i set prenderemo la somma globale più bassa.
> 4. Ripetiamo il processo  ricalcolando le distanze e ricreando tutti i set.

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 4-82.png]] ![[BI - Lecture 4-83.png]] 

> #IMPORTANTE 
> ![[Pasted image 20230107184139.png]]
> La distanza è calcolata nel seguente modo:
> $d_{AC} = a + e + c$
> $d_{BC} = b + e + c$
> $d_{AB} = a + b$
> #IMPORTANTE **Four-Points conditions**:
> ![[Pasted image 20230107184319.png]]
> Si intende che non ci sono scorciatoie e che la distanz $2e$ deve essere **positiva**.
> 
> #IMPORTANTE Il **Proximity relation method** si basa su prendere $f$ foglie.
> 1. Creaiamo tanti *set* di foglie in **tutte le possibili** combinazioni di 4 foglie diverse
> 2. Per ogni set di cui avremo all’interno quindi 4 foglie, che noi chiameremo con $A$, $B$, $C$, $D$, calcoliamo le seguenti somme:
> $$d_{AB} + d_{CD} \kern{10px},\kern{10px} d_{AC} + d_{BD} \kern{10px},\kern{10px} d_{AD} + d_{BC}$$
> 3. #NOT_SURE_ABOUT_THIS Prendiamo solo la somma delle tre con il totale più passo (per esempio mettiamo che per il $i$ set sia $d_{AB}^{i} + d_{CD}^{i}$), fatto questo per tutti i set prenderemo la somma globale più bassa.
> 4. Ripetiamo il processo  ricalcolando le distanze e ricreando tutti i set.

![[BI - Lecture 4-84.png]] ![[BI - Lecture 4-85.png]]
