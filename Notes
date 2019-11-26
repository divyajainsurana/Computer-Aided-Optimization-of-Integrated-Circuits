# Computer Aided Optimsation
### 21 Feb

Inverse Of a Matrix:

AX = B

x = A\B

another way to solve linear equations is 
linsolve(A,B)


### 7 March

LU Decomposition

A square matrix A can be decomposed into two square matrices L and U such that A = L U where U is an upper triangular matrix formed as a result of applying Gauss Elimination Method on A; and L is a lower triangular matrix with diagonal elements being equal to 1.

For A = \begin{bmatrix}   a_{11} & a_{12} & a_{13} \\   a_{21} & a_{22} & a_{23} \\   a_{31} & a_{32} & a_{33}  \end{bmatrix}, we have L = \begin{bmatrix}   1 & 0 & 0 \\   l_{21} & 1 & 0 \\   l_{31} & l_{32} & 1  \end{bmatrix} and U = \begin{bmatrix}   u_{11} & u_{12} & u_{13} \\   0 & u_{22} & u_{23} \\   0 & 0 & u_{33}  \end{bmatrix} ; such that A = L U.


http://www.stat.nctu.edu.tw/misg/SUmmer_Course/C_language/Ch06/LUdecomposition.htm

Gauss Elimination

in this method we reduce the rows of matrix to reduced row-echelon form. ( normally elimination method of linear equations)

Code

A = [1 1 1; 4 3 -1; 3 5 3]

A =

     1     1     1
     4     3    -1
     3     5     3

>> B = [1;6;4]

B =

     1
     6
     4

>> M = [A B]

M =

     1     1     1     1
     4     3    -1     6
     3     5     3     4

>> R = rref(M) : This command converts the matrix into the form of reduced row form

R =

    1.0000         0         0    1.0000
         0    1.0000         0    0.5000
         0         0    1.0000   -0.5000

We conclude that x= 1, y = 0.5 , z = -0.5


Cholesky Decomposition
The Cholesky decomposition of a Hermitian positive-definite matrix A is a decomposition of the form

A=L'*L,
where L is a lower triangular matrix with real and positive diagonal entries, and L' denotes the conjugate transpose of L. Every Hermitian positive-definite matrix (and thus also every real-valued symmetric positive-definite matrix) has a unique Cholesky decomposition.[2]

If the matrix A is Hermitian and positive semi-definite, then it still has a decomposition of the form A = LL' if the diagonal entries of L are allowed to be zero.[3]

When A has only real entries, L has only real entries as well, and the factorization may be written A = LL'.[4]

The Cholesky decomposition is unique when A is positive definite; there is only one lower triangular matrix L with strictly positive diagonal entries such that A = LL'. However, the decomposition need not be unique when A is positive semidefinite.

The converse holds trivially: if A can be written as LL* for some invertible L, lower triangular or otherwise, then A is Hermitian and positive definite.

In matlab we use chol function to compute cholesky factorisation.


### 14 March
Kirchoff Laws

![](https://i.imgur.com/Q6wJxha.jpg)


### 21 March

**A practice Problem: ( recap of Kirchoff Laws)**
![](https://i.imgur.com/cQVSPPD.jpg)

The easiest way to find the matrix A and B is that find the number of resistors between the two nodes.


**Optimisation of a electric circuit**
Use of function fmincom

![](https://i.imgur.com/7XfIFW8.jpg)

optimtool on command line open the optimisation window.

Solution of this:

fun = @(x) (x(2)/(x(1)+x(2)) -0.4)^2; // *objective function*
Aeq = [1,1] //*constraints*
beq = [1]    //*constraints*
A = [-1,0;0 -1]    //*constraints*
b = [0,0]    //*constraints*
x0 = [0.5,1];    //*constraints*
x = fmincon(fun,x0,A,b,Aeq,beq)


##### Intuitive Linear Programming
function: initlinprog

You are given a bag with size 40.  You could pick up any items with values ans size given 
Which products to pick so that size is less than 40 and value is maximised


| Value | 1 | 2| 4| 6|10|12|16|
| ----- | - |- | -| -|- |- |- |
| Size  | 2 | 13|5|7 |21|16|8 |

maximise: x1+2x2+4x3+6x4+10x5+12x6+16x7

Constraints:

[x1:x7]>=0

2x1+13x2+5x3+7x4+21x5+16x6+8x7 <=40

*x = intlinprog(f,intcon,A,b,Aeq,beq,lb,ub)* defines a set of lower and upper bounds on the design variables, x, so that the solution is always in the range lb ≤ x ≤ ub. Set Aeq = [] and beq = [] if no equalities exist.

since in this question we have to maximise but actually this programs minimises it so we use a negative sign.

S = [ 2 13 5 7 21 16 8]
B = [40]
V = [1;2;4;6;10;12;16]
intcon = 1:7

lb = zeros(7,1)

ub =[1;1;1;1;1;1;1]

x= intlinprog(-V,intcon,S,B,[],[],lb,ub)

### 28 march

LTSpice

To know its functioning


######


### 11 April

### 18 April
midterm

### 25 April
Time marching
Forward Euler Method

### 2 May
Convex Optimisation

###### Hessian Matix
###### what is convex problem
[Semidefinite Programming
](https://en.wikipedia.org/wiki/Semidefinite_programming)

### 9 may

###### Gmres (Generalized minimal residual method)

In mathematics, the generalized minimal residual method (GMRES) is an iterative method for the numerical solution of a nonsymmetric system of linear equations. The method approximates the solution by the vector in a Krylov subspace with minimal residual. The Arnoldi iteration is used to find this vector.

Denote the Euclidean norm of any vector v by ‖v‖. Denote the (square) system of linear equations to be solved by
Ax=b



### 16 May

###### Conjuagte Gradient Method


### 23 May

###### Awe moment matching

matlab command : fscanf

http://www.emcs.org/acstrial/newsletters/summer09/HowSpiceWorks.pdf



