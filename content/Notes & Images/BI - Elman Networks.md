##### Questions
- ***What are Elman Networks?***
	- ==Elman networks, also known as **Simple Recurrent Networks** (**SRNs**), are a type of **recurrent neural network** (**RNN**)== that were proposed by Jeffrey Elman in 1990. <br>They are designed to process sequential data by maintaining a memory of previous inputs using a set of recurrent connections.
	- ==Elman networks consist of three main layers: an input layer, a hidden layer, and an output layer==.
		- The input layer receives sequential data, with each input being processed one at a time.
		- ==The **hidden layer** contains a set of **recurrent connections** that allow the network to maintain a memory of previous inputs==.
		- The output layer produces a prediction or classification based on the input and the current state of the hidden layer.
	- ==In an Elman network, **the recurrent connections between the hidden layer and itself serve as a memory mechanism**==. <br>The hidden layer computes a weighted sum of the current input and the previous state of the hidden layer, and applies a nonlinear activation function to produce the current state of the hidden layer. <br>This current state is then used as the input to the next processing step.
	- One advantage of Elman networks is their relatively simple architecture, which makes them easier to train and interpret than more complex RNN architectures like Long Short-Term Memory (LSTM) or Gated Recurrent Units (GRU). <br>However, they may struggle with tasks that require long-term dependencies, as their memory mechanism is not as sophisticated as that of more advanced RNN architectures.
	- Elman networks have been used successfully in a variety of applications, including speech recognition, natural language processing, and time series prediction. <br>They remain a popular choice for researchers and practitioners working with sequential data.

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 6 - NNSD-008.png]]![[BI - Lecture 6 - NNSD-009.png]]![[BI - Lecture 6 - NNSD-010.png]]![[BI - Lecture 6 - NNSD-011.png]]