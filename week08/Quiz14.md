# Principal Component Analysis

## Question 1

Consider the following 2D dataset:

<img src="https://d3c33hcgiwev3.cloudfront.net/lkk6_L7kEeSZtCIACx4DqA_15.1-question.jpg?Expires=1593388800&Signature=EGDf-mBlj-uZ-Rnm9JXlhgZ4cbZUXOS8rrajQKZrjOpCNiwwrBBfsLesxylXsZvnpkEV2Y2rAhQvP45TVqSw5PV9fQgUZNfYoJmpLV06DMqetYkQaYr9GUQ~rwKtV50kXO7LMDByXnUl6ekHLpuwlwIEV2EPpUwfpsA1yDlG4e4_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A" alt="img" style="zoom:50%;" />

Which of the following figures correspond to possible values that PCA may return for $u^{(1)}$ (the first eigenvector / first principal component)? Check all that apply (you may have to check more than one figure).

- [x] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week08/image1.png" alt="image1" style="zoom:50%;" />

  > The maximal variance is along the y = x line, so this option is correct.

- [x] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week08/image2.png" alt="image2" style="zoom:50%;" />

  > The maximal variance is along the y = x line, so the negative vector along that line is correct for the first principal component.

- [ ] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week08/image3.png" alt="image3" style="zoom:50%;" />

- [ ] <img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week08/image4.png" alt="image4" style="zoom:50%;" />

---

## Question 2

Which of the following is a reasonable way to select the number of principal components $k$?

(Recall that $n$ is the dimensionality of the input data and $m$ is the number of input examples.)

- [ ] Choose the value of $k$ that minimizes the approximation error $\frac{1}{m} \sum_{i=1}^m ||x^{(i)} - x^{(i)}_{\rm approx}||^2$.

- [x] **Choose $k$ to be the smallest value so that at least 99% of the variance is retained.**

  > This is correct, as it maintains the structure of the data while maximally reducing its dimension.

- [ ] Choose $k$ to be the smallest value so that at least 1% of the variance is retained.

- [ ] Choose $k$ to be 99% of $n$ (i.e., $k = 0.99*n$, rounded to the nearest integer).

---

## Question 3

Suppose someone tells you that they ran PCA in such a way that "95% of the variance was retained." What is an equivalent statement to this?

- [ ] $\frac{ \frac{1}{m} \sum_{i=1}^m ||x^{(i)}- x^{(i)}_{\rm approx}||^2}{\frac{1}{m} \sum_{i=1}^m ||x^{(i)}||^2} \geq 0.05$

- [ ] $\frac{\frac{1}{m} \sum_{i=1}^m ||x^{(i)}||^2}{\frac{1}{m} \sum_{i=1}^m ||x^{(i)}- x^{(i)}_{\rm approx}||^2} \geq 0.95$

- [ ] $\frac{ \frac{1}{m} \sum_{i=1}^m ||x^{(i)}- x^{(i)}_{\rm approx}||^2}{\frac{1}{m} \sum_{i=1}^m ||x^{(i)}||^2} \geq 0.95$

- [x] **$\frac{ \frac{1}{m} \sum_{i=1}^m ||x^{(i)}- x^{(i)}_{\rm approx}||^2}{\frac{1}{m} \sum_{i=1}^m ||x^{(i)}||^2} \leq 0.05$**

---

## Question 4

Which of the following statements are true? Check all that apply.

- [x] **Given an input $x \in \mathbb{R}^n$, PCA compresses it to a lower-dimensional $z \in \mathbb{R}^k$.**

  > PCA compresses it to a lower dimensional vector by projecting it onto the learned principal components. 

- [ ] Feature scaling is not useful for PCA, since the eigenvector calculation (such as using Octave's $\tt svd(Sigma)$ routine) takes care of this automatically.

- [ ] PCA can be used only to reduce the dimensionality of data by 1 (such as 3D to 2D, or 2D to 1D).

- [x] **If the input features are on very different scales, it is a good idea to perform feature scaling before applying PCA.**

  > Feature scaling prevents one feature dimension from becoming a strong principal component only because of the large magnitude of the feature values (as opposed to large variance on that dimension).

---

## Question 5

