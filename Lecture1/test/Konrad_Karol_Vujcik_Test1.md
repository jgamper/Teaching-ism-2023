Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?
It is a problem where our models have a trouble predicting without much data. In the book it is explained by travelling example. If travelers only visit our website once or twice a year, the model will have hard time personalizing because human preferences change.
2. What is the most reliable way to demonstrate a return on investment of a machine learning system?
By conducting A/B experiments.
3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 
1 Value performance saturation
2 Segment Saturation
3 Uncanny Valley effect
4 Proxy overoptimization
4. What is git? Describe the most often used git commands?
Git is a distributed version control system. It can track data changes, and allows multiple people to work on the same project together
Most often used: clone, init, add, mv, rm, bisect, show, branch. merge, reset, fetch, pull, push  (atlaest the terminal shows that these are the most used :D )
5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?
Words:
The dot product of two vectors quantifies how much the vectors overlap.
Math:
X and Y are vectors
X and Y belong to R
Which has dimensions d
6. Explain what a vector norm is?
A norm is a function that maps a vector to a scalar and satisfies the following three properties:
1 Given any vector X, if we scale (all elements of) the vector by a scalar \alpha \in \mathbb{R}, its norm scales accordingly.
2 For any vectors  and : norms satisfy the triangle inequality.
3 The norm of a vector is nonnegative and it only vanishes if the vector is zero
7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?
It allows us to break down the computation of gradients for functions. AI needs gradient information for training.
8. Write the equation for a standard linear model in vector notation?
y = wX + b
w-weight
b- bias
X- input
9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 
p(x) = \frac{1}{\sqrt{2 \pi \sigma^2}} \exp\left(-\frac{1}{2 \sigma^2} (x - \mu)^2\right).
Exam scores, IQ scores, Height
10. Describe what a negative log likelihood is?
It is a metric, that helps us know how well our predictions match real data. Using the negative log formula we want values that fit our data best and minimizes the function.
11. Write down the formula for cross-entropy loss and explain how it is used?
l(\mathbf{y}, \hat{\mathbf{y}}) = - \sum_{j=1}^q y_j \log \hat{y}_j.
It is used for classification tasks. It encourages the model to be really confident about the right answer (near 1) and completely unconfident about the wrong answers (near 0) during training.
