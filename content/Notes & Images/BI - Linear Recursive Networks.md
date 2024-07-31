##### Questions
- ***What are Linear Recursive Networks?***
	- Linear Recursive Networks (LRNs) are a type of recurrent neural network architecture that is used for modeling time series data. <br>Unlike other recurrent neural networks, such as LSTMs and Elman networks, which use non-linear activation functions, LRNs use linear functions to compute the network's output.
	- ==The key idea behind LRNs is to recursively apply a linear transformation to the network's input over time, using a weight matrix that is shared across all time steps. <br>This weight matrix represents the network's memory of past inputs, and can be trained using backpropagation through time to optimize the network's performance on a given task==.
	- One advantage of LRNs is that they are relatively simple and computationally efficient, making them well-suited to problems that require fast and efficient processing of time series data. <br>However, their linear activation functions can also limit their ability to model complex and non-linear patterns in the data, and they may be less effective for tasks that require long-term memory or the ability to capture non-linear dependencies between inputs.
	- Despite these limitations, LRNs have been used successfully in a variety of applications, including speech recognition, time series prediction, and financial forecasting. <br>Their simplicity and efficiency make them a useful tool for modeling time series data, particularly in situations where computational resources are limited.

##### —————————————————————
##### Online Resources
- [Youtube ‘Recurrent Neural Networks (RNNs), Clearly Explained!!!‘ by ‘StatQuest’](https://www.youtube.com/watch?v=AsNTP8Kwu80)

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 6 - NNSD-092.png]]![[BI - Lecture 6 - NNSD-093.png]]![[BI - Lecture 6 - NNSD-094.png]]![[BI - Lecture 6 - NNSD-095.png]]![[BI - Lecture 6 - NNSD-096.png]]![[BI - Lecture 6 - NNSD-097.png]]![[BI - Lecture 6 - NNSD-098.png]]![[BI - Lecture 6 - NNSD-099.png]]![[BI - Lecture 6 - NNSD-100.png]]
