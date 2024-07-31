##### Questions
- ***What is Information Latching?***
	- ==Information latching is a mechanism in **recurrent neural networks (RNNs)** that allows the network to selectively store and retrieve information from its internal memory over multiple time steps==. <br>This mechanism is important for capturing long-term dependencies in sequential data, such as natural language or time series.
	- The basic idea behind information latching is to use a gating mechanism to selectively control the flow of information into and out of the memory. <br>==Specifically, the network uses a set of **gating neurons** to control the flow of information from the current input and the previous memory state into the current memory state, as well as the flow of information from the memory state to the output==.
	- In practice, information latching is typically implemented using a variant of a recurrent neural network architecture, such as a long short-term memory (LSTM) network or a gated recurrent unit (GRU) network. <br>These architectures include gating neurons that control the flow of information, as well as internal memory cells that store information over multiple time steps.
	- The key advantage of information latching is that it allows the network to selectively store and retrieve information over multiple time steps, rather than simply maintaining a fixed memory of previous inputs. <br>This makes it well-suited to tasks that require the network to remember complex dependencies over long sequences, such as machine translation or speech recognition.
	- Overall, information latching is an important mechanism in recurrent neural networks that allows the network to selectively store and retrieve information over multiple time steps, improving its ability to capture long-term dependencies in sequential data.
- ***What are the Dynamcis of a Network with Feedback?***
	- The dynamics of a neural network with feedback, also known as a recurrent neural network (RNN), can be quite complex and highly nonlinear. <br>This is because the network's internal state is constantly being updated based on its previous state and the current input, resulting in a dynamic system that evolves over time.
	- ==The dynamics of an RNN can be characterized by several properties, including stability, convergence, and oscillation==. 
		- **Stability** refers to the ability of the network's internal state to remain bounded over time
		- **Convergence** refers to the ability of the network to reach a stable state that is close to the desired output.
		- **Oscillation** refers to the tendency of the network's internal state to oscillate or fluctuate over time, which can lead to instability or unwanted behavior.
	- The behavior of an RNN with feedback depends on several factors, including the network architecture, the input sequence, and the initial state of the network. <br>==In general, RNNs with feedback can exhibit a wide range of behaviors, from simple linear responses to highly nonlinear and chaotic dynamics==.
	- One important property of RNNs with feedback is their ability to capture long-term dependencies in sequential data, such as natural language or time series. <br>This is because the network's internal state can store information over multiple time steps, allowing it to remember previous inputs and use this information to inform its processing of the current input.
	- Overall, the dynamics of a neural network with feedback are highly dependent on the specific architecture and parameters of the network, as well as the nature of the input sequence. <br>Understanding these dynamics is important for designing and training effective RNNs for a variety of applications, including speech recognition, natural language processing, and time series prediction.

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 6 - NNSD-035.png]]![[BI - Lecture 6 - NNSD-039.png]]

> **NOTE**: 
> The purple line represents the formula $y = \lambda \kern1px x + \mu$
> Where $x$ in this case represent the previous output of the neuron and $y$ the current one, so we can say: $x \propto y(t-1)$, and $y = y(t)$, for the actual formula look the previous slide.

![[BI - Lecture 6 - NNSD-040.png]]![[BI - Lecture 6 - NNSD-041.png]]![[BI - Lecture 6 - NNSD-042.png]]![[BI - Lecture 6 - NNSD-043.png]]![[BI - Lecture 6 - NNSD-044.png]]

> **NOTE**:
> As we can see this is an example on how the neuron with feedback founds a solution if it exists, in this case 3 solution exist, and the final result depends on the initial value $y_1(0)$.
> Formally this is the example of **information latching**.

![[BI - Lecture 6 - NNSD-045.png]]![[BI - Lecture 6 - NNSD-046.png]]![[BI - Lecture 6 - NNSD-047.png]]