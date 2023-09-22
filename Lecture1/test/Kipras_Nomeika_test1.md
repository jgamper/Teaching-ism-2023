Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

    Cold start problem means that the model constantly faces difficulties when it has to deal with unseen data, new patterns. This might happen because model lacks prior training and lacks specific information to make the accurate predictions in new and unexpected situations. A very good example is people going for a holiday only a couple times a year, because of rare occasion the model treats those same people differently, just like new users, because there is no older historical data or it is not relevant.


2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

    Demonstrating return on investment in machine learning basicaly means to get the benefits gained from the model/system relative to the costs that were spent while developing, launching and maintaining it. A clear way to demonstrate ROI is to prepare analysis of all costs spent and benefits gained from using it. Some of the examples could be: development costs, maintenance costs, maintaining a timeframe after which meaningful results could be expected, capturing and evaluating proper customer feedback about the model and suggestions for improvement. Basically just collecting the costs and values gained.


3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 3

    The 4 reasons for lack of correlation between offline performance gain and business value gain:
    1.  misalignment of metrics - this situation occurs when offline performance metrics that are being optimized do not directly align with key business metrics that actually derive certain value. The example could be as follows: a retail company focuses on reducing website load times in order to improve user's experience, but business' key metric is sales revenue and it may not show great improvements when webiste laod times are optimized.
    2. external factors - this situation refers to the impact of factors that are not in your control, such as marekt conditions, economic trends, competitor's actions. The  example could be: an airline seeks to gain more profits and reduce delay times (offline metric). Despite this, the sudden spike in fuel prices occurs and the company earns even less profits, has less business value.
    3. time lag - there can be a delay between optimizing offline performance and increases in the business value. Business metrics may take time to reflect the impact of improvements in performance. The example could be: a software developing company investst some money in improving software stability to reduce customer support requests. Despite the fact that improvements lead to fewer requests, financial benefits like higher sales and higher customer retention may take several months to happen.
    4. secondary effects - offline performance improvements can have accidental consequnces that effect business parameters and they may not align with expected gains. The example of this may be: a company reduces the function's/algorithm's processing time to improve user experience. However, this mistakenly leads to higher spreads of missinformation, which further leads to a decrease in company's reputation.


4. What is git? Describe the most often used git commands?

    GIT – it is a distributed version control system that helps people to manage all changes that were made to the code and other files within a project. It was created in 2005 and since then it has become the main tool used for product development. 

    The main functions used are: git branch (lists all branches in your repository; developers can create new features or bug fixes, while allowing others to work paralely), git clone (creates a copy of a remote repositoy on your local machine; usually this is how you start working on an existing project hosted on server like GitHub or GitLab), git merge (merging allows to combine changes made from one file to another), git commit (git allows to track all changes made to the code, allows to see author of the change, timestamp and description. It allows to track the evolution of the project during the process), git status (this command shows the status of your working directory and lists all the files that had some changes made to them). 


5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

    In words:
    the dot product of two vectors measures the degree to which they align with each other. It provides a measure of similarity or correlation between the two vectors in terms of direction, with positive value representing alignmnet, negative value representing anti-alignment and zero implying that vectors are othodognal.

    In equations:
    it is defined as 𝑥 ⋅ 𝑦 = x₁ * y₁ + x₂ * y₂ + ... + xᵈ * yᵈ. In this formula Xi represents components of vector X, where i ranges from 1 to d; Yi represents components of vector Y, also ranging from 1 to d; dot product is computed by multiplying the relevant components Xi and Yi and summing them. The resulting value is a single number and it represents the extent to which vectors X and Y are pointing in the same direction/not in the same direction (the rules were described 'In words' explanation).


6. Explain what a vector norm is?

    Vector norm is a term which is used to quantify the size of a vector in vector space, basically it is nonnegative number which helps to understand how ‘long’ or ‘big’ the vector is. The most common vector norm is the Euclidean norm.


7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

    There are several roles that chain rule play in automatic differentiation:
    1. it computes derivatives - it computes derivatives like chain functions, that are formed by connecting together simpler functions. If you have a complex function that can be expressed in a form of composed simpler function, you can apply chain to calcute its derivative efficiently.
    2. propagation of gradients - the chain rule allows the multiplication of gradients through graphs. It facilitates the calculation of how changes in parameters of one layer affect the final output. 

    Automatic differentiation is important for AI models because:
    1. it gives higher accuracy - automatic differentiation provides exact derivatives, which can be crucial in situations where small errors add up over time. It is especially important in physics simulations and application where precise numbers and results are required.
    2. it reduces human error - it is likely that manual derivations might have some human erorrs, automatic differentiation eliminates this source of error and gives more reliable results.
    3. increase in scale - as modern AI models grow in complexity and size, automatic differentiation becomes extremely valuable, because they are designed to handle high dimension parameters, which makes them a good fit for modern AI tasks. 


8. Write the equation for a standard linear model in vector notation?

    The equation for a standard linear model:
    y = ax + b

    The component and their expalanation:
    ~ y - represents the output value
    ~ a - represents the rate of change 
    ~ x - represents the input value
    ~ b - represents the constant


9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

    The formula for the probability density function (PDF) of the normal distribution is as follows:
    f(x | μ, σ²) = 1 / (σ √(2π)) * e^(-(x - μ)² / (2σ²))

    In this simplified version:
    - \(x\) stands for random variable.
    - \(\mu\) is the average value of the distribution.
    - \(\sigma\) is the standard deviation, which measures the spread of the data.
    - \(\e\) is the base of the natural logarithm.
    - \(\π\) is the mathematical constant pi.

    The examples of normally distributed data could be:
    ~ Human heights
    ~ IQ scores
    ~ Reaction times
    ~ Body temperature


10. Describe what a negative log likelihood is?

    The negative log likelihood is mathematical function, which is used in statistics and machine learning to measure the goodness of fit between probability distribution and observed data (in other words, it is used to measure how well the model aligns with observed data; how well the model fits the data used to train it.).


11. Write down the formula for cross-entropy loss and explain how it is used?

    The formula for cross-entropy loss:
    L(y, ŷ) = -[y * log(ŷ) + (1 - y) * log(1 - ŷ)]

    Meaning of its elements:
    L(y, ŷ) - This represents the binary cross-entropy loss for a single data point.
    y - This is the true binary label (0 or 1) for the data point.
    ŷ - This is the predicted probability that the data point belongs to class 1. It's typically the output of a sigmoid function applied to a model's raw prediction.

    This formula is often used in machine learning and classification tasks. It measures the difference between a predicted probability distribution and the true probability distribution of the target labels. Common spheres to use it is logistic regression, neural network training.