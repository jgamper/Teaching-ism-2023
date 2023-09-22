Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

It means that there are not enough data. The example from booking.com is that customers are in a continuous 'cold start' because their choices and preferences be completely different than last year or half a year ago so their old purchases can be irrelevant

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

A/B testing is one of the best ways to compare ROI because it compares two different models

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

a)Value performance saturation
b)Segment saturation
c)Uncanny Valley effect
d)Proxy over-optimization

Some of the most common examples are recommendation systems. For example, TV series or movies recomendation system. Offline metric is a number of available moveis or TV series on a platform (e.g., Netflix, HBO, etc.). Business metric is revenue gained from new or continued subscriptions

4. What is git? Describe the most often used git commands?

Git is a control system track changes in source code. The most often used commands are:
git add - adds files to a directory
git commit - commits the changes made
git init - initiates a new git directory
git clone - creates a copy of a git repository


5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

Dot product of vectors x and y is: $ x_1 * y_1 + x_2 * y_2 + ... + x_n * y_n $
Dot product calculates how much vectors point towards same direction

6. Explain what a vector norm is?

Vector norm is a length of a vector

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

It plays a major role. The chain rule is a fundamental concept in calculus and it allows you to compute the derivative of a composite function by breaking it down into simpler derivative calculations.
Automatic differentiation is important for modern AI models because it provides an efficient way to make these gradients. It also helps make R&D faster

8. Write the equation for a standard linear model in vector notation?

$ Y = X * $\beta$ + $\epsilon$ $

$\beta$ - vector of coefficients
X - the matrix
ε - error term

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

$p(x) = e^((-x - \mu)^2 / 2 * (\sigma ^ 2)) / \sigma * \sqrt(2 * \pi)$

One of the most popular examples of normally distributed data is human IQ since it follows the normally distributed pattern

10. Describe what a negative log likelihood is?

It is a loss function in ML. It shows how good statistical model's predictions compare with observed data

11. Write down the formula for cross-entropy loss and explain how it is used?

There are formulas for binary or multiclass classification. I will talk about multiclass classification formula

$ L(y, p) = - (sum_{n = 0}^{i}(y_i) * log(p_i))
y - can hold values of 1 and 0 only
p - predicted probability

It is used to evaluate models, train them and compare the models