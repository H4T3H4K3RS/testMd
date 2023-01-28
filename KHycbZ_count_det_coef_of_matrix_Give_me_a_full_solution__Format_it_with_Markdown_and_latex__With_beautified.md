

**Solution:**

Let A be a matrix of size m x n, then the cofactor of an element A<sub>i,j</sub> is denoted as C<sub>i,j</sub>. 

The cofactor of A<sub>i,j</sub> is given by,

$$C_{i,j}=(-1)^{i+j} det M_{i,j}$$

where $M_{i,j}$ is the Minor of A<sub>i,j</sub>.

The Minor of A<sub>i,j</sub> is the matrix obtained from A by deleting the i<sup>th</sup> row and j<sup>th</sup> column.

Now, the cofactor matrix C (also called the Adjoint) of A is given by,

$$C = \begin{bmatrix}
C_{1,1} & C_{1,2} & \ldots & C_{1,n}\\
C_{2,1} & C_{2,2} & \ldots & C_{2,n}\\
\vdots & \vdots & \vdots & \vdots\\
C_{m,1} & C_{m,2} & \ldots & C_{m,n}\\
\end{bmatrix}$$

Hence, the cofactor of a matrix A is given by the cofactor matrix C.