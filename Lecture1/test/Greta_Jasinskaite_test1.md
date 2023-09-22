Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

Cold start problem in practice means that some chalenges may arise when a model or system is faced with new, unseen data. In the book there was mentioned an example about the travelers, when their preferences change, since they are traveling once or twice per year.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

To do A/B testing.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

Reasons: 1. There could be misaligned metrics, 2. Data mismatch 3. Overfitting and model complexity 4. lack of causality.
Example: e-commerce system

Offline Metric: Click-Through Rate (CTR) - The ratio of product clicks to impressions based on historical data.
Business Metric: Conversion Rate - The percentage of users who make a purchase after clicking on a recommended product.

4. What is git? Describe the most often used git commands?

Git is used in software development, often to track changes during the development. Often used commands: git push, git add, git commit -m, git clone.

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

Their dot product means, which can be espressed as x * y =+ x[i] * y[i], which in words these vectors can be expressed as the result of multiplying each corresponding pair of elements in the two vectors and then summing up these products.

6. Explain what a vector norm is?

The norm of the vector tells us how big the operators in linear algebra are. 

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

The chain rule helps to calculate derivates, when automatic differentiation works backwards through the graph.

Auomatic differentiation is important for modern AI, because it can take all the hard calculations and issues, help to not make mistakes, which were often done by calculating by hand. 

8. Write the equation for a standard linear model in vector notation?

y = x * beta + epsilon

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

p(x) = \frac{1}{\sqrt{2 \pi \sigma^2}} \exp\left(-\frac{1}{2 \sigma^2} (x - \mu)^2\right)

Examples: school grades, people's height, shoe size.

10. Describe what a negative log likelihood is?

The negative log likelihood is used to estimate the parameters of a logistic regression model. This measure shows, how well the model fits the data used to train it. 

11. Write down the formula for cross-entropy loss and explain how it is used?

−∑ 
i=1
C
 y 
i*log(y^i) 
 
 This formula is often used in clasiffication problems. It measures the dissimilarity between the predicted probability distribution and the true probability distribution of the target variable. 
