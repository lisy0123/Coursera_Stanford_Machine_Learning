# Regularization

## Question 1

You are training a classification model with logistic regression. 

Which of the following statements are true? Check all that apply.

- [ ] Adding mant new features to the model helps prevent overfitting on the training set.
- [ ] Introducing regularization to the model always results in equal or better performance on the training set.
- [ ] Introducing regularization to the model always results in equal or better performance on examples not in the training set.
- [x] **Adding a new feature to the model always results in equal or better performance on the training set.** 

---

## Question 2

Suppose you ran logistic regression twice, once with $\lambda=0$, and once with $\lambda=1$. 

One of the times, you got parameters $\theta=\begin{bmatrix}81.47\\12.69\end{bmatrix}$, and the other time you got $\theta=\begin{bmatrix}13.01\\0.91\end{bmatrix}$. 

However, you forgot which value of $\lambda$ corresponds to which value of $\theta$.

Which one do you think corresponds to $\lambda=1$?

- [x] $\theta=\begin{bmatrix}13.01\\0.91\end{bmatrix}$
- [ ] $\theta=\begin{bmatrix}81.47\\12.69\end{bmatrix}$

---

## Question 3

Which of the following statements about regularization are true? Check all that apply.

- [ ] Because logistic regression outputs values $0 \le h_\theta(x) \le 1$, it's range of output values can only be "shrunk" slightly by regularization anyway, so regularization is generally not helpful for it.
- [x] **Using too large a value of $\lambda$ can cause your hypothesis to underfit the data.**
- [ ] Because regularization causes $J(\theta)$ to no longer be convex, gradient descent may not always converge to the global minimum (when $\lambda > 0$, and when using an appropriate learning rate $\alpha$).
- [ ] Using a very large value of $\lambda$ cannot hurt the performance of your hypothesis; the only reason we do not set $\lambda$ to be too large is to avoid numerical problems.

---

## Question 4

In which one of the following figures do you think the hypothesis has overfit the training set?

- [x] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image6.png" alt="image6" style="zoom:60%;" />

- [ ] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image7.png" alt="image7" style="zoom:60%;" />

- [ ] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image8.png" alt="image8" style="zoom:60%;" />

- [ ] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image9.png" alt="image9" style="zoom:60%;" />

---

## Question 5

In which one of the following figures do you think the hypothesis has underfit the training set?

- [x] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image10.png" alt="image10" style="zoom:60%;" />

- [ ] <img src="file:///Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image11.png?lastModify=1593168838" alt="image11" style="zoom:60%;" />
- [ ] <img src="file:///Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image12.png?lastModify=1593168838" alt="image12" style="zoom:60%;" />

- [ ] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week03/image13.png" alt="image13" style="zoom:60%;" />