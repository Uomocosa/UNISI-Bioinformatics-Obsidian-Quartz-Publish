##### Questions
- ***How can we Predict the Secondary Structure of a Protein?***
	- There are several methods that can be used to predict the secondary structure of a protein from its amino acid sequence. <br>Here are a few examples:
	  1. **Chou-Fasman method**: ==This method is based on the observation that certain amino acids tend to occur more frequently in alpha helices or beta sheets==. <br>The Chou-Fasman method assigns a score to each amino acid based on its tendency to form alpha helices or beta sheets, and then uses a sliding window algorithm to predict the probability of each secondary structure element at each position along the protein sequence.
	  2. **Neural network-based methods**: ==These methods use machine learning algorithms to learn patterns in protein sequences and their associated secondary structures==. <br>The algorithm is trained on a dataset of known protein structures, and then used to predict the secondary structure of new proteins.
	  3. **Hidden Markov models** (**HMMs**): ==HMMs are statistical models that can be used to predict the probability of a particular secondary structure element based on the surrounding amino acid sequence==. <br>HMMs are trained on a database of known protein structures, and can be used to predict the secondary structure of new proteins.
	  4. **Deep learning methods**: ==These methods use deep neural networks to predict the secondary structure of a protein from its amino acid sequence==. <br>Deep learning methods can capture more complex relationships between amino acid sequences and their associated secondary structures, and have shown promising results in recent years.
	- It's important to note that secondary structure prediction methods are not always accurate, and should be used in conjunction with other experimental methods such as X-ray crystallography or nuclear magnetic resonance (NMR) spectroscopy to confirm the structure of a protein.

##### —————————————————————
##### IMPORTANTE
> #IMPORTANTE ***Prediction Accuracy for Protein Secondary Structure***: ![[Pasted image 20230113120156.png]]![[Pasted image 20230113120214.png]] 

> #IMPORTANTE Abbiamo visto 4 algoritmi per la predizione di strutture secondarie:
> 1. **Chou-Fasman** (ACCURACY: $56\%$): approccio statistico semplice, osserviamo in molte strutture secondarie i 20 amminoacidi e definiamo per ogniuno di loro delle percentuali di formare ogni struttura secondaria.
> 2. **GOR** (ACCURACY: $65\%$): anch’esso statistico, ma basato su una finestra di 17 amminoacidi.
> 3. **Stereochemical Lim**: Sfrutta le conoscenze delle propietà **idrofobiche**, **idrofiliche** ed **elettrostatiche** degli amminoacidi, ed il loro ruolo nel protein folding, per aumentare l’accuratezza ma ad un enorme costo computazionale.
> 4. **Neural Networks** (ACCURACY: $70-75\%$)

##### —————————————————————
##### Slides with Notes

![[BI - Lecture 10 - Prediction of Protein and RNA Structure-21 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-22 1.png]] ![[BI - Lecture 10 - Prediction of Protein and RNA Structure-23 1.png]]

> #IMPORTANTE ***Prediction Accuracy for Protein Secondary Structure***: ![[Pasted image 20230113120156.png]]![[Pasted image 20230113120214.png]] 

> #IMPORTANTE Abbiamo visto 4 algoritmi per la predizione di strutture secondarie:
> 1. **Chou-Fasman** (ACCURACY: $56\%$): approccio statistico semplice, osserviamo in molte strutture secondarie i 20 amminoacidi e definiamo per ogniuno di loro delle percentuali di formare ogni struttura secondaria.
> 2. **GOR** (ACCURACY: $65\%$): anch’esso statistico, ma basato su una finestra di 17 amminoacidi.
> 3. **Stereochemical Lim**: Sfrutta le conoscenze delle propietà **idrofobiche**, **idrofiliche** ed **elettrostatiche** degli amminoacidi, ed il loro ruolo nel protein folding, per aumentare l’accuratezza ma ad un enorme costo computazionale.
> 4. **Neural Networks** (ACCURACY: $70-75\%$)
