 Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

when there is not a sufficient amount of data to build a model which could make, for example, a prediction. The book emphasise that sufficient amount of data is not enough, it also has to be right data, meaning without mistakes and predictive features.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

we should first quantify the expectations that we have of the return on investment by averaging all the outcomes and weighting them by the probability of that outcome happening. Then plugg it into utility function to meassure the expected happiness of returns on investment. Where higher return means higher utility.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

1)Value performance  saturation
offline metric: page load speed
business metric: number of clients who make a purchase

users have a better experience when the page load speed ishigher, but eventually the speed becomes unimportant as the number of clients who make a purchase depends also on other factors, like the quality of the product.

2)Segment saturation
offline metric: Product market share
business metric: profit margin for the poduct

At first, when you introduce new product the profit margin is increasing as you are gaining market share, but eventually the market becomes satured and it is hard to increase the profit share further. 

3)Uncanny Valley effect 
offline metric: accuracy of personalized offers
business metric: number of clients who make a purchase according to the personalized offer

While persolized odders improves user's experience, and lets them to find what they are looking for faster, this feature might not look atractive to some costumers and they might be hessitant to provide information about themselves.

4)Proxy over-optimization
offline metric: Click-Through rate
business metric: Revenue

if we are only focusing on CTR and our goal is to maximize it, it does not neceserlly mean that the revenue will be increasing together with the CTR.

4. What is git? Describe the most often used git commands?

Git is free and open-source version control system used to track changes in the source code.

git add - tells that you will be adding changes in the file in the next commit.
git commit - records the changes made.
git push - uploades the changes youcommited to remote repository

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

the formula for the product: 
\[\mathbf{x} \cdot \mathbf{y} = \sum_{i=1}^{d} x_i y_i\]

A product of two vectors shows if these two vectors are aligned with each other, it is a sum of the products at the same position. 

6. Explain what a vector norm is?

It is a function used to measure vector's lenght.

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI models?

Chain rule allows to efficiently calculate gradients when working with deeply nested functions, in automatic differentiation it is applied backwards to calculate derivatives.

With automatic differentiation you can train models with many parameters, it makes our job easier as we don't have to calculate everything by hand.

8. Write the equation for a standard linear model in vector notation?
\[ Y = \mathbf{w}^T \mathbf{x} + b \]

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 
\[ f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x - \mu)^2}{2\sigma^2}} \]

examples: Height of adults, body temperature, blood pressure

10. Describe what a negative log likelihood is?

Negative log likelihood is a negative logarithim of the likelihood function, it is used in optimization processwhen estimating the parameters of a logistic regression model and the goal is to minimize it. 

11. Write down the formula for cross-entropy loss and explain how it is used?

\[
\text{Cross-Entropy Loss} = -\frac{1}{N} \sum_{i=1}^{N} \left[ y_i \log(p_i) + (1 - y_i) \log(1 - p_i) \right]
\]

it is used during model training to adjust model weights as a loss function for binary classification problems, it measures how well does the model predict true labels, the goal is to minimize it. 
