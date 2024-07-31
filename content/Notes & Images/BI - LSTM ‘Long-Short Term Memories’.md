
##### Questions
- ***What are Long-Short Term Memories (LSTMs)?***
	- **Long-Short Term Memories** (**LSTMs**) are a type of recurrent neural network architecture that is designed to address the **vanishing/exploding gradient** problem and improve the network's ability to capture long-term dependencies in sequential data.
	- At their core, LSTMs are similar to traditional recurrent neural networks in that they use feedback connections to maintain an internal memory of previous inputs. <br>==However, LSTMs include several additional components, including **memory cells** and **gating mechanisms**, that allow the network to selectively store and retrieve information over multiple time steps==.
	- The key component of an LSTM is the memory cell, which is a self-contained unit that can store information over time. <br>The memory cell is controlled by three gating mechanisms: the input gate, the forget gate, and the output gate.
		- ==The **input gate** controls how much new information is added to the memory cell==.
		- ==The **forget gate** controls how much information is retained from the previous memory state==.
		- ==Finally, the **output gate** controls how much information is read out from the memory cell to generate the network's output==.
	- Together, these gating mechanisms allow LSTMs to selectively store and retrieve information over multiple time steps, making them well-suited to tasks that require the network to remember long-term dependencies in sequential data.
	- LSTMs have been used successfully in a wide range of applications, including speech recognition, natural language processing, and time series prediction. <br>Their ability to capture long-term dependencies and avoid the vanishing/exploding gradient problem has made them a popular choice for modeling complex sequential data in deep learning.

##### —————————————————————
##### Online Resources
- [Youtube ‘Long Short-Term Memory (LSTM), Clearly Explained’ by ‘StatQuest’](https://www.youtube.com/watch?v=YCzL96nL7j0)

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 6 - NNSD-050.png]]![[BI - Lecture 6 - NNSD-051.png]]![[BI - Lecture 6 - NNSD-052.png]]![[BI - Lecture 6 - NNSD-053.png]]
![[redditsave.com_lstm_visualized-afzlbpt2ncg81.mp4]]
> **NOTE**:
> The previous hidden state $h_{t-1}$ and the input $x_t$ form a vector together that is then passed to 3 sigmoid and 1 tanh, in the GIF it is pretty cleared, but just to avoid confusion we note that $h_{t-1}$ and $x_t$ are **stacked together**.

> **FORMULAS**:
> $\bar{x}_t = [h_t \kern1px , \kern1px x_t]$ : *complete input vector*
> $f_t \propto \sigma (\bar{x}_t)$ : *forget gate*
> $i_t \propto \sigma (\bar{x}_t)$ : *input gate*
> $\bar{c}_t \propto \tanh(\bar{x}_t)$ : *candidate gate* or *read gate*
> These are not the exact formula (in fact this are **dependencies**: $\propto$ ), at each passage the LSTM cell adds a bias and multiplies the input with a vector of parameters $\bar{\theta}$.
> 
> Instead these are exact formulas:
> $c_t = f_t \odot c_{t-1} + i_t \odot \bar{c}_t$ : ***new cell state*** (where $\odot$ is element wise multiplication)
> $h_t = \tanh (c_t) \odot \sigma (\bar{x}_t)$ : ***new hidden state***

