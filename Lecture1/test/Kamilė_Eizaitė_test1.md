Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

In simple terms the cold start problem in Machine Learning is a situation when a system or a model faces the information that has never seen before or lacks historical sources in order to accurately make decisions or predictions. In machine Learning practice cold start problem could be faced in Financial Forecasting, Healthcare, Fraud detection area and etc. 

Textbook provides us an example of recommender systems, where this problem is very often met. Since the main goal of these systems are to display a set of items relevant to the user. Meaning that the product ratings and reviews on Amazon, IMDb, or Goodreads are very important - the more active the customers are on their account by giving feedback and rating the goods, the more information system has. With this data service provider later can recommend film or good more accurately. This helps to eliminate the cold start problem. However, it is still difficult to make predictions or recommendations for total new users, who has no previous history.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

As the real-life example of Airbnb success confirms - ROI is invisible without A/B experiments.

It's essential to use A/B experiments because sometimes the changes made by machine learning models aren't easy to see with the naked eye. There might be no obvious differences in the user interface (UI), but these small, hidden changes can still have a big impact when you look at overall results. Running the new model in production with an experiment helps us discover these effects. It's like testing a new recipe to see if it tastes better, even if it looks the same on the plate.

Example when Airbnb ranking team ran A|B experiments. They had proof that location context, a host scoring, a host preference models were driving larger booking increases than nearly every other product initiative. When time came to make further investments, the search ranking team’s scope increased and the effect on metrics was very clear from the A|B experiments.

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

Based on the provided article about the Booking.com these are the reasons:
- Value Performance Saturation: After a certain point, making the model better doesn't make a noticeable difference in real-world results.
- Segment Saturation: happens when you're comparing a new model to an old one. You want to focus on users where the models disagree to see if the new model is better. But as models get better, they disagree less, so you have fewer users to test, which makes it harder to tell if the new model is really an improvement.
- Uncanny Valley effect: when AI models become really good at understanding users, almost like mind-readers. This can make some users uncomfortable, leading to a negative impact on their experience and the value they get from the service
- Proxy Over-optimization: A recommendation system might encourage users to click on similar products, but this can overwhelm users with choices and hurt actual sales.
 
Example: The food delivery service strives to fulfil orders as quickly as possible, however this causes couriers to rush deliveries and make mistakes, which causes orders to arrive cold and with mistakes.  While the times for delivery are impressive, customer satisfaction is harmed, which discourages repeat purchases and lowers overall business value.

4. What is git? Describe the most often used git commands?

Git is a widely used distributed version control system (DVCS) which allows multiple users to collaborate on a project and track changes of the code.

These are most used commands: 

- git init:
It sets up a place for your project's files and keeps track of changes you make to them.

- git clone [repository URL]:
Creates a copy of a remote project on your own computer, allowing you to work on the project locally.

- git add [file(s)]:
Stages changes for commit. It prepares specified files (or all changes if not specified) for the next commit.

- git commit -m "Your commit message":
Records staged changes in the version history along with a descriptive commit message that explains the changes made.

- git status:
Shows the current status of your work such as untracked files, directory, branch information and new changes.

- git log:
Displays a chronological list of all commits in the current branch, showing commit messages, authors, dates, and commit IDs.

- git branch:
This command lists all branches and mark the current branch that you are in with an asterisk.

- git checkout [branch name]:
Switches to another branch and allows to work on a particular branch's code.

- git merge [branch name]:
This helps to combine changes from different branches into the current/main branch. 

- git pull:
Fetches changes from the remote branch and update local branch with the latest changes that was made remotely.

- git push:
This command pushes/sends your local actions and all the changes to the remote work environment.

- git remote:
This shows were the local current project is stored in the remote environment.

- git fetch:
It recieves new changes from the remote place automatically but do not apply any updates without permission to the local work enironment.

- git diff:
This command helps to see the difference between the current work and the one before recent changes. 

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

The dot product of two vectors is a mathematical operation that measures how much these vectors "align" with each other. In other words, it quantifies the relationship between the two vectors.

$$\mathbf{x}^\top\mathbf{y} = \sum_{i=1}^{d} x_iy_i$$

6. Explain what a vector norm is?

A norm is a function ||.|| that maps a vector to a scalar. In simpler terms, it quantifies how "big" or "long" a vector is. It actually satisfies the following three properties:

- Scalar Multiplication:
It states that the norm of a scaled vector is equal to the absolute value of the scalar multiplied by the norm of the original vector.
||αx|| = |α| * ||x||

- Non-negativity(Positivity):
the norm of any vector is greater than or equal to zero.
||x|| ≥ 0 

- Triangle inequality:
It describes the relationship between the norms of vectors and their sum (or difference). This property reflects the idea that the shortest path between two points is a straight line, which is a fundamental concept in geometry.
||x + y|| ≤ ||x|| + ||y||

In the textbook there are mentioned 3 different norms which encode different notions of size: Euclidean, Manhattan distance, The Frobenius norm.

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

A chain rule is very important part in AD since this technique helps to efficiently compute derivatives. It breaks down the complex function into more understandable parts.

Automatic differentiation itself is very valuable in AI models since 1. Is efficiently determine gradients and is important for big models 2. Supports deep learning allowing deep neural networks 3.  This is used in Sensitivity analysis and AI efficient optimization 4. It also makes hyperparameter tunning possible. 

8. Write the equation for a standard linear model in vector notation?

$$\hat{y} = \mathbf{W}^\top\mathbf{x} + b$$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

$$f(x | \mu, \sigma^2) = \frac{1}{\sigma \sqrt{2\pi}} \cdot e^{-\frac{(x - \mu)^2}{2\sigma^2}}$$

Examples of normally distributed data:
- IQ scores: it is accepted that IQ follows a normal distribution which has a mean of 100 and a standard deviation of 15
- Height of Adults: it often follows normal distribution ad it has a mean height which varies around a certain value like the population average height and also there is standard deviation that quantifies the variation in heights.
- Residuals in regression: the residuals (differences among observable and projected values) are frequently assumed to be regularly distributed in linear regression analysis. For statistical inference to be accurate this assumption has to be true.

10. Describe what a negative log likelihood is?

A crucial tool in statistics and machine learning is the negative log likelihood. It evaluates how effectively a model's parameters account for the data that has been seen. An improved fit between the model and the data is shown by a lower negative log-likelihood. Because minimising the negative log likelihood is the same as maximising the likelihood, this metric is frequently applied in optimisation tasks. By minimizing the negative log-likelihood, we're essentially trying to make our model as good as possible at matching reality.

11. Write down the formula for cross-entropy loss and explain how it is used?

$$l(y, \hat{y}) = - \sum_{j=1}^{q} y_j \log(\hat{y}_j)$$
The cross-entropy loss is used in machine learning to measure how good our predictions are when we're trying to classify things into different categories, like sorting emails into "spam" or "not spam." So, lower loss means better predictions.

