Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository.    

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

    Cold start - when a ML model fails or finds it difficult to perform effectively and draw inferences on new, unseen data. For example while algorithm is trained to detect skin cancer and encounters a skin photo of any unseen race, it might fail to provide correct answers. 
    
    EX.: People might think differently and want different things after the last time they opened booking.com. The algorihm might not know how tot tackle the data they get.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

    A|B offline experimenting. This provides evidence that these models increases businesses metrics.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

    Value Performance Saturation,
    Segment Saturation,
    Uncanny Valley effect,
    Proxy Over-optimization

4. What is git? Describe the most often used git commands?

    Git helps us to trace code or computer file versions, manage them, track changes.

    git clone - helps in joining the repository

    git checkout - lets to create a new branch or hop onto an existing one

    git add - moving files from Working Directory to the Staging Index

    git commit - saves a changes and a comment of the log

    git push - adds the files from local to remote repository

    git branch - shows on which branch of the repository a user is and lets work only in that branch

    git status - provides the state of the repository

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

    The dot product is a sum over the produts of the elements at the same position.

6. Explain what a vector norm is?

    It is the lenght of the vector.

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

    Chain rule helps in calculating nested function by returning to functions of a single variable. This helps in calculating gradients. Automatic differentiation is important because it lets us to write shorter codes that might be easier to debug and train.

8. Write the equation for a standard linear model in vector notation?

    Y_{i} = x_i^T\beta+\epsilon_{i}

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

    p_{x} = \frac{1}{\sqrt{2\pi\sigma^{2}}}exp(-\frac{1}{2\sigma^{2}}(x-\mu)^32

    Points scored in basketball game. In Europe, basketball teams usually score 70-80 points per game, so the mean and the median might be in that interval. Some outliers also might occur.

10. Describe what a negative log likelihood is?

    This function serves the purpose of estimating parameters for a logistic regression model. It also offers a measure of how effectively the model aligns with the training data.

11. Write down the formula for cross-entropy loss and explain how it is used?

    H = -\displaystyle\sum\limits_{i=1}^n t_{1}\log{p_{i}}

    1.  In training classification models that has values from 0 to 1, it starts with random parameters and predicts for each data point.
    2.  Calculates cross-entropy loss for the entire dataset, and compares the probabilities to the exact labels.
    3.  Getting a scalar that shows how well the the model fits data.
