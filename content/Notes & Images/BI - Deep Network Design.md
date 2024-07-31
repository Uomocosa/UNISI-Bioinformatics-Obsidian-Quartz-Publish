##### Questions
- ***What is Momentum in Stochastic Gradient Descent?***
	- ==Momentum is a technique used in stochastic gradient descent (SGD) optimization to speed up the convergence of the algorithm by adding a "momentum" term to the gradient descent update equation==. <br>==The momentum term introduces a **memory** into the optimization process, which helps the algorithm to move more quickly through shallow minima and to converge more slowly towards deeper minima==.
	- In momentum-based SGD, the update rule for the parameters is modified as follows: $$\begin{align}&v = \text{momentum} * v - \text{learning\_rate} * \text{gradient} \\ & \text{parameters} = \text{parameters} + v\end{align}$$Where:
		- "$v$" is the momentum term
		- "momentum" is a **hyperparameter** between $0$ and $1$ that determines the contribution of the previous update to the current update
		- "learning_rate" is the step size of the update, and "gradient" is the gradient of the loss function with respect to the parameters.
	- The momentum term accumulates the gradients of the previous updates, which allows the algorithm to continue moving in the same direction, even if the current gradient direction changes. <br>==This helps to smooth out the updates and reduce oscillations in the optimization process==, which can improve convergence and reduce the number of iterations required to reach a minimum.
	- The momentum hyperparameter controls the contribution of the previous update to the current update, with a higher momentum value resulting in a stronger influence of the previous updates. <br>*A typical value for momentum is $0.9$, but it can be tuned depending on the problem and dataset*.
	- Overall, momentum is a useful technique for improving the convergence of stochastic gradient descent, particularly in cases where the loss function has shallow and flat regions or narrow valleys.
- ***What is the Adaptive Momentum Estimation (ADAM)?***
	- **Adaptive Moment Estimation (ADAM)** is an optimization algorithm used to update the weights of a neural network during training. <br>It is a variant of stochastic gradient descent (SGD) that combines ideas from both **momentum** and **adaptive learning** rate methods.
	- The ADAM algorithm maintains two moving averages of the gradient: the **first moment** (**mean**) and the **second moment** (**variance**). <br>These moving averages are used to estimate the adaptive learning rate and momentum terms for each weight.
		- The update rule for ADAM is given by:$$\begin{align}& m = \beta_1 \cdot m + (1 - \beta_1) \cdot \text{gradient} \\& v = \beta_2 \cdot v + (1 - \beta_2) \cdot (\text{gradient}^2) \\& \hat{m} = \frac{m}{(1 - \beta_1^t)} \\& \hat{v} = \frac{v}{(1 - \beta_2^t)} \\& \text{weight} = \text{weight} - \lambda \cdot \frac{\hat{m}}{\sqrt{\hat{v}} + \epsilon}\end{align}$$
##### —————————————————————
##### Slides with Notes
![[BI - Lecture 7 - CNN-20 1.png]]![[BI - Lecture 7 - CNN-21 1.png]]![[BI - Lecture 7 - CNN-22 1.png]]
![[BI - Lecture 7 - CNN-23 1.png]]![[BI - Lecture 7 - CNN-24 1.png]]