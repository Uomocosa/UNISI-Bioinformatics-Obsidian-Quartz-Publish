##### Questions
- ***What is Protein-Protein Interaction?***
	- ==**Protein-protein interactions** (**PPIs**) are the physical contacts between two or more proteins that occur within a cell or organism==. <br>PPIs play a critical role in many biological processes, including signal transduction, gene expression, and metabolism.
	- PPIs can occur through a variety of mechanisms, including the formation of stable complexes, transient interactions, and post-translational modifications. PPIs can also be modulated by a variety of factors, including cellular environment, post-translational modifications, and the presence of other interacting molecules.
	- ==PPIs can be studied using a variety of experimental techniques, including co-immunoprecipitation, yeast two-hybrid assays, and protein microarrays==. <br>In recent years, computational methods, such as molecular docking and machine learning algorithms, have also been developed to predict and analyze PPIs.
	- Understanding PPIs is essential for understanding many biological processes and for developing new drugs and therapies. <br>PPIs are also the focus of intense research in fields such as network biology and systems biology, which seek to understand the complex interactions between biomolecules within a cell or organism.
- ***How can we Predict Post-Translation Modifications?***
	- ==**Post-translational modifications** (**PTMs**) are covalent modifications of proteins that occur after translation, and they play important roles in protein function and regulation==. <br>PTMs can include **phosphorylation**, **acetylation**, **methylation**, **ubiquitination**, and many others. <br>Predicting PTMs can be challenging, as they can be site-specific and can occur at multiple residues within a protein.
	- There are several computational methods and tools that can be used to predict PTMs:
	  1. **Sequence-based prediction**: ==This method involves analyzing the amino acid sequence of a protein to predict PTM sites==. <br>Several tools, such as NetPhos, NetAcet, and GPS-SUMO, use machine learning algorithms to predict PTM sites based on sequence features such as amino acid composition, sequence motifs, and structural properties.
	  2. **Structure-based prediction**: ==This method involves analyzing the 3D structure of a protein to predict PTM sites==. <br>Structural features such as solvent accessibility, surface electrostatics, and hydrogen bonding patterns can be used to predict PTM sites. Several tools, such as iGPS and EzyPred, use structure-based prediction methods.
	  3. **Combination of sequence and structure-based prediction**: This method combines both sequence and structural features to predict PTM sites. <br>For example, the tool KinasePhos combines sequence motifs and structural features to predict phosphorylation sites.
	- It is important to note that PTM prediction tools have limitations, and experimental validation is necessary to confirm predicted PTM sites. <br>Additionally, PTMs can be context-dependent and can be affected by cellular environment and signaling pathways, which can make prediction challenging. Therefore, a combination of experimental and computational approaches is often used to study PTMs.

##### —————————————————————
##### IMPORTANTE

> #IMPORTANTE **Protein-Protein Interaction**:
> P-P interactions are characterized as **stable** or **transient**, also a P-P interaction can be either **weak** or **strong**:
> - ***Stable P-P Interactions***: Permanent interaction, (like a fusion of two proteins)
>   Some examples are: *Hemoglobin*, *RNA Polymerase*.
> - ***Transient P-P Interactions***: Temporary interaction, typically this interaction **requires a set of condition that promote the interaction** (*~ex.:* phosphorylation).
> - **Weak, Strong P-P Interactions**: the strength of the interaction is determined by the **size of the binding domain** (by how many peptides), also note that P-P iteractions are kept togheter by *hydrophobic bonds*, *van der Waals forces* or *salt bridges*.
> 
> The tetrary structure of a protein can be useful: given the 3D structure of a protein we can use ML to predict which residues are most likely involved in protein-protein interactios.
> For each residue in the surface (or close to it) we can extract a number of useful featues, to be used in a ML framework:
> - Number of residues within a given radius.
> - Net charge of the residue and of the neighboring residues.
> - Hydrophobicity level.
> - Potential of the hydrogen bonds.
> 
> We can then pass two features vectors, each corresponding to a residue of two different proteins, and the NN will give use a score for which the two residues will form a P-P interaction.
> 
> Protein interaction networks evolve over time and can suffer spontaneus alterations, occasioanl shifts are often associated with diseases conditions, noticing these changes can be hugly beneficial.
> The goal is to create extreamly specific medicine to combact these changes, or more generally, to have a better understand how target compounds can interact with a protein we insert in the body, via drugs.
> 
> #IMPORTANTE **Post-Translation Modification Prediction**
> ==*Proteins are subjected to many modification also after being translated*==
> So we need another field of study that can help use better understand the life cycle of proteins and how we can use them to our advantage.
> Some of the post-traslation modification are:
> - **Removal of protein segments**
> - **Formation of covalent bonds**, between residues and sugars, or phophate and sulphate groups.
> - **Formation of cross-links**, involving (possibly far) residues within a protiens (disulfide bonds)
> 
> ==Many of these modification are carried out by other proteins.==

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 11 - Proteomics Tools and Applications-100.png]] ![[BI - Lecture 11 - Proteomics Tools and Applications-101.png]] ![[BI - Lecture 11 - Proteomics Tools and Applications-102.png]] ![[BI - Lecture 11 - Proteomics Tools and Applications-103.png]] ![[BI - Lecture 11 - Proteomics Tools and Applications-104.png]]    
