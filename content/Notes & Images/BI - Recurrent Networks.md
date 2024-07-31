##### Questions
- ***What are Recurrent Networks?***
	- ==Recurrent networks are a type of neural network that are designed to process sequential data, such as time series or natural language. <br>Unlike feedforward neural networks, which process each input independently, recurrent networks maintain an internal memory of previous inputs and use this memory to inform the processing of the current input==.
	- The key feature of recurrent networks is the use of **recurrent connections**, which allow information to flow from one time step to the next. <br>Specifically, at each time step, the network receives an input and produces an output, as well as updating its internal state based on the current input and the previous state. This internal state is then used to inform the processing of the next input.
	- There are several types of recurrent networks, including Elman networks, Jordan networks, and more advanced architectures such as Long Short-Term Memory (LSTM) networks and Gated Recurrent Units (GRUs). <br>These networks differ in the way they use recurrent connections to maintain and update their internal memory, and in the way they process the current input based on this memory.
	- Recurrent networks have been successful in a variety of applications, including speech recognition, natural language processing, and time series prediction. <br>However, they can be more difficult to train than feedforward networks, due to the challenge of propagating gradients through the recurrent connections over long sequences. <br>Techniques such as gradient clipping, weight regularization, and truncated backpropagation through time are often used to address these issues.

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 6 - NNSD-016.png]]![[BI - Lecture 6 - NNSD-017.png]]![[BI - Lecture 6 - NNSD-018.png]]![[BI - Lecture 6 - NNSD-019.png]]

- ***RNN: Recurrent Neural Network***

![[BI - Lecture 6 - NNSD-020.png]]![[BI - Lecture 6 - NNSD-021.png]]

- ***MLP: Multilayer Perceptron*** (A simple Neural Network with $0-n$ hidden layers)

![[BI - Lecture 6 - NNSD-022.png]]![[BI - Lecture 6 - NNSD-023.png]]![[BI - Lecture 6 - NNSD-024.png]]![[BI - Lecture 6 - NNSD-025.png]]![[BI - Lecture 6 - NNSD-026.png]]![[BI - Lecture 6 - NNSD-027.png]]