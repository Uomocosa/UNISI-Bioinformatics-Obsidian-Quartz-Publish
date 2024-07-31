##### Questions
- ***What are Outgroup and Ingroup?***
	- ==In phylogenetics, an **outgroup** is a group of organisms that is closely related to the group of interest (called the **ingroup**) but is not a part of it==. <br>The outgroup serves as a reference point for comparing the characteristics and relationships of the organisms within the ingroup. It allows us to determine which traits are unique to the ingroup and which are shared with the outgroup.
	- ==*For example, if we are studying the evolutionary relationships of birds, the reptiles could be an outgroup, as birds are thought to have evolved from a group of reptiles*==. <br>By comparing the traits of birds with those of reptiles, we can identify which traits are unique to birds and which are shared with their reptilian ancestors.
- ***What is the Transformed Distance Method?***
	- The Transformed Distance Method is a distance-based method used for reconstructing phylogenetic trees. <br>==It involves transforming the original distance matrix into a new matrix that satisfies certain mathematical properties, such as additivity and ultrametricity, which are necessary for constructing a valid phylogenetic tree==. <br>The method was developed to overcome some of the limitations of traditional distance-based methods, which do not always produce accurate trees, especially when the data violate the assumptions of the model. <br>The Transformed Distance Method has been shown to be more robust to violations of the model assumptions and can produce more accurate trees than traditional distance-based methods.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE In cladistics or phylogenetics, an **outgroup** is a more distantly related group of organisms that serves as a reference group when determining the evolutionary relationships of the ingroup
> ![[Pasted image 20230108124958.png]]

> #IMPORTANTE Il **Transformed distance method** basato sull’**UPGMA** algorithm fa in modo che alla fine dei conti l’albero filogenetico uscente sia **ultrametrico** (ovvero che non ci siano “shortcut” tra gli archi)
> Partiamo da una matrice **UPGMA**
> ![[Pasted image 20230107180019.png]]
> La distanza più corta è tra *ab* (17) ⇒ costruiamo i primi archi:
> ![[Pasted image 20230107180118.png]]
> Ed aggiorniamo la matrice, usando le seguenti formule:
> ![[Pasted image 20230107180258.png]]
> Usando come esempio la prima formula abbiamo:
> ⇒ $(21 + 30)/2 = 25.5$
> La risultante matrice è:
> ![[Pasted image 20230107180200.png]]
> Ripetiamo l’algoritmo, la nuova distanza minima è 22 tra *(ab)e*, il ramo che aggiungiamo dovrà tenere conto del precedente (di lunghezza $8.5$), quindi:
> ![[Pasted image 20230107180550.png]]
> La matrice va riaggiornata, e le formule questa volta saranno:
> ![[Pasted image 20230107180729.png]]
> (Nota che adesso si fa una media su 3 unità taxonomiche, e che le distanze che si usano sono sempre quelli della **matrice iniziale**)
> Oppure possiamo usare le distanze della **matrice precedente** cambiando leggermente la formula, ottenendo lo stesso risultato:
> ![[Pasted image 20230107181231.png]]
> La matrice risultante sarà:
> ![[Pasted image 20230107180629.png]]
> Distanza minore $28$ di *cd*
> ![[Pasted image 20230107180931.png]]
> Usando la **matrice precedente** per il calcolo delle nuove distanze:
> ![[Pasted image 20230107181310.png]]
> Or we can use the other formula:
> $$\frac{D_{((a,b),e),c} + D_{((a,b),e),d}}{2}$$
> Dove:
> $$D_{((a,b),e),c} = \frac{D_{ac}+D_{bc}+D_{ec}}{3} = 30$$
> $$D_{((a,b),e),d} = \frac{D_{ad}+D_{bd}+D_{ed}}{3}=36$$
> Il risultato è lo stesso: $33$
> ![[Pasted image 20230107180949.png]]
> 
> L’albero finale sarà: *(((a,b,),e),(c,d))*
> ![[Pasted image 20230107181344.png]]
> **Online resource**: [Youtube](https://www.youtube.com/watch?v=061ukTACDvY)

> La formula che utilizziamo per creare la “giusta” distanza dei rami è:
> **In caso di nodi appartenenti ad allo stesso “mega-cluster”** 
> ~Es.: $((a,b),c),e$
> $$D_{((a,b),e),c} = \frac{D_{ac}+D_{bc}+D_{ec}}{3}$$
> **In caso di nodi appartenenti a due “mega-cluster” diversi**
> ~Es.: $((a,b),e),(c,d)$ 
> In questo caso i due “*mega-cluster*” sono $((a,b),e)$ & $(c,d)$
> $$D_{((a,b),e),(c,d)}=\frac{D_{((a,b),e),c} + D_{((a,b),e),d}}{2}$$

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 4-74.png]] ![[BI - Lecture 4-75.png]] ![[BI - Lecture 4-76.png]]

> #IMPORTANTE In cladistics or phylogenetics, an **outgroup** is a more distantly related group of organisms that serves as a reference group when determining the evolutionary relationships of the ingroup
> ![[Pasted image 20230108124958.png]]

![[BI - Lecture 4-77.png]] ![[BI - Lecture 4-78.png]] ![[BI - Lecture 4-79.png]] ![[BI - Lecture 4-80.png]] ![[BI - Lecture 4-81.png]]

> #IMPORTANTE Il **Transformed distance method** basato sull’**UPGMA** algorithm fa in modo che alla fine dei conti l’albero filogenetico uscente sia **ultrametrico** (ovvero che non ci siano “shortcut” tra gli archi)
> Partiamo da una matrice **UPGMA**
> ![[Pasted image 20230107180019.png]]
> La distanza più corta è tra *ab* (17) ⇒ costruiamo i primi archi:
> ![[Pasted image 20230107180118.png]]
> Ed aggiorniamo la matrice, usando le seguenti formule:
> ![[Pasted image 20230107180258.png]]
> Usando come esempio la prima formula abbiamo:
> ⇒ $(21 + 30)/2 = 25.5$
> La risultante matrice è:
> ![[Pasted image 20230107180200.png]]
> Ripetiamo l’algoritmo, la nuova distanza minima è 22 tra *(ab)e*, il ramo che aggiungiamo dovrà tenere conto del precedente (di lunghezza $8.5$), quindi:
> ![[Pasted image 20230107180550.png]]
> La matrice va riaggiornata, e le formule questa volta saranno:
> ![[Pasted image 20230107180729.png]]
> (Nota che adesso si fa una media su 3 unità taxonomiche, e che le distanze che si usano sono sempre quelli della **matrice iniziale**)
> Oppure possiamo usare le distanze della **matrice precedente** cambiando leggermente la formula, ottenendo lo stesso risultato:
> ![[Pasted image 20230107181231.png]]
> La matrice risultante sarà:
> ![[Pasted image 20230107180629.png]]
> Distanza minore $28$ di *cd*
> ![[Pasted image 20230107180931.png]]
> Usando la **matrice precedente** per il calcolo delle nuove distanze:
> ![[Pasted image 20230107181310.png]]
> ![[Pasted image 20230107180949.png]]
> L’albero finale sarà: *(((a,b,),e),(c,d))*
> ![[Pasted image 20230107181344.png]]
> **Online resource**: [Youtube](https://www.youtube.com/watch?v=061ukTACDvY)
