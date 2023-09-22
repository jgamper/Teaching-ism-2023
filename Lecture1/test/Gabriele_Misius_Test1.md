Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 
...

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

The cold start problem is an issue related to the lack of historical data when a ML model or system is initialized or when a model encounters new data, especially in recommender systems. Thus, the output (predictions or recommendations) that the model makes can be inaccurate. 

In the case of Booking.com, they encounter a cold start problem as well since some people travel rarely, so by the time they visit the website again, their preferences might chnage completely. Thus, the model has to figure some preferences from scratch again. Also, new accomodations are added daily, so it is difficult to make them visible at first (lack of reviews, picture, etc.), so this is a problem of new data.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

There could be many ways but the most reliable is AB experimentation since it compares and experiments with different models and their effects. This method has proven to be very efficient for many companies like Airbnb, Netflix, Facebook and the positive results of this has helped to increased the budget for ML teams. 

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

1) Value Performance Saturation: Some business problems reach a point where improving model performance doesn't bring significant benefits anymore.
2) Segment Saturation: as models improve, the population of users exposed to treatment can decrease along with the power to detect gains in value.
3) Uncanny Valley effect: as models improve, they know more about the user and this can be uncomfortable for some of the users.
4) Proxy Over-optimization: a model can be excessively optimized to perform well on a proxy metric that it can forget the actual business objective. This can distract the user from his goal.

Hypothetical example: in social media, the # of likes could be an offline metric and some content (that influences a consumer to buy, for example) of a company could be a business metric. Some algorithms can accidentaly promote irrelevant content that users like a lot (e.g. funny videos) instead of the relevant company's content.

4. What is git? Describe the most often used git commands?

According to git's website, it is a version control system that records changes to a file or set of files over time so that you can recall specific versions later. This is a useful technique for people to collaborate on various projects and trace all the changes that each person made.

Most often used commands: checkout (switches between branches or commits), clone (creates a copy of a remote repository on your device), commit (records the changes which were made using the git add), add (adds the made changes that to the project for the next commit), pull (gets changes from another repository and puts them into your local branch), push (sends the commits that you made to sombeody else, a.k.a remote repository) 

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

The dot product of these two vectors is the sum over products of the elements (in the x and y vectors) at the same position. 

$$\mathbf{x}^\top \mathbf{y} = \sum_{i=1}^{d} x_iy_i$$

6. Explain what a vector norm is? 

It is the magnitude of the vector (basically, the norm of a vector tells us how big it is). 

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

Automatic differentiation is used to compute the derivatives of complex functions, so the chain rule is essential here since it is used to calculate the derivative of a composite function.

Automatic differentiation is important because it makes derivative calculations easier and more efficient (and calculating derivatives is crucial for the optimization algortihms when training deep networks). You do not have to make calculations by hand anymore.

8. Write the equation for a standard linear model in vector notation?

$\mathbf{y} = \mathbf{X} \mathbf{w}^\top\ + b$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

$p(x) = \frac{1}{\sigma \sqrt{2\pi}} \cdot e^{-\frac{1}{2}\left(\frac{x - \mu}{\sigma}\right)^2}$

Examples: birthweight of newborn babies, height of adults, shoe sizes, scores of standardized tests like SAT, blood pressure, etc.

10. Describe what a negative log likelihood is?

It is basically a cost function that operates as a loss function in ML, so that's why we multiply the log likelihood function by -1. The log is used here to simplify the numbers, so it would be easier for the computer to represent them. The likelihood tells us how well do the model's predictions match the observed data. Overall, NLL can tell us how bad (or well) the model performs.

11. Write down the formula for cross-entropy loss and explain how it is used?

$$L(\mathbf{y}, \mathbf{t}) = -\sum_{i=1}^{C} \mathbf{t}_i \cdot \log(\mathbf{y}_i)$$

Cross-entropy is used in classification tasks to measure the accuracy of a model's performance by defining the difference between the estimated probability and an actual label. It serves as the objective function that the optimization algorithm tries to minimize. y represents the vector of predicted probabilities and t represents the vector of actual labels. 

