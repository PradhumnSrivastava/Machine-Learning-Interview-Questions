# Questions Inbox
1. What is Gradient Descent in Machine Learning? Ans- Gradient Descent is an optimization algorithm used to minimize a loss function by iteratively updating model parameters in the direction opposite to the gradient of the loss.

2. Why is Gradient Descent used for training neural networks? Ans- Gradient Descent is used to find parameter values that minimize the loss function, allowing the neural network to make more accurate predictions.

3. What is the role of the learning rate in Gradient Descent? Ans- The learning rate controls the size of each parameter update. A very small learning rate makes training slow, while a very large learning rate can cause unstable training or prevent convergence.

4. What is the Gradient Descent update rule? Ans- The general update rule is θ_new = θ_old - η∇J(θ), where θ represents model parameters, η is the learning rate, and ∇J(θ) is the gradient of the loss function.

5. What is Batch Gradient Descent? Ans- Batch Gradient Descent calculates the gradient using the entire training dataset before performing each parameter update. It provides stable updates but can be computationally expensive for large datasets.

6. What is Stochastic Gradient Descent (SGD)? Ans- Stochastic Gradient Descent updates model parameters using one randomly selected training example at a time. It is computationally faster per update but produces noisier parameter updates.

7. What is Mini-Batch Gradient Descent? Ans- Mini-Batch Gradient Descent divides the training dataset into small batches and updates the model parameters after processing each batch. It provides a balance between the efficiency of batch training and the faster updates of SGD.

8. What happens when the learning rate is too small or too large? Ans- A very small learning rate causes slow convergence, while a very large learning rate can cause the loss to oscillate, diverge, or overshoot the minimum.

9. Why does Gradient Descent move in the opposite direction of the gradient? Ans- The gradient points in the direction of the steepest increase in the loss function, so moving in the opposite direction produces the greatest local decrease in loss.

10. What are common problems faced by Gradient Descent in deep learning? Ans- Gradient Descent can face problems such as vanishing gradients, exploding gradients, saddle points, local minima, slow convergence, and sensitivity to the learning rate.
