Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?
Cold start in ML occurs when insufficient historical data makes it challenging to provide recommendations. For example, on booking.com, infrequent travelers may have changed preferences when revisiting the site. New accommodations with limited content and reviews face difficulty attracting guests.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?
Demonstrating the return on investment in A/B experimentation is best achieved through conducting A/B tests. Without these experiments, recognizing the impact on investment becomes elusive.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 
a. Different Goals: Sometimes, the things we measure in the lab (like how well a machine learning model works) aren't the same as what we want in real life (like making more money).
b.Wrong Data: If we practice with the wrong kind of problems, we might not be ready for the real ones. It's like practicing basketball indoors but playing the game outdoors.
c. Too Good at Practice: Imagine you're practicing a magic trick, and you get really good at it. But when you perform it in front of others, it doesn't amaze them because you practiced too much and it became too obvious.
d. Outside Factors: Sometimes, things outside our control, like the weather affecting a picnic, can make a big difference. Similarly, external factors can mess up our machine learning plans.

4. What is git? Describe the most often used git commands?
its a platform that it allows multiple developers to collaborate on a project by keeping track of each change made to the codebase, making it easier to manage, collaborate, and maintain code.

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?
The dot product of two vectors measures how much they align with each other. It quantifies the similarity in direction between the two vectors. If the vectors are pointing in the same direction, the dot product is positive and larger. If they are perpendicular (at a 90-degree angle), the dot product is zero. If they point in opposite directions, the dot product is negative and smaller.

6. Explain what a vector norm is?
is the distance from the origin to the tip of the vector when treated as an arrow in space. 

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?
The chain rule holds a pivotal position in calculus. It serves as a foundational principle that enables us to find the derivative of a complex function by dissecting it into smaller, more manageable parts. Automatic differentiation emerges as a crucial tool in contemporary AI models due to its efficiency in computing these derivatives. It not only speeds up research and development but also simplifies the process of obtaining gradients, which are vital for training and optimizing AI algorithms.

8. Write the equation for a standard linear model in vector notation?
$ f(x) = X *  +  $

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

f(x | μ, σ^2) = (1 / (σ√(2π))) * e^(-((x - μ)^2) / (2σ^2))
Exam Scores: The distribution of scores in a well-designed test, where the test is not too easy or too hard, may approximate a normal distribution.


10. Describe what a negative log likelihood is?
 the negative log-likelihood measures how well a model's parameter values explain observed data. Minimizing the negative log-likelihood helps us find the best-fitting parameters for the model. 

11. Write down the formula for cross-entropy loss and explain how it is used?
L(y, y') = - ∑ (y_i * log(y'_i))



