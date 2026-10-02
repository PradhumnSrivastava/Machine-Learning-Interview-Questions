# Questions Inbox
11. What is the difference between a convex and non-convex loss function for Gradient Descent? Ans- A convex loss function has a single global minimum, making optimization easier, while a non-convex loss function can contain multiple local minima, saddle points, and flat regions.

12. What is momentum in Gradient Descent? Ans- Momentum accelerates Gradient Descent by using a fraction of the previous parameter update along with the current gradient, helping reduce oscillations and move faster in consistent directions.

13. What is the difference between Gradient Descent and Momentum-based Gradient Descent? Ans- Standard Gradient Descent updates parameters using only the current gradient, while Momentum also considers previous updates to accelerate convergence and reduce oscillations.

14. What is learning rate decay in Gradient Descent? Ans- Learning rate decay gradually decreases the learning rate during training, allowing larger updates initially and smaller, more precise updates as the model approaches a minimum.

15. What is an epoch in Gradient Descent? Ans- An epoch represents one complete pass through the entire training dataset. In Mini-Batch Gradient Descent, multiple parameter updates are usually performed during one epoch.

16. What is the difference between an iteration and an epoch? Ans- An iteration generally represents one parameter update, while an epoch represents one complete pass through the entire training dataset. With mini-batches, one epoch contains multiple iterations.

17. Why is feature scaling important for Gradient Descent? Ans- Feature scaling puts features on comparable scales, which can make the loss surface better conditioned and help Gradient Descent converge faster and more efficiently.

18. What is a saddle point in Gradient Descent? Ans- A saddle point is a point where the gradient can be zero but the point is neither a local minimum nor a local maximum. In high-dimensional neural networks, saddle points can slow optimization.

19. How does batch size affect Gradient Descent? Ans- A larger batch size generally produces more stable gradient estimates but requires more memory, while a smaller batch size produces noisier updates but can require less memory and may sometimes help optimization escape flat or unfavorable regions.

20. How can Gradient Descent be improved for faster and more stable training? Ans- Gradient Descent can be improved using techniques such as Momentum, RMSProp, Adam, learning-rate scheduling, proper weight initialization, feature scaling, and appropriate batch sizes.
