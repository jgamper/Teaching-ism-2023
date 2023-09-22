\usepackage{amsmath}
Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?
A cold start in machine learning describes a situation where we are starting from scratch, meaning we have a very limited amount of information. There is a scarcity of data, based on which we can have a reliable model. What we do in this case is design an in initial model which cannot really do anything useful, we then introduce it to some initial low levels of data and see how our model performs, we then tweak the knobs to make the model perform better assed on those examples, we then grab more new data and continuously udpate the model and see if we are improving it or making it worse, aswe then have new and new data, we can make the model better. Sometimes, however, it is difficult to even gather enough data.Booking provided an example where a customer visits the site very rarely, meaning that the history of use for the user is not relevel, so there is not enough data and earlier information does not provide any reliable use as people's preferences may have changed.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?
An effective measure is A/B testing, offline evaluation of a model is not enough. Fo a CFO to go with a suggested ML model, he needs to see that it will yield a good enough financial return, it shows the management team that the invesmtent in the model will yield a return

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 
    1) Value performance saturation - If we for example want to reduce pollution levels, it may make a lot of sense to do that initially if we have high initial levels of pollution which impact both the length and quality of life of our population, but f.e. by reducing each additional ton of CO2 emissions, our costs associated with the reduction become higher and at some point, while our models still shows ways of how we can reduce (gain additional performance) the levels of pollution, in a real world (or business) sense the gains are negligible and no longer worth pursuing as they are too costly
    2) Segment Saturation - again here, if we have models competing against one another and they are improving, the better the model gets, the smaller the treatment group will be and so our models will effect less people, and we will be able to make less gains, making it too expensive to continue competing. Here as well the pollution argument as example holds, we can come up with more efficient models to lower pollution, but at some point the gains will be too small to justify their need
    3) Uncanny value effect -if we have a powerful model, it can get unsettling for customers to see suggestions or feed for content based on what they have not yet indicated they like to watch on social media which could be unsetteling for customers, making them think that there is too much information being collected about them, making them leave the service
    4) Proxy Over optimization - if we over optimize some sort of proxy/variable, like f.e. time spent on a particular social media app, it could lead to people drowning in content that perhaps they are not interested in the feed, but have to go trhough before getting to what they like, leaving them upset about their experience and eventually making them leave the platform which hurts the business

4. What is git? Describe the most often used git commands?
Git  is a control system that tracks changes in any set of computer files, usually used for coordinating work among programmers (working on the same codebase) who are collaboratively developing source code during software development. Here are some of the most frquently used commands: 1) git init: Initializes a new repository in the current directory.
2)git clone: Creates a copy of a remote repository on your local machine.
3)git add: Stages changes which will be commited in a file.
4)git commit: Records changes to the repository with a commit message.
5)git push: Pushes local commits to a remote repository.
6)git checkout: Switches between branches or commits.
7)git log: Displays the commit history, showing details of previous commits.

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?
$\mathbf{x} \cdot \mathbf{y} = \sum_{i=1}^{d} x_i \cdot y_i$
These are two different vectors and the dot product shows the degree to which the two vectors are aligned or point in the same direction.

6. Explain what a vector norm is?
Informally, the norm of a vector tells us how big it is - the length of the vector. For instance, the l2 norm measures the (Euclidean) length of a vector. A norm is a function that maps a vector to a scalar and satisfies the following three properties: 1) Given any vector x, if we scale (all elements of) the vector by a scalar, its norm scales accordingly. 2) For any vectors x and y norms satisfy the triangle inequality. 3) The norm of a vector is nonnegative and it only vanishes if the vector is zero

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?
In deep learning frameworks, when we pass data through each successive function, the framework builds a computational graph that tracks how each value depends on others. To calculate derivatives, automatic differentiation works backwards through this graph applying the chain rule. Automatic differentiation is important because as working on calculations by hand can be difficult and you are likely to make a mistake and these issues become bigger as our models become bigger and more complex which is why it is good to automate it.

8. Write the equation for a standard linear model in vector notation?
$y=x\beta+\varepsilon$


9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 
$f(x)=\frac{1}{\sigma \sqrt{2\pi }}e^{-\frac{1}{2}}\left ( \frac{x-\mu }{\sigma } \right )^{2}$

Normally distrubuted example is height in the adult population, the average height between females and males has been found to be around 175cm. However, of course there are outliars.

10. Describe what a negative log likelihood is?
The negative-log-likelihood function is used to estimate the parameters of a logistic regression model. It’s a measure of how well the model fits the data used to train it. The objective of logistic regression is to find the set of parameters that maximizes the NLL function. The negative-log-likelihood function is defined as the negative logarithm of the likelihood function. The likelihood function measures the probability of observing the training data given the model parameters. By taking the negative logarithm of the likelihood function, we convert the multiplication of probabilities into an addition of logarithms, which makes it easier to optimize using gradient descent.

11. Write down the formula for cross-entropy loss and explain how it is used?
$L(y,\hat{y})=-\sum_{i=1}^{C}y_{i}log(\hat{y_{i}})$
Cross-entropy is used to optimize classification models. Cross-entropy loss measures the performance of a classification model whose output is a probability value between 0 and 1. Cross-entropy loss increases as the predicted probability diverges from the actual label. It is used in the training period
