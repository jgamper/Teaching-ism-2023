Please copy the file and rename it as FirstName_LastName_Test.md. Raise a pull request with this file (with answers) added to the repository. 

1. What does cold start problem mean in Machine Learning in practice? How does it examplify in book?

A problem thats poor at predicting models due to lack of data
Booking.com example: most people travel only once or twice per year, so everytime they comeback their preferences might have changed significantly. A problem occurs that accomodations which they liked last year might not be relevant for them this year, which can impact the conversion and overall customers experience with the app.

2. What is the most reliable way to demonstrate a return on investment of a machine learning system?

The first thing to measure ROI of machine learning system we have to understand the main goal -> what metric we want to improve, is it CR% or maybe AOV or maybe customer complaints? 

Before implementing your ML model, we have to gather valid data. Lets take TikTok as an example, we want to increase mens 45+ age screen time and make them stay on the app as long as possible

Problem --> 45+ aged men are not using tiktok, but they are really great customers as 45+ men most probably have more money than younger generation so they could spend a bag on buying thing from ads, the ads will perform better --> businesses will increase the spend on ads --> TikTok will end up with gathering more revenue

To run ML model, gather solid data of Men 45+ age screen time on tiktok, their AOV and their CR% 

Lets imagine we created some sort of ML model which made 45+ Men stay longer on the app (improved algorithm or smth). To evaluate the data we are going to compare new CR% and AOV metrics, because maybe Men are staying longer on the app but their CR% and AOV was not affected and we ended up wasting money on new algorithm 

To calculate ROI --> You calculate costs of new algorithm, time of how much did you spend on it and outcomes --> did we ended up with getting more revenue and 45+ aged men customers or not?

3. What are the 4 reasons for lack of correlation between offline performance gain and business value gain? Make up a hypothetical example - name concrete offline metrics, and business metrics. 

4 reasons:
Value performance saturation - improvements in model does not provide any value for business

Segment Saturation - as models improve on each other,
this disagreement rate goes down, reducing the population of users that are actually exposed to a treatment, and with that, the power to detect gains in value

Uncanny Valley Effect - as models become better and better,
they seem to know more and more about our users, or can
predict very well what the user is about to do. This can be
unsettling for some of our customers

Proxy Over optimization - models might start focusing too much on the metric we want to improve. For example, CTR, it will increase the CTR with some clickbaiting stuff, but it won't improve our conversion rate.

Hypothetical Example

Lets try to consider netflix business model

Offline metrics
- Precision: proportion of recommended movies in the top 10 that are relevant
- Recall: proportion of relevant movies that are recommended in the top10

Business metrics
- Retention, subscriptions

Lets say we increased precision from 60% to 90% and recall from 50 to 75%

The recommendations might have better accuracy but not diverse enough, so users will get bored and eventually subscription won't get bigger

Customers might be sharing netflix accounts, maybe one is looking for 1 genre and another is looking for different one so quality of data might be poor



4. What is git? Describe the most often used git commands?

Git is a distributed version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers who are collaboratively developing source code during software development. Its goals include speed, data integrity, and support for distributed, non-linear workflows. 

git checkout
git add
git clone
git commit
git checkout

5. Given two vectors $\mathbf{x}$, $\mathbf{y}$ $\in \mathcal{R}^{d}$, describe in words and equations what their dot product means?

The dot product of two vectors teels us how much they point in the same direction - the bigger the score, the bigger probability theat they are pointing into the same direction and if the score is 0, that means that they are pointint to completely different directions


6. Explain what a vector norm is?

Vector norm tells us hiw big it is (the lenght of a vector). There L1 and L2 norms which measure vector norm. L2 - euclidean norm, measures distance between two points in space, the L1 - measures distance if you are moving along gridlines

In deep learning, we are often trying to solve optimization problems: maximize the probability assigned to observed data; maximize the revenue associated with a recommender model; minimize the distance between predictions and the ground truth observations; minimize the distance between representations of photos of the same person while maximizing the distance between representations of photos of different people. These distances, which constitute the objectives of deep learning algorithms, are often expressed as norms. (Definition from the book)

7. What role does chain rule play in automatic differentiation? Why automatic differentiation is important for modern AI
models?

THe chain rule making it possible to compute gradient efficiently for complex functions, like calculating derivatives and more.

Autograd lets us design massive models for which pen and paper gradient computations would be prohibitively time consuming, it can train complex ML systems --> Basically automates the job for people to not waste time on complex math, does everything by himself

8. Write the equation for a standard linear model in vector notation?

$
\mathbf{y} = \mathbf{X} \mathbf{w} + b
$$

9. Write a formula for the normal distribution? Give examples of what may be normally distributed data? 

$$
f(x | mu, sigma) = (1 / sqrt(2 * pi * sigma^2)) * exp(-0.5 * (x - mu)^2 / sigma^2)
$$

Example: People IQ scores is a good example of nornal distribution, we have a strong mean where majority of people are and then there people with lower and higher IQ scores than the mean

10. Describe what a negative log likelihood is?

We usually look at this metric when we are training and evaluating our model to get better understanding how well our model is doing. Negative log likelihood represents the probability of observing given data. The lower likelihooh indicates better data fit and better model predictions


11. Write down the formula for cross-entropy loss and explain how it is used?

L(y,p)=−ylog(p)−(1−y)log(1−p)

Usually we use cross-entropy during model training phase, the main goal is to minimize this loss, which leads to better classification performance. In terms - Cross-entropy loss measures dissimilarity between true label distribution nad predicted probabilities

