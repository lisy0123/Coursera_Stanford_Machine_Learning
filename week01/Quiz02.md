# Linear Regression with One Variable

## Question 1

Consider the problem of predicting how well a student does in her second year of college/university, given how well she did in her first year.

Specifically, let x be equal to the number of "A" grades (including A-. A and A+ grades) that a student receives in their first year of college (freshmen year). We would like to predict the value of y, which we define as the number of "A" grades they get in their second year (sophomore year).

Here each row is one training example. Recall that in linear regression, our hypothesis is 
![equation](https://microsoft.codecogs.com/svg.latex?h_\theta(x)%20=%20\theta_0%20+%20\theta_1x), and we use *m* to denote the number of training examples.

| x    | y    |
| ---- | ---- |
| 3    | 4    |
| 2    | 1    |
| 4    | 3    |
| 0    | 1    |

For the training set given above (note that this training set may also be referenced in other questions in this quiz), what is the value of *m*? In the box below, please enter your answer (which should be a number between 0 and 10).

> 4

---

## Question 2

For this question, assume that we are

using the training set from Q1. Recall our definition of the

cost function was ![equation](https://microsoft.codecogs.com/svg.latex?J(\theta_0,%20\theta_1)%20=%20\frac{1}{2m}\sum_{i=1}^m{(h_\theta(x^{(i)})%20-%20y^{(i)})^2})

What is ![equation](https://microsoft.codecogs.com/svg.latex?J(0,%201))? In the box below,

please enter your answer (Simplify fractions to decimals when entering answer, and '.' as the decimal delimiter e.g., 1.5).

> 0.5

---

## Question 3

Suppose we set ![equation](https://microsoft.codecogs.com/svg.latex?\theta_0%20=%20-1,%20\theta_1%20=%202) in the linear regression hypothesis from Q1. What is ![equation](https://microsoft.codecogs.com/svg.latex?h_\theta(6))?

> 11

---

## Question 4

Let ![equation](https://microsoft.codecogs.com/svg.latex?f) be some function so that 

![equation](https://microsoft.codecogs.com/svg.latex?f(\theta_0,%20\theta_1)) outputs a number. For this problem,

![equation](https://microsoft.codecogs.com/svg.latex?f) is some arbitrary/unknown smooth function (not necessarily the

cost function of linear regression, so ![equation](https://microsoft.codecogs.com/svg.latex?f) may have local optima).

Suppose we use gradient descent to try to minimize ![equation](https://microsoft.codecogs.com/svg.latex?f(\theta_0,%20\theta_1))

as a function of ![equation](https://microsoft.codecogs.com/svg.latex?\theta_0) and ![equation](https://microsoft.codecogs.com/svg.latex?\theta_1). Which of the

following statements are true? (Check all that apply.)

- [ ] If ![equation](https://microsoft.codecogs.com/svg.latex?\theta_0) and ![equation](https://microsoft.codecogs.com/svg.latex?\theta_1) are initialized so that ![equation](https://microsoft.codecogs.com/svg.latex?\theta_0%20=%20\theta_1), then by symmetry (because we do simultaneous updates to the two parameters), after one iteration of gradient descent, we will still have ![equation](https://microsoft.codecogs.com/svg.latex?\theta_0%20=%20\theta_1).
  
- [x] ***If the learning rate is too small, then gradient descent may take a very long time to converge.***

- [x] ***If ![equation](https://microsoft.codecogs.com/svg.latex?\theta_0) and ![equation](https://microsoft.codecogs.com/svg.latex?\theta_1) are initialized at a local minimum, then one iteration will not change their values.***

- [ ] Even if the learning rate α is very large, every iteration of gradient descent will decrease the value of ![equation](https://microsoft.codecogs.com/svg.latex?f(\theta_0,%20\theta_1))

---

## Question 5

Suppose that for some linear regression problem (say, predicting housing prices as in the lecture), we have some training set, and for our training set we managed to find some ![equation](https://microsoft.codecogs.com/svg.latex?\theta_0,%20\theta_1) such that ![equation](https://microsoft.codecogs.com/svg.latex?f(\theta_0,%20\theta_1)%20=%200).

Which of the statements below must then be true? (Check all that apply.)

- [ ] For this to be true, we must have ![equation](https://microsoft.codecogs.com/svg.latex?\theta_0%20=%200) and ![equation](https://microsoft.codecogs.com/svg.latex?\theta_1%20=%200) so that ![equation](https://microsoft.codecogs.com/svg.latex?h_\theta(x)%20=%200).
- [ ] For this to be true, we must have ![equation](https://microsoft.codecogs.com/svg.latex?y^{(i)}%20=%200) for every value of ![equation](https://microsoft.codecogs.com/svg.latex?i%20=%201,%202,...,%20m).
- [ ] Gradient descent is likely to get stuck at a local minimum and fail to find the global minimum.
- [x] ***Our training set can be fit perfectly by a straight line, i.e., all of our training examples lie perfectly on some straight line.***

