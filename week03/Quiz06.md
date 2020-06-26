# Logistic Regression
## Question 1

Suppose that you have trained a logistic regression classifier, and it outputs on a new example $x$ a prediction $h_θ(x) = 0.4$. This means (check all that apply):

- [ ] Our estimate for $P(y=0|x;\theta)$ is 0.4.
- [ ] Our estimate for $P(y=1|x;\theta)$ is 0.6.
- [x] **Our estimate for $P(y=1|x;\theta)$ is 0.4.**
- [x] **Our estimate for $P(y=0|x;\theta)$ is 0.6.**

---

## Question 2

Suppose you have the following training set, and fit a logistic regression classifier $h_\theta(x) = g(\theta_0 + \theta_1x_1 + \theta_2 x_2)$.

| $x_1$ | $x_2$ | $y$  |
| :---: | :---: | :--: |
|   1   |  0.5  |  0   |
|   1   |  1.5  |  0   |
|   2   |   1   |  1   |
|   3   |   1   |  0   |

<img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image1.png" alt="image1" style="zoom:70%;" />

Which of the following are true? Check all that apply.

- [x] **Adding polynomial features (e.g., instead using $h_\theta(x)=g(\theta_0+\theta_1x_1+\theta_2x_2+\theta_3x^2_1+\theta_4x_1x_2+\theta_5x^2_2)$) could increase how well we can fit the training data.**
- [ ] If we train gradient descent for enough iterations, for some examples $x^{(i)}$ in the training set it is possible to obtain $h_\theta(X^{(i)}>1)$.
- [x] **At the optimal value of $\theta$ (e.g., found by fminunc), we will have $J(\theta)\ge 0$.**
- [ ] Adding polynomial features (e.g., instead using $h_\theta(x)=g(\theta_0+\theta_1x_1+\theta_2x_2+\theta_3x^2_1+\theta_4x_1x_2+\theta_5x^2_2)$) would increase $J(\theta)$ because we are now summing over more terms.

---

## Question 3

For logistic regression, the gradient is given by $\frac{\partial}{\partial \theta_j} J(\theta) =\frac{1}{m}\sum_{i=1}^m{ (h_\theta(x^{(i)}) - y^{(i)}) x_j^{(i)}}$. Which of these is a correct gradient descent update for logistic regression with a learning rate of $\alpha$? Check all that apply. 

- [ ] $\theta :=\theta-\alpha \frac{1}{m}\sum^m_{i=1}(\theta^Tx-y^{(i)})x^{(i)}$.
- [ ] $\theta_j :=\theta_j-\alpha \frac{1}{m}\sum^m_{i=1}(h_\theta(x^{(i)})-y^{(i)})x^{(i)}$ (simultaneously update for all $j$.
- [x] **$\theta_j :=\theta_j-\alpha \frac{1}{m}\sum^m_{i=1}(h_\theta(x^{(i)})-y^{(i)})x^{(i)}_j$ (simultaneously update for all $j$).**
- [x] **$\theta_j :=\theta_j-\alpha \frac{1}{m}\sum^m_{i=1}(\frac{1}{1+e^{-\theta^Tz^{(i)}}}-y^{(i)})x^{(i)}_j$ (simultaneously update for all $j$).**

---

## Question 4

Which of the following statements are true? Check all that apply.

- [x] **The sigmoid function $g(z)=\frac{1}{1+e^{-z}}$ is never greater than one ($> 1$).**
- [ ] Linear regression always works well for classification if you classify by using a threshold on the prediction made by linear regression.
- [ ] For logistic regression, sometimes gradient descent will converge to a local minimum (and fail to find the global minimum). This is the reason we prefer more advanced optimization algorithms such as fminunc (conjugate gradent/BFGS/L-BFGS/etc).
- [x] **The cost function $J(\theta)$ for logistic regression trained with $m \ge 1$ examples is always greater than or equal to zero.**

---

## Question 5

Suppose you train a logistic classifier $h_\theta(x) = g(\theta_0 + \theta_1x_1 + \theta_2 x_2)$. Suppose $\theta_0 = -6$, $\theta_1 = 0$, $\theta_2 = 1$. Which of the following figures represents the decision boundary found by your classifier?

- [ ] ![Screen Shot 2020-06-26 at 4.07.39 PM](/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/Screen Shot 2020-06-26 at 4.07.39 PM.png)
- [ ] ![Screen Shot 2020-06-26 at 4.07.57 PM](/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/Screen Shot 2020-06-26 at 4.07.57 PM.png)
- [ ] ![Screen Shot 2020-06-26 at 4.08.02 PM](/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/Screen Shot 2020-06-26 at 4.08.02 PM.png)
- [x] ![Screen Shot 2020-06-26 at 4.08.04 PM](/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/Screen Shot 2020-06-26 at 4.08.04 PM.png)

