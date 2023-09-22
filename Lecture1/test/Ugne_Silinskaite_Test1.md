Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?
Cold start indicates a situation where model is faced with insufficient information to make the best prediction. In the case of booking, cold start refers to changed preferences of the users or new listings. Here the model has no previous user profile to rely on when fetching new recomendations. It has to figure out all the preferences from scratch.
2. What is the most reliable way to demonstrate a return on investment of a machine learning system?
A/B expirementation. This shows the actual impact a development has on business metrics as it compares situations with and without the development.
3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 
1.Value Performance Saturation. In the beginning as the model gets better, we can see significant improvements in the business gains. But as we develop further, there comes a point where the additional gains are too small to detect.
2.Segment saturation. When models are being improved upon each other, the smaller and smaller are the disagrements between them.  As a result of that, it is harder to see the impact on the business gains as there are only a small group of people that are being affected and treateddifferently.
3. Uncanny Valley.This refers to an inverse correlation between the acuracy of the model and the business gains. Some people might feel uncomfortable with the predictions and recomendations and stopengaging with th emodel completely.
4.Proxy Over-optimization. Proxy metrics are just indications of but not the actual business metrics. So over-optimizing them can disctract users from reaching the desirable results.
My examples will be on something very relevant - coffee. Let's say speed at which baristas make coffee is one of the proxy parameter we are improvingon in order  to get more sales. But customer satisfaction or returned customers do not only depend on that. So if we focus solely on new more efficient machines and speed of making coffee the overall experience and the times a customer returns can get lower. This will not help to improve the sales as much as expected.


4. What is git? Describe the most often used git commands?
It's a tool used for co-creating projects. It enables people to keep track of changes, get back to previous versions of the work, manage group work without chaos. 
Git checkout - switching between branches, git clone - create a copy to your device, git add - select new changes, git commit - save the changes, git pull - get code from repository, git push - send local changes to repository.

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?
The dot product is the sum of multiplied corresponding x and y. 
$\mathbf{x} \cdot \mathbf{y} = x_1 y_1 + x_2 y_2 + x_3 y_3 + \ldots + x_d y_d$
We multiple first pairs, add them to the seconds and so on for d amount of times.A more general formula would be this: \mathbf{x} \cdot \mathbf{y} = $\sum_{i=1}^{d} x_i y_i$
This operation takes two vectors and produce one number. This number represents how alighned the vectors are or how much of them point to the same direction. 
6. Explain what a vector norm is?
Vector norm is the magnitude of the vector. l1 and l2 are some of the norms (functions) that measure the lenght of the vectors.
7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?
chain rule helps to calculate derivatives of complex functions. Optimization algorithms are crucial for AI as they are used to train neural networks. But for these optimizations, derivatives are necessary. Automatic differentiation allows to automize this work and not depend on deriving formulas manually. 
8. Write the equation for a standard linear model in vector notation?
$\mathbf{y} = \mathbf{X}\boldsymbol{\beta} + \boldsymbol{\epsilon}$
9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 
$f(x) = \frac{1}{\sqrt{2\pi}\sigma} e^{-\frac{(x - \mu)^2}{2\sigma^2}}$
Examples of normally distributed data - IQ test scores, blood pressure results, height, weight scores.
10. Describe what a negative log likelihood is?
It a loss function our model optimizes. That's why we need the minus sigh. Log is to simplify the computations and likelihood shows how good our model is - hat's the propability of the observed data, given our model was correct. 
11. Write down the formula for cross-entropy loss and explain how it is used?
$L(y, \hat{y}) = -[y \log(\hat{y}) + (1 - y) \log(1 - \hat{y})]$
This formula is used for training the model and calculating the weights. This loss function compares predictions to actual data points with labels. The goal is to minimize this difference. When it's minimized, models are more accurate with the classification problems.