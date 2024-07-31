##### Questions
- ***What is the Vanishing/Exploding Gradient Problem?***
	- The vanishing/exploding gradient problem is a common issue that can occur when training deep neural networks, particularly those that use recurrent connections or deep feedforward connections.
	- ==The problem arises when the gradients used to update the weights during backpropagation become either very small (vanishing) or very large (exploding)==.
		- When the gradients become vanishingly small, the weights may not be updated effectively, leading to slow or stalled learning.
		- Conversely, when the gradients become explosively large, the weights may be updated too aggressively, leading to unstable and erratic behavior..
	- ==The vanishing/exploding gradient problem is particularly pronounced in deep networks with many layers, as the gradients must be propagated through multiple layers before reaching the **input layer**==. <br>In such networks, the gradient can be subject to repeated multiplication or division by the same weight matrix, leading to the exponential amplification or attenuation of the gradient.
	- Several techniques have been developed to address the vanishing/exploding gradient problem, including weight initialization schemes, regularization techniques, and alternative activation functions. <br>*For example, initialization methods such as Xavier or He initialization can help to ensure that the gradients remain stable and avoid vanishing or exploding, while regularization techniques such as dropout or L2 regularization can help to prevent overfitting and stabilize the training process*.
	- Overall, the vanishing/exploding gradient problem is an important issue to consider when designing and training deep neural networks, and a variety of techniques have been developed to address it and improve the stability and effectiveness of deep learning algorithms.

##### —————————————————————
##### Online Resources
- [Youtube ‘Recurrent Neural Networks (RNNs), Clearly Explained!!!‘ by ‘StatQuest’](https://www.youtube.com/watch?v=AsNTP8Kwu80)

##### —————————————————————
##### Slides with Notes
![[BI - Lecture 6 - NNSD-048.png]]![[BI - Lecture 6 - NNSD-049.png]]