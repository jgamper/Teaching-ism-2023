Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

    Cold start problem in machine learning in practice means that the website do not have a very good picture of the custumer because he visits it just once or twice a year and preferences from the last visit could be changed (in booking example: maybe there is more children or budget changed) so the history of user can have 0 value now and the code would not work as best as it can because new products (hotels) are added and code just offer all possible variant that would not neccessary fit the customer but the code did not know that because of cold start problem.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

    When the parameters "boost" in a better way: more bookings, better location detection, better ranking, happier clients (airbnb hose owners get better booking based on they pattern: no less than 3 days, no gaps between bookings, etc). This return do not reach the least client but it shows at the revenue, at the bookings, responses.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

    1. Value Performance Saturation
    2. Segment Saturation
    3. Uncanny Valley effect
    4. Proxy Over-optimization

4. What is git? Describe the most often used git commands?

    Git means global transformation tracker so it is a system used for tracking changes in computer files, source code, for source code management and software development.
    1. Git init - to create a new Git repository
    2. Git clone - creates  copy of a remote Git repository on local mashine and allows to start working
    3. Git add - adds changes to the staging area
    4. Git commit - saves the modification in local repository with git commit
    5. Git status - key to Git's mind. Shows the status of working directory. Indictes which files are modified, staged or untracked
    6. Git log - shows a history of commit messages, authors, dates and commit hashes
    7. Git pull - bring changes from remote repository and merges with current branch
    8. Git push - sends all commits and changes to a remote repository
    9. Git branch - shows the list of all branches in repository
    10. Git checkout - allows to work on different parts of the code by switching between branches or commits
    11. Git merge - merge the changes from one branch into another
    12. Git remote - lists a remote repositories where your local repository is connected to
    13. Git fetch - detect changes from a remote repository but do not merge them to my current branch

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

    $$\mathbf{x}^\top\mathbf{y} = \sum_{i=1}^{d} x_iy_i$$
    Dot product tells how much x and y vectors share a common direction in d-dimencional space

6. Explain what a vector norm is?

    The norm of a vector tells us how big it is. There is two norms that is decribed in book: l1 and l2. l1 norm measures the lenght of a vector, sums teh absolute values of a vector's elements and l2 is the sqaure root of the sum of squares of a vector's elements, l1 is less sensitive to outliers than l2

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

    Chain rule takes care of the gradient of the concern which is often difficult to calculate. Gradients is necceassary to know how to move the parameters of the model fot the best output. Automatic differentiaion, driven by the chain rule is for efficiency of computing gradients. So, chain rule is essential in automatic differentiation because it allows to differenciate composite functions, which are mostly in modern AI models.

8. Write the equation for a standard linear model in vector notation?

    $$\hat{y} = \mathbf{W}^\top\mathbf{x} + b$$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

    $$f(x | \mu, \sigma^2) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x - \mu)^2}{2\sigma^2}}\$$
    Normaly distributed data is characterized by bell shaped curve. So, this kind of curve can have the data of adult humans height, test scores, income levels, body temperature, etc.

10. Describe what a negative log likelihood is?

    While optimizing the function, usually it is easier to express optimization as minimization rather than maximization, so, to achieve this you need to negate the logarithm of likelihood function because maximum likelihood estimation is used to estimates parameters for models to maximize likelihood function (parameters of linear model that fit the data best)

11. Write down the formula for cross-entropy loss and explain how it is used?

$$l(y, \hat{y})= - \sum_{j=1}^{q} y_j \log(\hat{y}_j)$$
It is used for classification model performance measurement during training proces when new weights of the model is adjusting, for minimizing the loss. Cross-entropy measures the difference between actual and  predicted probability distribution and the purpose is to reduce it.
