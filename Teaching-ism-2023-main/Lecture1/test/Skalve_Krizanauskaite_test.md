Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?
"Cold start" is a problem in computer-based information systems when the system can't make predictions or recommendations for new users or items because it lacks enough data about them.
2. What is the most reliable way to demonstrate a return on investment of a machine learning system?
In summary, the most reliable way to demonstrate of investment for a machine learning system is to use a structured approach that considers not only the accuracy of predictions but also the costs associated with mistakes and manual review
3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 
1. Different Goals: Improvements in how things work on the inside don't always match what customers want or what the business needs.
2. Missing Information: Making things work better technically doesn't guarantee more money if other important things are missing or not done right.
3. Guessing Behavior: Sometimes, we guess that if we make something faster or better, people will use it more. But that's not always true. People may not notice or care.
4. Waiting for Results: Sometimes, changes take time to show results. For example, if we make a computer program smarter, it might take a while before it helps keep more customers.

Offline Metric: Time to bake cookies (measured in minutes)
Business Metric: Cookie sales revenue (measured in dollars)

Imagine a bakery that wants to make more money by baking cookies faster. They speed up their baking process but find that their sales revenue doesn't go up as expected. The reason could be that customers care more about the taste and price of cookies than how quickly they are baked. So, baking faster doesn't always mean selling more cookies and making more money.

4. What is git? Describe the most often used git commands?
Git is a crucial tool for software development, helping teams track code changes, manage different versions of code, and collaborate effectively. Some commonly used Git commands include "git branch," "git push," "git log," "git diff," "git clone," "git add," "git checkout," and "git status."
git branch: Shows a list of branches and lets you create new ones.
git push: Uploads local changes to a remote repository.
git log: Displays a history of commits in the repository.
git diff: Compares changes between different versions of files.
git clone: Creates a copy of a remote repository on your local machine.
git add: Stages changes for a commit.
git checkout: Switches between branches or commits.
git status: Shows the current status of your working directory and staged changes.


5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?
The dot product of two vectors, represented as $\mathbf{x}$ and $\mathbf{y}$ in ℝᵈ, quantifies how much they share the same direction. A positive result indicates alignment, a negative result signifies opposite directions, and a result of zero means they are perpendicular (90 degree angle)
In equation: $\displaystyle\sum\limits_{i=1}^n(X_{i}\times Y_{b})$

6. Explain what a vector norm is?
It is a mathematical notion that estimates the size or length of a vector. It calculates how long or big a vector is in a given vector space.

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

Role of Chain Rule in Automatic Differentiation:
Chain rule helps AI understand how changing one part of a math formula affects the whole thing. It's like figuring out how stepping on the gas pedal changes your car's speed.
Why Automatic Differentiation Matters for AI:
Automatic differentiation makes AI models learn faster and better. Without it, teaching AI models would be slow and hard.
It helps us create new AI models and understand them. Think of it as a handy tool for building and analyzing AI programs.
It's useful in science and engineering too, for solving problems involving change and motion.

8. Write the equation for a standard linear model in vector notation?

$\begin{bmatrix}x_{1} \\x_{2} \end{bmatrix}\begin{bmatrix}b_{1} & b_{2} \\\end{bmatrix}=\begin{bmatrix}y_{1}  \\y_{2} \end{bmatrix}$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

Normally distributed data can be IQ scores, heights and weights of adults, blood pressure measurements and test scores.
 $f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x - \mu)^2}{2\sigma^2}}$

10. Describe what a negative log likelihood is?
A negative log likelihood (NLL) is a way to measure how good a guess or model is at explaining real data. We want to minimize the NLL to make our guess or model as close to reality as possible. It's like trying to get the highest score in a game to show that our prediction is excellent.

11. Write down the formula for cross-entropy loss and explain how it is used?
$H(y, \hat{y}) = -\sum_{i=1}^{N} y_i \cdot \log(\hat{y}_i)$

Used in classification tasks to see how well model's guesses match the real answers. It helps to see how effective is the model and if it needs the improvement.
