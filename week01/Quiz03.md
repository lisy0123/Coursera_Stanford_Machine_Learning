# Linear Algebra

## Question 1

Let two matrices be

$A=\begin{bmatrix}1&-1\\-2&1\\\end{bmatrix}$, $B=\begin{bmatrix}0&3\\5&8\\\end{bmatrix}$

What is $A+B$?

- [x] $\begin{bmatrix}1&-1\\3&9\\\end{bmatrix}$

- [ ] $\begin{bmatrix}1&-1\\7&9\\\end{bmatrix}$

- [ ] $\begin{bmatrix}1&7\\7&9\\\end{bmatrix}$

- [ ] $\begin{bmatrix}1&-7\\-7&-7\\\end{bmatrix}$

  > To add two matrices, add them element-wise.

---

## Question 2

Let $x=\begin{bmatrix}8\\2\\5\\1\end{bmatrix}$

What is $2 * x$?

- [ ] $\begin{bmatrix}4\\1\\\frac52\\\frac12\end{bmatrix}$

- [x] $\begin{bmatrix}16\\4\\10\\2\end{bmatrix}$

- [ ] $\begin{bmatrix}4&1&\frac52&\frac12\end{bmatrix}$

- [ ] $\begin{bmatrix}16&4&10&2\end{bmatrix}$

  > To multiply the vector x by 2, take each element of x and multiply that element by 2. 

---

## Question 3

Let u be a 3-dimensional vector, where specifically

$u=\begin{bmatrix}2\\1\\8\end{bmatrix}$

What is $u^T$?

- [ ] $\begin{bmatrix}8&1&2\end{bmatrix}$

- [ ] $\begin{bmatrix}2\\1\\8\end{bmatrix}$

- [ ] $\begin{bmatrix}8\\1\\2\end{bmatrix}$

- [x] $\begin{bmatrix}2&1&8\end{bmatrix}$

---

## Question 4

Let u and v be 3-dimensional vectors, where specifically

$u=\begin{bmatrix}4\\-4\\-3\end{bmatrix}$

and

$u=\begin{bmatrix}4\\2\\4\end{bmatrix}$

What is $u^Tv$?

(Hine: $u^T$ is a

$1\times3$ dimensional matrix, and v can also seen as a $3\times1$

matrix. The answer you want can be obtained by taking

the matrix product of $u^T$ and $v$.) Do not add brackets to your answer.

> -4

---

## Question 5

Let A and B be $3\times3$ (square) matrices. Which of the following

must necessarily hold true? Check all that apply.

- [x] If B is the $3\times3$ identity matrix, then $A*B=B*A$

  > Even though matrix multiplication is not commutative in general($A*B\ne B*A$ for general matrices $A,\;B$), for the special case where $B=I$, we have $A*B=A*I=A$, and also $B*A=I*A=A$. So $A*B=B*A$.

- [ ] $A*B=B*A$

- [x] If $C=B*A$, then C is a $3\times3$ matrix.

  > Since A and B are both $3\times3$ matrices, their product is $3\times3$. More generally, if A were an $m\times n$ matrix, and B a $n\times o$ matrix, then C would be $m\times o$. (In our example, $m=n=o=3$.)

- [ ] $A*B*A=B*A*B$