# AML_2019 Coursework, Part 1, Group 13
<b>1. Why is gradient descent important in machine learning?</b> 
<br>
Gradient descent is important in machine learning because it is used to minimize the cost function efficiently. In machine learning, there is usually a loss function (called loss function, which we will call the objective function objection function). We usually want this function to be as small as possible (that is, to find the minimum value). Each time a model is created (for example drawing best-fit a line across all that captures most of data points), we have to validate its performance. This is done by coming up with a cost function such as mean square error (the difference between the predicted values and the actual values). In order to fit the best model, we need to minimize that cost function. Intuitively this results in the model which predicts with the smallest error. 
<br>
<br>

<b> 2. How does vanilla gradient descent work:</b>
<br>
Vanilla gradient descent works by stepping iteratively in the direction of the negative gradient of the cost function until a local minimum is found. This is when the slope reaches as close to zero as possible – usually defined by a tolerance variable such as 0.00001.
“Stepping iteratively” means continuously updating the parameters of the cost function by adding the step size multiplied by the negative gradient to each parameter and recalculating the new gradient. The size of each step is called the learning rate. 
The main challenges of vanilla gradient descent includes: 
1.	Taking too large steps may miss the minimum
2.	Taking too small steps results in the algorithm taking too much time and computational effort
3.	It can get stuck at saddle points
<br>
<b>3. Two modifications to plain vanilla gradient descent</b>
<br>
•	Momentum gradient descent takes into account the previous step and assigns a weight between the previous step and current gradient for each parameter update in gradient descent. This allows the gradient descent to be much smoother.

•	Nesterov’s accelerated gradient descent builds upon the momentum method, by looking ahead and adjusting the step if the gradient flattens or changes sign at the look ahead point. This prevents the overshooting problem.  


# Experiments with Gradient Descent

For our project part 1, we apply vanilla gradient descent, gradient descent with momentum and gradient descent with Nesterov’s accelerated gradient descent to the function:
