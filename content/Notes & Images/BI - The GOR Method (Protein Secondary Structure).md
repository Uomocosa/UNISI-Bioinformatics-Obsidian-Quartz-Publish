##### Questions
- ***What is the GOR Method?***
	- ==The GOR (Garnier-Osguthorpe-Robson) method is a method for predicting protein secondary structure from amino acid sequence==. <br>It was developed in the early 1980s by Philippe Garnier, David Osguthorpe, and Robson Barlow.
	- The GOR method uses a statistical approach to predict the secondary structure of a protein. <br>It involves analyzing the frequency of each type of secondary structure element (**alpha helix**, **beta sheet**, or **coil**) in a training set of known protein structures, and then using this information to predict the secondary structure of a new protein based on its amino acid sequence.
	- ==The GOR method uses a sliding window of typically 17 amino acids to make the prediction. <br>At each position in the protein sequence, the method calculates the probability of each type of secondary structure based on the frequencies observed in the training set==. <br>The probabilities are calculated using a log-odds scoring scheme, which takes into account the likelihood of observing a particular amino acid in each type of secondary structure.
	- The GOR method was one of the first methods to achieve a high level of accuracy in secondary structure prediction, and it was widely used in the 1980s and 1990s. <br>However, its accuracy has since been surpassed by more sophisticated machine learning methods, such as neural networks and support vector machines.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE ***The GOR Method***:
> We take a 17-residues window: ![[Pasted image 20230113152815.png]]
> Using $4$ score matrices $17\times 20$ we calculate a score for the central residue, and we determine if it belongs to a helic, a sheet, a turn or a random coil.
> This method is more effective on $\alpha$-helics (> 65% accuracy), but less precise on $\beta$-sheets (36.5% accuracy)


##### —————————————————————
##### Slides with Notes
![[BI - Lecture 10 - Prediction of Protein and RNA Structure-31 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-32 1.png]] 