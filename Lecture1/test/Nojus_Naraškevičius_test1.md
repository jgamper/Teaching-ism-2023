Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

When there isn't enough information from the model starting. In the book there is an example that talks about the situation when user visits the site only few times a year therefore that user's information is not relevent and model encounters cold start problem.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

The most reliable way to demonstrate a return on investment is A/B Testing.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

Value Performance Saturation, Segment Saturation, Uncanny Valley effect and Proxy Over-optimization.
Example:
Metrics - number of people that enters site per day.
Business metric - items sold.
Just because many people enters the site doesn't mean they're going to buy something.

4. What is git? Describe the most often used git commands?

Git is a version control system that tracks changes in computers files during development.
Most used: - git add + file, - git merge + branch name, - git clone, -git push, - git checkout + branch name.


5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

In words: these 2 different vectors different components are both real numbers and their dot product measures the degree to which the two vectors are aligned or point in the same direction. Negative  - negative correlated and vice versa with possitve. If they are 0, the vectors are orthogonal.
Equation: $\mathbf{x} \cdot \mathbf{y} = \sum_{i=1}^{d} x_i \cdot y_i$.

6. Explain what a vector norm is?

It shows the space of the vector.

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

It is very important in neural networks, because it saves a lot of time and helps to avoid human error.

8. Write the equation for a standard linear model in vector notation?

$\mathbf{y} = \mathbf{x}\mathbf{\beta} + \epsilon$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data?

$\documentclass{Normal Distribution formula:}
\begin{document}
\[ f(x|\mu ,\sigma^2)=\frac{1}{\sigma}\varphi\left(\frac{x-\mu}{\sigma}\right) \]
\end{document}$

10. Describe what a negative log likelihood is?

It meassures the accuracy of the model by comparing the predicted outcomes with the real ones.

11. Write down the formula for cross-entropy loss and explain how it is used?

$-\sum_{c=1}^My_{o,c}\log(p_{o,c})$
It used to check how does model perform and wheather it need to adjust the weights. It is used in the trainging period.