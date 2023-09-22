Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

**Answer 1**: Cold start is when a model encounters a difficulty (problem) when it is first deployed, meaning there is no enough amount of data or prior information. In booking this is made via an example where a customer only visits the site once or twice every year meaning that the information history of the user is not relevant. So there's not enough data and prior information is useless.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

**Answer 2**: A/B Testing the best and effective way. Like said in the article, it is the receipts for the management that the investments (developing machine learning systems) are doing something


3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

**Answer 3** :
    Value Performance Saturation - basically a business value and model performance tradeoff.
    Segment Saturation - basically oversaturating the selected population group (the ones that are exposed to a change).
    Uncanny Valley effect - basically too much informationg gathering or too accurate prediction may lead to a population suspiscions.
    Proxy Over-optimization - basically, having the best optimised list (proxy4ies) for a customer can overcomplicate them, because we have to not be irritating. (we have to make perfect conditions lol, funny.)

Let's say the most basic example:
 **Running Instagram ads for my company**
- Metric - **Click Through Rate**
- Business metric - **company's revenue**
There may have been observed of more **clicks** on the launched ads through Instagram, but this would not neccesarily reflect in the **company's revenue**. Meaning that there would be no correlation between these two things.


4. What is git? Describe the most often used git commands?

**Answer 4**: Git is a version control system that tracks changes in computers files during development.
**Most often used commands**:
- git clone + repository - creates a copy of the wanted depository on your system
- git init - initializes new repository in the current directory
- git add + file - stages changes to be commited in a file
- git checkout + branch name - switches to a different kind of branch
- git merge + branch name - combines changes from one to the other
- git commit -m - records the made changes (adds a name also)
-git push - puts the local repository to the remote one.

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

**Answer 5**: 
- In equation: $\mathbf{x} \cdot \mathbf{y} = \sum_{i=1}^{d} x_i \cdot y_i$
- In words: these 2 different vectors different components (two, if two-dimensional) are both real numbers and their dot product measures the degree to which the two vectors are aligned or point in the same direction. Negative  - negative correlated and vice versa with possitve. If they are 0, the vectors are orthogonal.


6. Explain what a vector norm is?

**Answer 6**: The vector norm is the lenght of the vector. In other words it tells us the extent of the vectors space.

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

**Answer 7**: Chain rule plays a crucial part of automatic differentiation. Especially in neural networks. In short, in neural networks - we compute the gradient loss with respect to the models parameters by propagating through gradients layers backwards.

**Why important**: it saves a lot of time and effort. Manual computation of a lot of gradients would be time-consuming and human error would be a thing. With automatic differentiation we effectively train these big and complex models. Less feature engineering?

8. Write the equation for a standard linear model in vector notation?

**Answer 8**: 
$\mathbf{y} = \mathbf{x}\mathbf{\beta} + \epsilon$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

**Answer 9**:
$\documentclass{Normal Distribution formula:}
\begin{document}
\[ f(x|\mu ,\sigma^2)=\frac{1}{\sigma}\varphi\left(\frac{x-\mu}{\sigma}\right) \]
\end{document}$

10. Describe what a negative log likelihood is?

**Answer 10**: A type of metric that measures how well models predicted probabilities match with the real outcome. Basically a way to see the performance of probabilistic models.

11. Write down the formula for cross-entropy loss and explain how it is used?

**Answer 11**: 
$-\sum_{c=1}^My_{o,c}\log(p_{o,c})$
It is used in the training period of a model, seeing how it performs and by the formula, adjusting the weights of the model.