# Neural Networks: Representation

## Question 1

Which of the following statements are true? Check all that apply.

- [ ] if a neural network is overfitting the data, one solution would be to decrease the regularization parameter $\lambda$.
- [x] **In a neural network with many layers, we think of each successive layer as being able to use the earlier layers as features, so as to be able to compute increasingly complex functions.**
- [ ] Suppose you have a multi-class classification problem with three classes, trained with a 3 layer network. Let $a^{(3)}_1=(h_\Theta(x))_1$ be the activation of the first output unit, and similarly $a^{(3)}_2=(h_\Theta(x))_2$ and $a^{(3)}_3=(h_\Theta(x))_3$. Then for any input $x$, it must be the case that $a^{(3)}_1+a^{(3)}_2+a^{(3)}_3=1$.
- [x] **if a neural network is overfitting the data, one solution would be to increase the regularization parameter $\lambda$.**

---

## Question 2

Consider the following neural network which takes two binary-valued inputs $x_1,x_2 \in \{0, 1\}$ and outputs $h_\Theta(x)$. Which of the following logical functions does it (approximately) compute?

<img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week04/image1.png" alt="image1" style="zoom:80%;" />

- [x] **NAND (meaning "NOT AND")**
- [ ] AND
- [ ] XOR (exclusive OR)
- [ ] OR

---

## Question 3

Consider the neural network given below. Which of the following equations correctly computes the activation $a_1^{(3)}$? Note: $g(z)$ is the sigmoid activation function. 

<img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week04/image2.png" alt="image2" style="zoom:80%;" />

- [ ] The activation $a^{(3)}_1$ is not present in this network.

- [x] **$a^{(3)}_1=g(\Theta^{(2)}_{1,0}a_0^{(2)}+\Theta^{(2)}_{1,1}a^{(2)}_1+\Theta^{(2)}_{1,2}a_2^{(2)})$**

  > Thiscorrectly uses the first row of $\theta^{(2)}$ and includes the “+1” term of $a^{(2)}_0$).

- [ ] $a^{(3)}_1=g(\Theta^{(1)}_{1,0}a_0^{(1)}+\Theta^{(1)}_{1,1}a^{(1)}_1+\Theta^{(1)}_{1,2}a_2^{(1)})$

- [ ] $a^{(3)}_1=g(\Theta^{(1)}_{1,0}a_0^{(2)}+\Theta^{(1)}_{1,1}a^{(2)}_1+\Theta^{(1)}_{1,2}a_2^{(2)})$

---

## Question 4

You have the following neural network:

<img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week04/image3.png" alt="image3" style="zoom:80%;" />

You'd like to compute the activations of the hidden layer $a^{(2)} \in \mathbb{R}^3$. One way to do so is the following Octave code:

```matlab
% Thetal is Theta with superscript "(1)" from lecture
% ie, the matrix of parameters for the mapping from layer 1 (input) to layer 2
% Thetal has size 3x3
% Assume 'sigmoid' is a built-in function to compute 1 / (1 + exp(-z))

a2 = zeros(3, 1);
for i = 1:3
	for j = 1:3
		a2(i) = a2(i) + x(j) * Theta1(i, j);
	end
	a2(i) = sigmoid (a2(i));
end
```

You want to have a vectorized implementation of this (i.e., one that does not use for loops). Which of the following implementations correctly compute $a^{(2)}$? Check all that apply.

- [ ] a2 = sigmoid (Theta2 * x);
- [ ] z = sigmoid(x); a2 = Theta1 * z;
- [ ] a2 = sigmoid (x * Theta1);
- [x] **a2 = sigmoid (Theta1 * x);**

---

## Question 5

You are using the nerual network pictured below and have learned the parameter $\Theta^{(1)}=\begin{bmatrix}1&2.1&1.3\\1&0.6&-1.2\end{bmatrix}$ (used to compute $a^{(2)}$) and $\Theta^{(2)}=\begin{bmatrix}1&4.5&3.1\end{bmatrix}$ (used to compute $a^{(3)}$) as a function of $a^{(2)}$. Suppose you swap the parameters for the first hidden layer between its two units so $\Theta^{(1)}=\begin{bmatrix}1&0.7&-1.2\\1&2.1&1.3\end{bmatrix}$ and also swap the output layer so $\Theta^{(2)}=\begin{bmatrix}1&3.1&4.5\end{bmatrix}$. How will this change the value of the ouput $h_\Theta(x)$?

<img src="/Users/sangeunlee/lisy/com/Coursera_Stanford_Machine_Learning/week04/image4.png" alt="image4" style="zoom:70%;" />

- [ ] It will increase.
- [ ] It will decrease.
- [ ] Insufficient information to tell: it may increase or decrease.
- [x] **It will stay the same.**