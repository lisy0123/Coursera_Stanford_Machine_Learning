# Advice for Applying Machine Learning

## Question 1

You train a learning algorithm, and find that it has unacceptably high error on the test set. You plot the learning curve, and obtain the figure below. Is the algorithm suffering from high bias, high variance, or neither?

<img src="http://spark-public.s3.amazonaws.com/ml/images/10.1-a.png" alt="img" style="zoom:70%;" />

- [ ]  Neither
- [x] **High blas**
- [ ] High variance

---

## Question 2

Suppose you have implemented regularized logistic regressionto classify what object is in an image (i.e., to do object recognition). However, when you test your hypothesis on a new set of images, you find that it makes unacceptably large errors with its predictions on the new images. However, your hypothesis performs **well** (has low error) on the training set. 

Which of the following are promising steps to take? Check all that apply.

- [ ] Try evaluating the hypothesis on across validation set rather than the test set.
- [ ] Try decreasing the regularization parameter $\lambda$.
- [x] **Try using a smaller set of features.**
- [x] **Try increasing the regularization parameter $\lambda$.**

---

## Question 3

Suppose you have implemented regularized logistic regression to predict what items customers will purchase on a web shopping site. However, when you test your hypothesis on a new set of customers, you find that it makes unacceptably large errors in its predictions. Furthermore, the hypothesis performs **poorly** on the training set. 

Which of the following might be promising steps to take? Check all that apply.

- [x] **Try adding polynomial features.**
- [ ] Use fewer training examples.
- [ ] Try evaluating the hypothesis on a cross validation set rather than the test set.
- [x] **Try decreasing the regularization parameter $\lambda$.**

---

## Question 4

Which of the following statements are true? Check all that apply.

- [ ] Suppose you are training a regularized linear regression model. The recommended way to choose what value of regularization parameter $\lambda$ to use to choose the value of $\lambda$ which gives the lowest **training set** error.
- [x] **The performance of a learning algorithm on the training set will typically be better than its performance on the test set.**
- [ ] Suppose you are training a regularized linear regression model. The recommended way to choose what value of regularization parameter $\lambda$ to use is to choose the value of $\lambda$ which gives the lowest **test set** error.
- [x] **Suppose you are training a regularized linear regression model. The recommended way to choose what value of regularization parameter $\lambda$ to use is choose the value of $\lambda$ which gives the lowest cross validation error.**

---

## Question 5

Which of the following statements ar true? Check all that apply.

- [ ] If a neural network has much lower training error than test error, then adding more layers will help bring the test error down because we can fit the test set better.
- [x] **If a learning algorithm is suffering from high blas, only adding more training examples may nor improve the test error significantly.**
- [x] **When debugging learning algorithms, it is useful to plot a learning curve to understand if there is a high blas or high variance problem.**
- [x] **A model with more parameters is more prone to overfitting and typically has higher variance.**