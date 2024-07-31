##### Questions
- ***What are Self Organizing Maps?***
	- **Self-Organizing Maps** (**SOM**), also known as Kohonen maps, are a type of unsupervised learning neural network that is used to ==visualize and analyze high-dimensional data==. <br>==SOMs are based on the principle of **competitive learning**, where neurons in the network compete with each other to represent different regions of the input data==.
	- ==In a SOM, the input data is mapped onto a low-dimensional grid of neurons==, where each neuron corresponds to a particular region of the input space. <br>==During training, the weights of each neuron are adjusted based on the similarity between the neuron's weight vector and the input data. <br>Neurons that are close together in the grid respond to similar patterns in the input data, while neurons that are far apart respond to dissimilar patterns==.
	- One of the key advantages of SOMs is their ability to visualize high-dimensional data in a two-dimensional space. <br>This is achieved by mapping the input data onto the grid of neurons, which allows patterns and structures in the data to be easily visualized and interpreted. SOMs have been used in a wide range of applications, including data clustering, image and speech recognition, and anomaly detection.
	- In addition to their visualization capabilities, SOMs are also useful for data compression and feature extraction. <br>By mapping the high-dimensional input data onto a low-dimensional grid of neurons, the dimensionality of the data can be reduced, while preserving the essential features and patterns in the data. This makes SOMs a powerful tool for exploratory data analysis and machine learning.
- ***What are Lateral Connections in SOMs?***
	- ==Lateral connections in Self-Organizing Maps (SOMs) refer to the connections between neurons in the grid that allow neighboring neurons to interact with each other during training==. <br>These connections play an important role in shaping the response properties of the neurons and organizing the input data into clusters or regions.
	- In a SOM, each neuron in the grid is associated with a weight vector that defines its response to the input data. <br>During training, the weights of each neuron are adjusted based on the similarity between the neuron's weight vector and the input data. <br>==However, the weights of the neighboring neurons are also affected by this adjustment process, due to the lateral connections between them==.
	- The lateral connections in SOMs are typically modeled using a **Gaussian function** that decreases with distance, so that neurons that are closer together have a stronger influence on each other than those that are further apart. <br>This means that when a neuron is activated by a particular pattern in the input data, its neighboring neurons are also activated to some extent, leading to the formation of clusters or regions in the input space.
	- ==Lateral connections in SOMs have been shown to be important for improving the accuracy and stability of the network, as well as for enhancing its ability to generalize to new data==. <br>They also allow SOMs to capture the underlying structure and patterns in the input data more effectively, and can lead to more efficient and effective learning.
- ***What is Competitive Learning?***
	- ==**Competitive learning** is a type of **unsupervised learning** in neural networks, where **neurons in the network compete with each other to respond to the input data**==. <br>In competitive learning, each neuron in the network is associated with a weight vector that determines its response to the input data. <br>During training, the weights of the neurons are adjusted based on the similarity between the neuron's weight vector and the input data.
	- ==The competition between neurons is based on a **winner-takes-all mechanism**, where only the neuron with the strongest response to the input data is activated==. <br>The activation of the winning neuron inhibits the activation of its neighbors, so that only one neuron responds to each input. <br>This competition allows the network to learn to classify and cluster the input data based on its similarities and differences.
	- Competitive learning is often used in self-organizing maps (SOMs), which are neural networks that use competitive learning to map high-dimensional input data onto a low-dimensional grid of neurons. <br>In a SOM, the competition between neurons allows the network to organize the input data into clusters or regions based on their similarities, which can be visualized in the low-dimensional space of the grid.
	- Competitive learning has also been used in other applications, such as image and speech recognition, where it is used to learn feature representations of the input data. <br>Competitive learning algorithms are often simple and computationally efficient, making them well-suited for large-scale data analysis tasks.

##### —————————————————————
##### Slides with Notes
> #IMPORTANTE **Self Organizing Maps (SOMs)**:
> The main difference between SOMs and K-Mean Clusters is in the **Update Neuron** step, where **ALL** the neurons are updated, and not just one.
> Algortihm:
> ![[Pasted image 20230110175804.png]]
> *~Ex.:*
> **START**: 
> In red are the inputs, in green and blue are the outputs (or classes).
> ![[Pasted image 20230110175932.png]]
> **Select random input** (in yellow):
> ![[Pasted image 20230110180027.png]]
> **Compute Winner Neuron**:
> The closest neuron to the random input is the green one.
> **Update Neurons**:
> **ALL THE NEURONS ARE UPDATED**, the winner neuron is updated the most, but also the other are updated **in reduced scale**.
> ![[Pasted image 20230110180130.png]]
> **Repeat the previous passages for all input data**:
> ![[Pasted image 20230110180409.png]]
> ![[Pasted image 20230110180431.png]]
> $\ldots$

![[BI - Lecture 8 - UMC-18.png]]![[BI - Lecture 8 - UMC-19.png]]![[BI - Lecture 8 - UMC-20.png]]![[BI - Lecture 8 - UMC-21.png]]![[BI - Lecture 8 - UMC-22.png]]![[BI - Lecture 8 - UMC-23.png]]
![[BI - Lecture 8 - UMC-24.png]]![[BI - Lecture 8 - UMC-25.png]]![[BI - Lecture 8 - UMC-26.png]]![[BI - Lecture 8 - UMC-27.png]]![[BI - Lecture 8 - UMC-28.png]]![[BI - Lecture 8 - UMC-29.png]]![[BI - Lecture 8 - UMC-30.png]]![[BI - Lecture 8 - UMC-31.png]]![[BI - Lecture 8 - UMC-32.png]]![[BI - Lecture 8 - UMC-33.png]]![[BI - Lecture 8 - UMC-34.png]]![[BI - Lecture 8 - UMC-35.png]]![[BI - Lecture 8 - UMC-36.png]]![[BI - Lecture 8 - UMC-37.png]]![[BI - Lecture 8 - UMC-38.png]]
