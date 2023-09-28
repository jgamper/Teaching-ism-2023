Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?
Cold start problem is a case when a model experiences newly discovered or unseen data. The model can experience insufficiency of information or make innacurate predictions.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?
We could use A/B testing, calculate costs, sensitivity analysis to see how different assumptions can impact return on investment.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics.
Dissimilar goals: improving in how things work on the inside don't always same what customers want or what the business needs at the moment.
Missing information: making things work better technically doesn't guarantee more money if other important things are missing or not done as need it.
Estimating behavior: sometimes, we guess that if we make something faster or better, people will use it more. But that's not always true. People may not notice or care.
Waiting/time for results: sometimes, changes take time to show results. For example, if we make a computer program smarter, it might take a while before it helps keep more customers.
Offline Metric: Time to bake cookies (measured in minutes)
Business Metric: Cookie sales revenue (measured in dollars)

Example: a bakery which wants to make more income by baking cookies faster. They speed up their baking process but finds out that their sales revenue doesn't go up as expected. The reason could be that customers care more about the taste and price of cookies than how quickly they are baked. So, baking faster doesn't always mean selling more cookies and making more money.

4. What is git? Describe the most often used git commands?
It's a control system which works for tracking code changes in software development, using this control system it helps to manage different versions of code, allows for several people to collaborate on the same code/project. The most used git commands are git branch, git push, git log, git diff, git clone, git add, git checkout, git status.
5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?
The dot product of two vectors estimate how much they point in the same direction. If the result will be positive, they will align; if negative, they will point in opposite directions; if zero, they will become perpendicular.
In equation: $\displaystyle\sum\limits_{i=1}^n(X_{i}\times Y_{b})$

6. Explain what a vector norm is?
A vector norm is a mathematical notion that estimates the size or length of a vector. It calculates how long or big a vector is in a given vector space.
7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?
Chain rule helps AI understand how changing one part of a formula affects the whole thing. It's like figuring out how stepping on the gas pedal changes your car's speed.
Automatic differentiation makes AI models learn faster and better. Without it, teaching AI models would be slower and harder.
It helps us create new AI models and understand them. Think of it as a handy tool for building and analyzing AI programs.
It's useful in science and engineering too, for solving problems involving change and motion.

8. Write the equation for a standard linear model in vector notation?
$\begin{bmatrix}x_{1} \\x_{2} \end{bmatrix}\begin{bmatrix}b_{1} & b_{2} \\\end{bmatrix}=\begin{bmatrix}y_{1}  \\y_{2} \end{bmatrix}$
9. Write a formula for the normal distribution? Give examples of what may be normally distributed data?
Height of adults, weight of adults, IQ scores, temparatures, test scores, ages in populations are examples of normally distributed data.
$f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x - \mu)^2}{2\sigma^2}}$

10. Describe what a negative log likelihood is?
A negative log likelihood is a method to measure how good a guess or model is at explaining real data. We want to minimize the negative log likelihood to make our guess or model as close to reality as possible. It's like trying to get the highest score in a game to show that our prediction is excellent.
11. Write down the formula for cross-entropy loss and explain how it is used?
$H(y, \hat{y}) = -\sum_{i=1}^{N} y_i \cdot \log(\hat{y}_i)$
Cross-entropy loss is a formula which is used in classification tasks to estimate how well a model's predicted probabilities go with the actual labels. It's used for training models, optimizing them, and evaluating their performance.