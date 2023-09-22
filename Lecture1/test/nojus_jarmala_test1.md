Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

Cold start problem in Machine Learning is when the system cannot draw any inferences for users or items about which it has not yet gathered sufficient information or information is too old to use. Examples in the booking.com website are given that people only travel once or twice a year and by the time they come back to the same website, their preferences could have changed significantly. Long in the past history of users is actually irrelevant. Furthermore, new types of acommodations are added everyday, their lack of review and general content such as photos, descriptions, etc., make it difficult to give them much of visibility.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

The most reliable way to demonstrate a return on investment of a machine learning system are A/B experiments, through which business impact has to be made and present. 

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

The main 4 reasons for lack of correlation between offline performance gain and business value gain are:

Value Performance Saturation - there are business problems for which it is not possible to drive value from model performance gains indefinitely.
Segment Saturation - as models improve on each other, the disagreement rate goes down, reducing the population of users that are actually exposed to a treatment, and with that, the power to detect gains in value.
 Uncanny Valley Effect - models that have high accuracy may result negatively on business value gain due to the fact that it is unsettling for people to be predicted themselves so well as they feel invased or that the models "know" them too well.
Proxy Over-optimisation - over-optimizing proxies leads to distracting the users away from their goals.

Example - let's imagine a social media platform who aims to improve user engagement through its recommnedation algorithms. Company focus on enhancing offline metrics, namely click-through rates and user engagement proxies. At first, optimization of these metrics lead to increase in number of clicks and interaction that then lead to higher user engagement score. However, this boost does not necessarily translates to business value because even if people click on the sensationalized content or provocative headlines, people may not engage in subscriptions or purchases of personalized content. It then may lead to a decline in the quality of content and user experience, causing some users to disengage or even leave the platform. This would result in decline of conversion rate as well as user retention rate within the platform. 

4. What is git? Describe the most often used git commands?

Git is a distributed version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers who are collaboratively developing source code during software development. Its goals include speed, data integrity, and support for distributed, non-linear workflows.

The most common git commands and their descriptions:
git init - initializes a new Git repository in the current directory.
git clone - creates a copy of a remote repository on a local machine.
git add - includes changes of files into the next commit.
git commit - records changes to the repository with a commit message describing what was done.
git status - shows the current status of user's working directory, including which files are modified, staged, or untracked.
git pull - fetches changes from a remote repository and merges them into a local branch.
git push - pushes user's local changes to a remote repository. 
git checkout - switches to a different branch.
git config - lets users to specify, update or add their username and email that will be used with the commits. 
git merge - merges and combines the work done in different branches. 
git branch - allows to list, create, delete and manage branches. 


5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

$$\mathbf{x} \cdot \mathbf{y} = \sum_{i=1}^{d} x_i y_i$$


The dot product is a mathematical operation that combines these vectors in a way that measures how similar they are in direction. In other words, it quantifies the degree to which the vectors align with each other.

6. Explain what a vector norm is?

Norms capture various notions of the magnitude of a vector and are commonly applied to the difference of two vectors to measure their distance apart. Informally, the norm of a vector tells us how “big” it is. A norm is a function  that maps a vector to a scalar and satisfies the following three properties:
1. If all elements of the vector are scaled by a scalar, its norm scales accordingly.
2. Norms satisfy the triangle inequality
3. The norm of a vector is nonnegative and it only vanishes if the vector is zero. 

Common vector norms include the l1 and l2 norms. For instance, the l2 norm measures the (Euclidean) length of a vector. Here, we are employing a notion of size that concerns the magnitude of a vector’s components (not its dimensionality). The L1 norm is a vector norm (also known as the "Manhattan norm") used to measure the size or magnitude of a vector in a more "taxicab-like" manner compared to the Euclidean norm (L2 norm). While the L2 norm calculates the straight-line distance from the origin to the vector's endpoint, the L1 norm calculates the distance as if traveling along the edges of a grid or city blocks. 

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

Calculating derivatives is a crucial step in all the optimization algorithms that we use to train deep networks. While the calculations are straightforward, working them out by hand can be tedious and error-prone, thus fortunately all modern deep learning frameworks take this work off our hands by offering automatic differentiation. That is why it is so important for modern AI models. As we pass data through each successive function, the framework builds a computational graph that tracks how each value depends on others. So the role of the chain rule in automatic differentiation is: during the calculations of derivatives, automatic differentiation works backwards through computational graph applying the chain rule. 

8. Write the equation for a standard linear model in vector notation?

$y = \beta_0 + \beta_1 x_1 + \beta_2 x_2 + \ldots + \beta_p x_p + \varepsilon$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

$f(x | μ, σ^2) = \frac{1}{\sigma \sqrt{2\pi}} \, e^{-\frac{(x - μ)^2}{2\sigma^2}}$

Examples of normally distributed data can be: weights, heights, IQ scores, test scores, shoe sizes, etc.

10. Describe what a negative log likelihood is?

A negative log likelihood is a way to measure how well a statistical model, like a machine learning model, predicts the likelihood of observed data. It's "negative" because we want to minimize it, meaning that we want our model to be good at making accurate predictions. So, the lower the negative log likelihood, the better your model's predictions match the real data.

11. Write down the formula for cross-entropy loss and explain how it is used?

$\text{Binary Cross-Entropy Loss} = -\left(y \cdot \log(p) + (1 - y) \cdot \log(1 - p)\right)$

Cross-entropy loss measures the difference between predicted probabilities and actual outcomes in classification problems. It quantifies how well a model's predictions align with the true labels of a dataset. The goal is to minimize this loss during the training process, which essentially means making the model's predictions as close as possible to the actual labels.