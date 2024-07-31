##### Questions
- ***What are the Recursive Models for Non-Positional Graphs?***
	- Recursive models for non-positional graphs are a type of recursive neural network that can be used to process structured data that does not have a natural positional structure, such as graphs or unordered sets.
	- Unlike traditional recurrent neural networks, which process inputs sequentially and rely on the temporal ordering of the data, ==recursive models for non-positional graphs are designed to process the entire graph structure simultaneously==, by recursively applying a set of local transition functions to each node in the graph.
	- ==The key idea behind these models is to define a set of local functions that can be applied to each node in the graph, using information from the node's neighbors to update its representation. <br>This process is repeated recursively, allowing the model to build up a global representation of the entire graph structure==.
	- There are several variations of recursive models for non-positional graphs, including **Graph Convolutional Networks** (GCNs), **Graph Attention Networks** (GATs), and **Graph Neural Networks** (GNNs), each with their own specific architectural features and use cases.
	- These models have been used successfully in a variety of applications, including social network analysis, drug discovery, and recommender systems. <br>They are particularly useful for tasks that involve processing structured data with complex dependencies and interactions, where traditional neural networks may struggle to capture the underlying patterns and relationships in the data.

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 6 - NNSD-101.png]]![[BI - Lecture 6 - NNSD-102.png]]![[BI - Lecture 6 - NNSD-103.png]]![[BI - Lecture 6 - NNSD-104.png]]
