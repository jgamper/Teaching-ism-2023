Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

Cold start refers to an issue in Machine Learning when there is not enough historical data in order to e.g., provide recommendations in recommender systems. For instance, in the case of booking.com, majority of people travel only 1-2 times a year and when they come back to the website, it might be the case that their preferences have changed substantially. Besides that, when new accommotations become added on bookin.com, they do not have enough content (e.g., photos, descriptions in several languages) or reviews, thus it is difficult to find guests for them.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

The most reliable way to demonstrate a return on invesment in A|B experimentation. Without machine learning teams running A|B experiments, return on investment cannot be recognised. 

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

1 Value performance saturation (there are business problems for which it is not possible to indefinitely drive value from model performance gains);
2 Segment saturation (disagreement rate goes down as models improve on each other, leading to a reduction in the user population which is exposed to a treatment, and the power to detect value gains);
3 Uncanny Valley effect (improving models can result in a negative effect on value due to people not always reacting positively to accurate predictions about them);
4 Proxy over-optimization (proxies that are over-optimizing can distract users away from their goal) 

Example: improving the performance of the model (which can be, e.g., evaluated by Mean Reciprocal Rank) does not necessarily lead to business value gain (e.g., improvement in such business metrics as conversion rate). For instance, an online platform with recommender system, ranking the most relevant products at the top of the recommendation list, with a goal to increase conversion rates by providing personalized recommendations to the users. The model’s performance can be improved by improving the ranking and Mean Reciprocal Rank metric, but that will not necessarily lead to business gain. It might be the case that users click on products recommended to them but not purchase them. Customers might care about other factors, not addressed by improvements in Mean Reciprocal Rank (e.g., pricing, etc.)


4. What is git? Describe the most often used git commands?

Git is an open source, free distributed version control system that tracks changes in computer files and is used for managing source code in software development projects. 
git config: allows to specify email and username that will be used with the commits;
git init: can be used to create a new Git repository;
git clone: dowloads existing source code from a remote repository;
git status: provides information about current branch;
git add: includes changes of files into the next commit;
git commit: saves changes locally;
git push: uploads commits to the remote repository;
git branch: can be used for creating, listing, and deleting branches;
git checkout: can be used to switch from one branch to another;
git pull: can be used to pull recent changes from remote server into local repository;
git merge: merges the branch with the parent branch.


5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

Dot product is a sum over the products of the elements that are at the same position. 
$$\mathbf{x}^\top\mathbf{y} = \sum_{i=1}^{d} x_iy_i$$

6. Explain what a vector norm is?

Vector norm is a size of the vector. It maps a vector to a scalar and satisfies 3 properties:
1 if all elements of the vector are scaled by a scalar, its norm scales accordingly;
2 norms satisfy the triangle inequality;
3 the norm is non-negative and vanishes if the vector is zero.


7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

Automatic differentiation works backwards through computational graph applying the chain rule to calculate derivatives. 
Automatic differentiation is important for modern AI models because in all optimization algorithms derivatives have to be calculated and it would be tedious to do this by hand, so automatic differentiation does this instead of us. 

8. Write the equation for a standard linear model in vector notation? 

$$\hat{y} = \mathbf{w}^\top\mathbf{x} + b$$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

$f(x) = \frac{1}{σ\sqrt{2\pi}} e^{-\frac{(x - μ)^2}{2σ^2}}\$

Examples of normally distributed data: weight, height, IQ scores, blood pressure

10. Describe what a negative log likelihood is?

It is a loss function used in optimization. Because optimizations are often expressed as minimization rather than maximization, it is an alternative for maximization of the logarithm of the likelihood (logarithms are used in order to simplify calculations).

11. Write down the formula for cross-entropy loss and explain how it is used?


$$l(\mathbf{y}, \mathbf{\hat{y}}) = - \sum_{j=1}^{q} y_j \log(\hat{y}_j)$$

It measures the performance of classification model and is used during training when adjusting weights of the model, aiming to mimize the loss. Cross-entropy loss measures the difference between predicted probability distribution and the actual one, so the goal is to reduce it.  