Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?
It means, that some product can be not good yet, because there is not enough information and there are no enough tests done, to say if the product, system can be reliable and sucessful. In the book they mention the problem with the accomodation: people cannot keep up with the new conditions, also as they travel not often they can have different preferences every year, as they for example grow up, create family or grow old, so it is hard to create the best model for every user to satisfy them. 

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?
A/B testing.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 
    1. The offline metrics are made for the theoretical performance and not all people in the economy are homo economus. 
    2. It can be overfitting - it will work well in theoretical matter, but fail to adapt if there are some unseen factors. 
    3. Also, the training data can miss some of the segments and not including them means that for this area the model will not perform good.
    4. Users can adapt to the new decision and then their behaviour would change - that means the model will not fully measure the performance.
Hypothetical example - in the medical care system, when we have a model, which can detect the disease this situation may occur. The model can be too conservative and lead to many missed diagnosis in order to, as much as possible, avoid the false diagnosis, when the patient gets a positive result, when there is no disease. Then the accuracy of the model is really high, but it is not good in the business matter as the patients get false positive results and then get additional stress, more tests need to be done and it overall damages the image of the medical institution. 

4. What is git? Describe the most often used git commands?
It is a powerful, fast and free version control system, which allows to do small and bigger projects and also allows programmers to collaborate and allow them to make changes without interfering in each other's work. 
Git commands:
    1. git clone - creates a copy of a Git repository.
    2. git status - shows the status of work directory.
    3. git commit - record changes.
    4. git branch - lists all branches in repository.
    5. git push - pushes your commits to a remote repository, to keep the changes.

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

6. Explain what a vector norm is?
It is kind of measure to know how big or small the vectors is and there are different norms of vectors. In the reading there were mentioned mostly two - Manhattan Norm and Euclidean distance norm. The Manhattan norm measures vector in the space of grid - you can only measure it going along the lines and with Eucliden distance - it is the smallest possible distance. 

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?
Without the chain rule it would be quite difficult, because we are working with deeply nested functions and chain rule allows us to break down the computation of derivatives into the series of elementary operations. Moreover, the chain rule allows deep learning models to learn from data by adjusting their parameters and minimizing a loss function.

8. Write the equation for a standard linear model in vector notation?

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

10. Describe what a negative log likelihood is?

11. Write down the formula for cross-entropy loss and explain how it is used?
