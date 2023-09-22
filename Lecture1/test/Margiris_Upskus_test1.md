Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

-It is a situation when a model faces new/ unseen data and encounters difficulties to provide output or to give accurate predictions (lacks prior knowledge about the new inputs; there is no feedback from the past). Example: in the book there was a term about cold- start recommendation (recommending for new users and reccomending new items to existing users with little or no historical data). Another example was with booking.com. Most people onl travel onece or twice every year. By the time they come back to the booking.com site, their preferences might have changed significantly.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

-Need to understand the goal, what you want to improve: customer retention, increasing sales... Establish a benchmark wich would indicate comaprison between past and future performances. Collect the data. Compare the past results with the results that you got eith the new model. Calculate the difference in KPIs and assess whether the ML systems has led to improvements. Calculate new costs asociayed with the development and maintenance of the new model (ROI calculation at the end). 
3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 
-Real- world business scenarios are way more complex than offline metrics. Offline metrics are based on the past data and do not take into account new data and real- world is always changing. 
-Over- optimization. Offline model can achieve high accuracy during offline testing (using past data), but this may not translate to improved revenue (mode does not adapt and take inti account new/ unseen data).
-Innacuracy in objectives. 
-Delayed impact. Hard to establish a direct cause- and- effect relationship (improving recommendation accuracy may not immediatly boost revenue, it might rake months for customers to change their shopping habits).
-Example: offline metrics could be including accuracy of product recommendation while business metrics could include revenue and customer retention rate. 

4. What is git? Describe the most often used git commands?
-A system used in software development, coding. The most popular commands: git init (creates new Git repository in the current directory); git clone (creates a local copy); git add (stages changes for commit); git status (shows the status of your working directory); git branch (lists all local branches in your repository and shows in which branch you currently are); git checkout (switches to a different branch); git push (uploads your local commits to a remote repository); git rm (removes a file from both your working directory and the Git repository).
5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?
-Dot product expresses a weighter average. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, their dot product $\mathbf{x}^{T}$\mathbf{y}$, (also known as inner product) is a sum over the products of the elements.

6. Explain what a vector norm is?
-The norm of a vector tells us how big it is. 

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?
-Chain rule tells us how to find the derivative of a composite function. Automatic differentiation is important because is is a powerful tool to automate the calculation of derivatives and is preferable when differentiating complex algorithms and mathematical functions. AD can be helpful by quickly computing gradients in relation to hyperparameters, allowing for automatic hyperparameter tweaking.
8. Write the equation for a standard linear model in vector notation?
-y = Xβ + ε

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 
-f(x | μ, σ²) = (1 / (σ√(2π))) * exp(-((x - μ)² / (2σ²)))
Examples: test scores, income, human body temperature, sales.
10. Describe what a negative log likelihood is?
-A concept used in statistics, ML to quantify how well a statistical model or probability distribution fits observed data. Finding model parameters that reduce this cost, or in other words, finding the parameters that maximize the probability of the observed data, is the objective when the log-likelihood is negated.
11. Write down the formula for cross-entropy loss and explain how it is used?
-H(y, p) = -Σ [yᵢ * log(pᵢ) + (1 - yᵢ) * log(1 - pᵢ)]. It is used in classification problems. It quantifies the dissimilarity between predicted probabilities and true labels and is used for model training and evaluation. 