# <u>**Machine Learning Concise Notes**</u>

# Prerequisites

## Linear Algebra

Linear algebra is the branch of mathematics concerning linear equations.

1. ### Matrices

   Matrix is a rectangular array of numbers, symbols, or expressions, arranged in rows and columns.

   ![{\displaystyle \mathbf {A} ={\begin{bmatrix}a_{11}&a_{12}&\cdots &a_{1n}\\a_{21}&a_{22}&\cdots &a_{2n}\\\vdots &\vdots &\ddots &\vdots \\a_{m1}&a_{m2}&\cdots &a_{mn}\end{bmatrix}}={\begin{pmatrix}a_{11}&a_{12}&\cdots &a_{1n}\\a_{21}&a_{22}&\cdots &a_{2n}\\\vdots &\vdots &\ddots &\vdots \\a_{m1}&a_{m2}&\cdots &a_{mn}\end{pmatrix}}=\left(a_{ij}\right)\in \mathbb {R} ^{m\times n}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/599e7d283086f53898bbe2c0f48b6cfcdcda019e)

   

   1. Matrices can be used to compactly write and work with multiple linear equations, that is, systems of linear equations.

   2. * Transpose matrix A = ![\begin{pmatrix}a & b \\ c & d \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7Da%20%26%20b%20%5C%5C%20c%20%26%20d%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2) is a matrix then it’s transpose martix is

        A’=![\begin{pmatrix}a & c \\ b & d\end {pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7Da%20%26%20c%20%5C%5C%20b%20%26%20d%5Cend%20%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2)

      * Zero matrix =(0,0), ![\begin{pmatrix}0 &0 \\ 0 & 0 \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7D0%20%260%20%5C%5C%200%20%26%200%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2), etc.

      * Unit matrix = ![\begin{pmatrix}1 & 0 \\ 0 &1\end{pmatrix},\begin  {pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7D1%20%26%200%20%5C%5C%200%20%261%5Cend%7Bpmatrix%7D%2C%5Cbegin%20%20%7Bpmatrix%7D%201%20%26%200%20%26%200%20%5C%5C%200%20%26%201%20%26%200%20%5C%5C%200%20%26%200%20%26%201%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2), etc.

      * Equal matrices; If A = ![\begin{pmatrix}a & b \\ c & d \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7Da%20%26%20b%20%5C%5C%20c%20%26%20d%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2) and B = ![\begin {pmatrix} x & y \\ z & u \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%20%7Bpmatrix%7D%20x%20%26%20y%20%5C%5C%20z%20%26%20u%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2)

        Then A = B if and only if a=x, b=y, c=z and d=u

        i.e. corresponding elements of the two matrices are equal.

      * Idempotent matrix: A square matrix A Is called idempotent if

      ![A = A^2 = A^3 = \cdots](http://s.wordpress.com/latex.php?latex=A%20%3D%20A%5E2%20%3D%20A%5E3%20%3D%20%5Ccdots&bg=ffffff&fg=000000&s=2)

      * A = ![\begin{pmatrix}a & b \\ c & d \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7Da%20%26%20b%20%5C%5C%20c%20%26%20d%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2) Determinant of A is ![\begin{vmatrix}a & b \\ c & d \end{vmatrix} = (ad - bc)](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bvmatrix%7Da%20%26%20b%20%5C%5C%20c%20%26%20d%20%5Cend%7Bvmatrix%7D%20%3D%20%28ad%20-%20bc%29&bg=ffffff&fg=000000&s=2)

       

      * Inverse of matrix A = ![\begin{pmatrix} a & b \\ c & d \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7D%20a%20%26%20b%20%5C%5C%20c%20%26%20d%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2) is ![ A ^{-1} = \dfrac{1}{|A|} \begin{pmatrix} d & -b \\ -c & a \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%20A%20%5E%7B-1%7D%20%3D%20%5Cdfrac%7B1%7D%7B%7CA%7C%7D%20%5Cbegin%7Bpmatrix%7D%20d%20%26%20-b%20%5C%5C%20-c%20%26%20a%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2)

       

      * Equation in matrix form:

      ![\begin{pmatrix}a _1x + b_1y \\ a_2x +b_2y\end{pmatrix} = \begin{pmatrix} c_1 \\ c_2 \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7Da%20_1x%20%2B%20b_1y%20%5C%5C%20a_2x%20%2Bb_2y%5Cend%7Bpmatrix%7D%20%3D%20%5Cbegin%7Bpmatrix%7D%20c_1%20%5C%5C%20c_2%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2) Then  ![\begin{pmatrix}a _1 & b_1 \\ a_2 & b_2 \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} c_1 \\ c_2 \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7Da%20_1%20%26%20b_1%20%5C%5C%20a_2%20%26%20b_2%20%5Cend%7Bpmatrix%7D%20%5Cbegin%7Bpmatrix%7D%20x%20%5C%5C%20y%20%5Cend%7Bpmatrix%7D%20%3D%20%5Cbegin%7Bpmatrix%7D%20c_1%20%5C%5C%20c_2%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2)

      *  Multiplication of a matrix by a vector:

      ![(a \, b)_{1 \times 2} \begin{pmatrix}x & y \\ z & u \end{pmatrix} _{2 \times 2} = (ax + bz \, ay + bu ) _{1 \times 2}](http://s.wordpress.com/latex.php?latex=%28a%20%5C%2C%20b%29_%7B1%20%5Ctimes%202%7D%20%5Cbegin%7Bpmatrix%7Dx%20%26%20y%20%5C%5C%20z%20%26%20u%20%5Cend%7Bpmatrix%7D%20_%7B2%20%5Ctimes%202%7D%20%3D%20%28ax%20%2B%20bz%20%5C%2C%20ay%20%2B%20bu%20%29%20_%7B1%20%5Ctimes%202%7D&bg=ffffff&fg=000000&s=2)

      * Multiplication of 2 matrices

        ![\begin{pmatrix}a & b \\ c & d \end{pmatrix} \begin{pmatrix} x & y \\ z & u \end {pmatrix} = \begin{pmatrix} ax + bz & ay + bu \\ cx + dz & cy + du \end{pmatrix}](http://s.wordpress.com/latex.php?latex=%5Cbegin%7Bpmatrix%7Da%20%26%20b%20%5C%5C%20c%20%26%20d%20%5Cend%7Bpmatrix%7D%20%5Cbegin%7Bpmatrix%7D%20x%20%26%20y%20%5C%5C%20z%20%26%20u%20%5Cend%20%7Bpmatrix%7D%20%3D%20%5Cbegin%7Bpmatrix%7D%20ax%20%2B%20bz%20%26%20ay%20%2B%20bu%20%5C%5C%20cx%20%2B%20dz%20%26%20cy%20%2B%20du%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2)

        Note: Multiplication of two matrices exists if Number of row of first matrix is equal to number of column to another matrix..

      * Addition and subtraction of matrices:

        ![A \pm B = \begin{pmatrix}a & b \\ c & d \end{pmatrix} \pm \begin{pmatrix}x & y \\ z & u\end{pmatrix} = \begin{pmatrix}a \pm x & b \pm y \\ c \pm z & d \pm u \end{pmatrix}](http://s.wordpress.com/latex.php?latex=A%20%5Cpm%20B%20%3D%20%5Cbegin%7Bpmatrix%7Da%20%26%20b%20%5C%5C%20c%20%26%20d%20%5Cend%7Bpmatrix%7D%20%5Cpm%20%5Cbegin%7Bpmatrix%7Dx%20%26%20y%20%5C%5C%20z%20%26%20u%5Cend%7Bpmatrix%7D%20%3D%20%5Cbegin%7Bpmatrix%7Da%20%5Cpm%20x%20%26%20b%20%5Cpm%20y%20%5C%5C%20c%20%5Cpm%20z%20%26%20d%20%5Cpm%20u%20%5Cend%7Bpmatrix%7D&bg=ffffff&fg=000000&s=2)Multiplication of two matrices:

        

2. ### Vectors

   1. A scalar is a number.
   2. A vector is a list of numbers. 
   3. It can be though as a point in a space or a magnitude and a direction
   4. a = [5,3,6] is a vector in 3 Dimensions, a = [4,3] is a vector in 2 Dimensions

   ![1559694540757](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559694540757.png)

    	5. Magnitude of a vector is the length of a vector.

   $$
   |\vec{a}| = \sqrt {x^2 + y^2}
   $$

   6. Unit Vector is used to represent the direction, magnitude of a unit vector is 1

   ![1559694861059](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559694861059.png)

   7. ![1559694896881](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559694896881.png)

   8. Vector Addition: ![1559694950328](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559694950328.png)

   9. Vector Subtraction: 
      $$
      \vec c=\vec a -\vec b
      $$

   10. If two vectors point in different directions, they are said to be linearly independent. 
   11. **Dot Product** of two vectors generates a scalar value from the product of two vectors.

   $$
   d =\vec a.\vec b
   $$

   12. The **cross product** generates a vector from the product of two vectors.
       $$
       \vec
       c =
       \vec
       a \times
       \vec
       b=\begin{vmatrix} \overrightarrow{i} & \overrightarrow{j} & \overrightarrow{k} \\ a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3 \end{vmatrix}
       $$

   13. Two vectors are orthogonal to one another if the dot product of those two vectors is equal to zero.

   14. The components of a vector are two or more vectors ( Usually vectors along the x , y , z axes) whose vector sum is equal to the given vector.

   15. All vectors live within a vector space.  A vector space is represented using R. A n-dimensional vector space can be represented using 
       $$
       \mathbb{R}^n
       $$
       Eg, Consider a neural network having 5 neurons, 

       State of this network can be depicted as,

       ![1559695600900](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559695600900.png)

       ![1559695795906](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559695795906.png)

       Similarly 
       $$
       s_2=[0,1,0,0,0]\:,
       s_3=[0,0,1,0,0]\:,
       s_4=[0,0,0,1,0]\:,
       s_5=[0,0,0,0,1]
       $$
       By taking combinations of these five basis vectors, and multiplying them by scalar constants, we can describe any state of the network in the entire vector space.

       to generate the network state [0, 3, 0, 9, 0] we could write:

       ![1559696308187](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559696308187.png)

       The definition of a set of basis vectors is twofold:

        (1) linear combinations (meaning addition, subtraction and multiplication by scalars) of the basis vectors can describe any vector in the vector space

        (2) every one of the basis vectors must be required in order to be able to describe all of
       the vectors in the vector space.

   16.  A basis set is a linearly independent set of vectors that, when used in linear combination, can represent every vector in a given vector space.

        The *xy*-coordinate plane has dimension 2.  The standard basis consists of the two vectors (1,0) and (0,1). Any two independent vectors will also form a basis, for example, (3,8) and (−4,0) will form a basis of this plane.

   ​    

3. ### Linear Transformations

   1. Linear transformations are the set of all functions that can be written as a matrix
      multiplication
   2. They can also be thought as functions from one vector space into another vector space
   3. A transformation function maps set of X to set of Y

   $$
   i.e, f(X):X→Y
   $$

   3. A Linear Transformation is a function that maps X->Y while preserving linearity (Addition and Scalar Multiplication properties of Vectors/Matrices)

   $$
   f(\mathbf{u}+\mathbf{v}) = f(\mathbf{u})+f(\mathbf{v}) 
   \\
   f(c \mathbf{u}) = c f(\mathbf{u})
   $$

   4. Examples are Rotation, Translation, Scaling, Identity Operation, Reflection and Shearing

   5. Let us take the projection of vectors in R<sup>2</sup> to vectors on the x-axis. Let's call this transformation T.

      We know that T maps vectors from R<sup>2</sup> to R<sup>2</sup>, so we can say 
      $$
      T: \mathbb{R}^2 \rightarrow \mathbb{R}^2
      \\
      T\begin{pmatrix} x_0 \\ x_1 \end{pmatrix} = \begin{pmatrix} x_0 \\ 0 \end{pmatrix}
      \\
      $$
      Since this transformation preserves both addition and scalar multiplication properties, it is linear.

   6. The *kernel* of a linear transformation T: V -> W is the set of all vectors in V which are mapped to the zero vector

   $$
   \mathrm{ker}\ T = \{v \in V\ |\ T\mathbf{v} = \mathbf{0}\}
   \\
   i.e,  Ax=0
   $$

   7. The *image* of a linear transformation T:V->W is the set of all vectors in W which were mapped from vectors in V. For Example, if T(1)=2, then image of 2 is 1.

4. ### Determinants

   1. Determinant is a scalar value that can be computed from the elements of a square matrix and encodes certain properties of the linear transformation described by the matrix.
   2. It can be viewed as the volume scaling factor of the linear transformation described by the matrix.
   3. It is denoted by

   $$
   det(A)\:or\:det\:A\:or\:|A|
   $$

   4. For a 2X2 Matrix,

   $$
   \begin{align}|A| = \begin{vmatrix} a & b\\c & d \end{vmatrix}=ad - bc .\end{align}
   $$

   5. For a 3X3 Matrix,

   $$
   \begin{align}
     |A| = \begin{vmatrix} a & b & c \\ d & e & f \\ g & h & i \end{vmatrix}
        &= a\,\begin{vmatrix} \Box & \Box & \Box \\ \Box & e & f \\ \Box & h & i \end{vmatrix} - 
           b\,\begin{vmatrix} \Box & \Box & \Box \\ d & \Box & f \\ g & \Box & i \end{vmatrix} + 
           c\,\begin{vmatrix} \Box & \Box & \Box \\ d & e & \Box \\ g & h & \Box \end{vmatrix} \\[3pt]
        &= a\,\begin{vmatrix} e & f \\ h & i \end{vmatrix} - 
           b\,\begin{vmatrix} d & f \\ g & i \end{vmatrix} + 
           c\,\begin{vmatrix} d & e \\ g & h \end{vmatrix} \\[3pt]
        &= aei + bfg + cdh - ceg - bdi - afh.
   \end{align}
   $$

   6. Each determinant of a (n-1) ×(n-1) matrix in this equation is called a "minor" of the matrix A.
   7. In linear algebra, an n-by-n square matrix A is called invertible (also nonsingular or nondegenerate) if there exists an n-by-n square matrix B such that 

   $$
   AB=BA=I_n
   $$

   8. Cofactor is the determinant of a minor. A cofactor matrix is the matrix of cofactors.
   9. An Adjugate matrix or adjoint matrix is the transpose of cofactor matrix.
   10. Inverse of a matrix can also be defined as,

   $$
   A^{-1}=\frac{1}{det(A)}adj(A)
   $$

   

5. ### Eigenvalue and Eigenvectors 

   1. Eigenvector or characteristic vector of a linear transformation is a non-zero vector that changes by only a scalar factor when that linear transformation is applied to it.
   2. This scalar factor is called as an Eigen Value.

   $$
   i.e, T(v)=\lambda v
   $$

   3. Since every matrix is a linear transformation,

   $$
   Av=\lambda v
   $$

   4.  Eigenvalue can be defined as **largest effect on input**
   5. Eigenvector is the vector (or direction) that has the largest effect.

   ![img](https://upload.wikimedia.org/wikipedia/commons/3/3c/Mona_Lisa_eigenvector_grid.png)

   In this shear mapping the red arrow changes direction but the blue arrow does not. The blue arrow is an eigenvector of this shear mapping because it does not change direction, and since its length is unchanged, its eigenvalue is 1.

  6. v is the eigenvector of matrix A if the following equation is true

        		![{\displaystyle (A-\lambda I)v=0,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/c23473bf4e5986fe7b3759e686dae74f16646a2f)

        where I is the identity matrix.

      This equation has a non zero solution only if,

     ![{\displaystyle |A-\lambda I|=0}](https://wikimedia.org/api/rest_v1/media/math/render/svg/1f51f610b43bbf9a5d794d835b70fa145befb412)

     Example,

     ![{\displaystyle M={\begin{bmatrix}2&1\\1&2\end{bmatrix}}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/9d527f10c9b73c73780c8fb6ecea77282310cd4e)

     ![{\displaystyle |M-\lambda I|={\begin{vmatrix}2-\lambda &1\\1&2-\lambda \end{vmatrix}}=3-4\lambda +\lambda ^{2}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/54df3aacb533c43c0eca088fb799c2dcdf2c28eb)

     Setting the characteristic polynomial equal to zero, it has roots at λ = 1 and λ = 3, which are the two eigenvalues of *M*. The eigenvectors corresponding to each eigenvalue can be found by solving for the components of *v* in the equation *Mv* = *λv*. In this example, the eigenvectors are any non-zero scalar multiples of

     ![{\displaystyle v_{\lambda =1}={\begin{bmatrix}1\\-1\end{bmatrix}},\quad v_{\lambda =3}={\begin{bmatrix}1\\1\end{bmatrix}}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/bd6c1eb876047bb69a8da6eb65129aadea4b428a)

7. Let A be a square n × n matrix with n linearly independent eigenvectors qi (where i = 1, ..., n). Then A can be factorized as 

![\mathbf{A}=\mathbf{Q}\mathbf{\Lambda}\mathbf{Q}^{-1}  ](https://wikimedia.org/api/rest_v1/media/math/render/svg/4e0edeaafb9644ef4c52881019a256add81d1356)

​	where Q is the square n × n matrix whose ith column is the eigenvector qi of A, and Λ is the      diagonal matrix whose diagonal elements are the corresponding eigenvalues, Λii = λi. Note that only diagonalizable matrices can be factorized in this way. 

A is called diagonalizable or non-defective if it is similar to a diagonal matrix,  if there exists an invertible matrix P such that P <sup>− 1</sup> A P is a diagonal matrix.

The decomposition can be derived from the fundamental property of eigenvectors:

![{\displaystyle {\begin{aligned}\mathbf {A} \mathbf {v} &=\lambda \mathbf {v} \\\mathbf {A} \mathbf {Q} &=\mathbf {Q} \mathbf {\Lambda } \\\mathbf {A} &=\mathbf {Q} \mathbf {\Lambda } \mathbf {Q} ^{-1}.\end{aligned}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/d5959a7b9ece5ccc993166b2f61f1d1b712f8be5)

Example,

The 2 × 2 real matrix **A**

![\mathbf{A} = \begin{bmatrix} 1 & 0 \\ 1 & 3 \\ \end{bmatrix}](https://wikimedia.org/api/rest_v1/media/math/render/svg/8eb8a3a1a61236fcff1a3626f7314badd043cbfb)

may be decomposed into a diagonal matrix through multiplication of a non-singular matrix **B**

![{\displaystyle \mathbf {B} ={\begin{bmatrix}a&b\\c&d\end{bmatrix}}\in \mathbb {R} ^{2\times 2}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/b6fc8d0433a8750525dd720f77b47c8dfd6c6294)

Then

![{\displaystyle {\begin{bmatrix}a&b\\c&d\end{bmatrix}}^{-1}{\begin{bmatrix}1&0\\1&3\end{bmatrix}}{\begin{bmatrix}a&b\\c&d\end{bmatrix}}={\begin{bmatrix}x&0\\0&y\end{bmatrix}},}](https://wikimedia.org/api/rest_v1/media/math/render/svg/8379917a3e462547a942ca779777b4f1c5e3ce00)

Multiplying both sides of the equation on the left by **B**:

![{\displaystyle {\begin{bmatrix}1&0\\1&3\end{bmatrix}}{\begin{bmatrix}a&b\\c&d\end{bmatrix}}={\begin{bmatrix}a&b\\c&d\end{bmatrix}}{\begin{bmatrix}x&0\\0&y\end{bmatrix}}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/c25f03d07d4ad15a1675e19146e361a7e0826b11)

The above equation can be decomposed into two simultaneous equations,

![{\displaystyle {\begin{cases}{\begin{bmatrix}1&0\\1&3\end{bmatrix}}{\begin{bmatrix}a\\c\end{bmatrix}}={\begin{bmatrix}ax\\cx\end{bmatrix}}\\{\begin{bmatrix}1&0\\1&3\end{bmatrix}}{\begin{bmatrix}b\\d\end{bmatrix}}={\begin{bmatrix}by\\dy\end{bmatrix}}\end{cases}}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/9c2a910bb46119fa8b9cad84b0516ed7e269083c)

![ \begin{cases} \begin{bmatrix} 1 & 0\\ 1 & 3 \end{bmatrix} \begin{bmatrix} a \\ c \end{bmatrix} = x\begin{bmatrix} a \\ c \end{bmatrix} \\ \begin{bmatrix} 1 & 0\\ 1 & 3 \end{bmatrix} \begin{bmatrix} b \\ d \end{bmatrix} = y\begin{bmatrix} b \\ d \end{bmatrix} \end{cases} ](https://wikimedia.org/api/rest_v1/media/math/render/svg/a470eb5aae455023e456d7bd7f057dea2da7da5b)

Let,

![{\displaystyle {\overrightarrow {a}}={\begin{bmatrix}a\\c\end{bmatrix}},\quad {\overrightarrow {b}}={\begin{bmatrix}b\\d\end{bmatrix}},}](https://wikimedia.org/api/rest_v1/media/math/render/svg/38d601d54c641fa0598628f795b8974fff3b800e)

Then

![ \begin{cases} A \overrightarrow{a} = x \overrightarrow{a} \\ A \overrightarrow{b} = y \overrightarrow{b} \end{cases}](https://wikimedia.org/api/rest_v1/media/math/render/svg/c0ed21324d651360ea5a580c2cae08fde438f707)

And can be represented by a single vector equation involving two solutions as eigenvalues

![\mathbf{A} \mathbf{u} = \lambda \mathbf{u}](https://wikimedia.org/api/rest_v1/media/math/render/svg/4a4e5cd752aa08d13eb76c4a78bc55851010f810)

Solving for eigenvalues, we get

![{\displaystyle (1-\lambda )(3-\lambda )=0}](https://wikimedia.org/api/rest_v1/media/math/render/svg/9bb77447a5952462ac056bb8693d6e3c5ec40359)

![ \begin{cases} \begin{bmatrix} 1 & 0 \\ 1 & 3 \end{bmatrix} \begin{bmatrix} a \\ c \end{bmatrix} = 1\begin{bmatrix} a \\ c \end{bmatrix} \\ \begin{bmatrix} 1 & 0\\ 1 & 3 \end{bmatrix} \begin{bmatrix} b \\ d \end{bmatrix} = 3\begin{bmatrix} b \\ d \end{bmatrix} \end{cases} ](https://wikimedia.org/api/rest_v1/media/math/render/svg/1eeb8b5a43502c215a07897da826ed1e9239ca22)

![{\displaystyle a=-2c\quad {\text{and}}\quad b=0,\qquad [c,d]\in \mathbb {R} .}](https://wikimedia.org/api/rest_v1/media/math/render/svg/0b8fc478728f728220f7d6fb4ede83bd97090c2d)

![{\displaystyle \mathbf {B} ={\begin{bmatrix}-2c&0\\c&d\end{bmatrix}},\qquad [c,d]\in \mathbb {R} ,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/35aa552222b28c189ebaa7b6d2bb8c1c43bf7a26)

![{\displaystyle {\begin{bmatrix}-2c&0\\c&d\end{bmatrix}}^{-1}{\begin{bmatrix}1&0\\1&3\end{bmatrix}}{\begin{bmatrix}-2c&0\\c&d\end{bmatrix}}={\begin{bmatrix}1&0\\0&3\end{bmatrix}},\qquad [c,d]\in \mathbb {R} }](https://wikimedia.org/api/rest_v1/media/math/render/svg/6bb6af6220a8da5b28b8642103d097dab3a7ee81)

8. Eigenvalue and Eigenvectors are used extensively in Dimensionality Reduction. in Principal Component Analysis, Eigenvalue of covariance matrix depicts variance, and eigenvector depicts the vector or direction having highest variance.
9. Rank of a matrix is equivalent to the maximum number of linearly independent columns of A.

## Statistics and Probability

Statistics is basically the mathematical study and interpretation of data. Statistics can be used as a powerful tool to analyze data.

**Descriptive Statistics** is a type of statistics used to describe patterns and insights in data. This includes measures of central tendency, spread etc.

**Inferential Statistics** is a type of statistics used to make conclusions from data.

1. ### Measures of Central Tendency

   1. **Mean**: Gives the average of all data points
      $$
      Mean=\frac{\sum_{i=1}^{n} {x_i}} {n}
      $$

   2. **Median:** It is the middle most value we get when we sort our data. For even number of data points, median is the mean of middle two data points. 

   3. **Mode:** It is the value that appears most in the dataset.

2. ### Measures of Spread

   1. **Range:** It is the difference between two extreme points.

   $$
   Range=Highest\:Value - Lowest\:Value
   $$

   2. **Inter-Quartile Range:** It is the difference between first two quartiles' and last two quartiles' Median.

   $$
   IQT=Median(Q3,Q4)-Median(Q1,Q2)
   $$

   3. **Deviation:** Difference of each data point from the mean.
   4. **Variance:**  It measures how far a set of numbers are spread out from their average value.

   $$
   Variance = {\frac{1}{N-1} \sum_{i=1}^N (x_i - \overline{x})^2}
   $$

   5. **Standard Deviation:** Average amount of deviation we expect the points from the mean

   $$
   SD = \sqrt{Variance}
    = \sqrt{\frac{1}{N-1} \sum_{i=1}^N (x_i - \overline{x})^2}
   $$

   

3. ### Correlation

   1. Measure of the way two variables move together both in direction and closeness of their movement. 
   2. Coefficient of Correlation is the numerical way to represent or measure correlation
   3. Pearson's *r*, is a measure of the strength and direction of the linear relationship between two variables 
   4. ![Image result for karl pearson correlation formula](https://businessjargons.com/wp-content/uploads/2016/04/Karl-Pearson-final.jpg)
   5. **R Squared** can be used to determine the amount of variance in the prediction. It ranges from 0 to 1.
   6. Just because two variables are correlated doesn't mean one causes another

   $$
   i.e, Correlation \neq Causation
   $$

   

4. ### Event

   1. An **event** is a set of outcomes of an experiment (a subset of the sample space) to which a **probability** is assigned.
   2. A single outcome may be an element of many different events.

5. ### Random Variables

   1. A variable whose values depends on outcomes of a random phenomenon
   2. Also Known as **random quantity** or **stochastic variable** 

6. ### Addition Rule and Multiplication Rule

   $$
   Addition\:Rule :P(A)\:\cup\:P(B)=P(A)+P(B)-P(A)\cap P(B)
   $$

   $$
   Multiplication\:Rule :P(A)\:\cap\:P(B)=P(A)*P(B)
   $$

   

7. ### Distributions

   1. **Binomial Distribution:** Distribution of probability of x being true out of n

   $$
   P=n_{C_x}\:p^xq^{n-x}
   $$

   2. **Bernoulli Distribution:** Special case of Binomial Distribution where n=1

   $$
   P=p^x(1-p)^{1-x}
   $$

   3. **Geometric Distribution:** The geometric distribution gives the probability that the first occurrence of success requires *k* independent trials, each with success probability *p*. 

   $$
   \Pr(X = k) = (1-p)^{k-1}p
   $$

   4. **Continuous Distribution: ** A **continuous probability distribution** is a probability distribution that has a cumulative distribution function that is continuous.

   $$
   \operatorname{P}[a\le X\le b] = \int_a^b f(x) \, dx
   $$

   5. **Normal distribution:** also known as the **Gaussian distribution**, is a probability **distribution** that is symmetric about the mean, showing that data near the mean are more frequent in occurrence than data far from the mean.

   $$
   f(x \mid \mu, \sigma^2) = \frac{1}{\sqrt{2\pi\sigma^2} } e^{ -\frac{(x-\mu)^2}{2\sigma^2} }
   $$

   ![File:Normal Distribution PDF.svg](https://upload.wikimedia.org/wikipedia/commons/thumb/7/74/Normal_Distribution_PDF.svg/720px-Normal_Distribution_PDF.svg.png)

   6. **Poisson Distribution:** is a discrete probability distribution that expresses the probability of a given number of events occurring in a fixed interval of time or space if these events occur with a known constant rate and independently of the time since the last event.

   $$
   P(k \text{ events in interval}) = e^{-\lambda}\frac{\lambda^k}{k!}
   $$

   7. **Student's-t Distribution :** The **t distribution** (aka, Student's **t**-**distribution**) is a probability **distribution** that is used to estimate population parameters when the sample size is small and/or when the population variance is unknown.

   ![Student t pdf.svg](https://upload.wikimedia.org/wikipedia/commons/thumb/4/41/Student_t_pdf.svg/800px-Student_t_pdf.svg.png)

   8. **Exponential Distribution:** It is the continuous analogue of the geometric distribution,  is the probability distribution of the time between events in a Poisson point process (Which is a set of random points in sample space)

8. ### **Central Limit Theorem**

   * Most Distributions get closer and closer to a normal distribution as sample set increases.

   * A Confidence Interval is a **range of values**  we are fairly sure our **true value** lies in.

9. ### Bayes Theorem and Applications

   1. Bayes Theorem describes the probability of an event, based on prior knowledge of conditions that might be related to the event. i.e, conditional probability of events.

   $$
   P(A/B)=\frac {P(B/A)\:P(A)} {P(B)}
   $$

   2. Core idea of Bayes Theorem is updating what you believe using new information.
   3. Bayes Theorem has lots of applications in Business, Medicine, Spam Filtering etc.
   4. Lots of Machine Learning techniques are based on Bayes Theorem such as Naïve Bayes Classifier, EM Clustering, MAP, LDA etc.
   5. **Probabilistic graphical model (PGM)** or structured probabilistic model is a probabilistic model for which a graph expresses the conditional dependence structure between random variables. They are commonly used in probability theory, statistics—particularly Bayesian statistics—and machine learning.   
   6. **Bayesian Network **is a probabilistic graphical model (a type of statistical model) that represents a set of variables and their conditional dependencies via a directed acyclic graph (DAG).

   ![img](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fd/SimpleBayesNetNodes.svg/1280px-SimpleBayesNetNodes.svg.png)

   ​		A simple Bayesian network. Rain influences whether the sprinkler is 
   ​		activated, and both rain and the sprinkler influence whether the grass 
   ​		is wet.

10. ### Inferential Statistics

    1. Statistical inference is the process of using data analysis to deduce properties of an underlying probability distribution.
    2. **Hypothesis:** It is a statement that needs to be proved.
    3. **Null Hypothesis:** The null hypothesis is generally assumed to be true until evidence indicates otherwise. It is denoted as ***H0***.
    4. **Alternative Hypothesis:** It is the opposite of Null Hypothesis.
    5. **P-Values:** Tells the extremity of data. If P value is low, Null Hypothesis is rejected. If P value is greater than cutoff, its a failure to reject null Hypothesis.
    6. **Type I Error: ** Rejecting Null Hypothesis even if its true
    7. **Type II Error: **Accepting Null Hypothesis when its false.

11. ### Tests

    1. **Student's-t Test:** It is used to determine whether there is a significant difference between the means of two groups. 

       H0 -> Means are equal

       Ha -> Means are not equal

    $$
    T=\frac{\overline X -\mu}{S.D/\sqrt{n}}
    $$

    $$
    Where \: \sqrt{n}=\sqrt{\sigma^2_1/N1+\sigma^2_2/N2}
    $$
    2. **Chi-Squared test:** It **tests** to see whether distributions of categorical variables differ from each another. A very small **chi square test** statistic means that your observed data fits your expected data extremely well.

    $$
    \chi^2=\frac{\sum{(\overline{X}-\mu)^2}} {\mu}
    $$

    3. **F-test:** The F-Test to Compare Two Variances. However, the f-statistic is used in a variety of tests including regression analysis and ANOVA. It uses an F-Distribution ( right-skewed **distribution**).

       1. For Regression,  (SSR-> Sum of Squares of regression, SSE -> Sum of Squares of Error, DF-> Degree of freedom)
          $$
          F=\frac {SSR/DF} {SSE/DF}s
          $$

       2. For ANOVA or Varience, 

       $$
       F = \frac{\text{explained variance}}{\text{unexplained variance}}
       $$

    4. **Z-Scores:** *z*-*score* is the number of standard deviations from the mean a data point is.

    $$
    Z=\frac{x-\mu}{\sigma}
    $$

    

12. ### Degree of Freedom

    1. The number of independent ways by which a dynamic system can move, without violating any constraint imposed on it, is called number of **degrees of freedom**.

13. ### Joint Probability 

    1. Joint probability is the probability of two events happening together. The two events are usually designated *event A* and *event B.* In probability terminology, it can be written as:
       
       $$
       p(A\: and\: B)
       
       \:or\:
       
       p(A ∩ B)
       $$
        Joint probability is also called the intersection of two (or more) events.
       $$
       f(x,y) = P(X = x, Y = y)
       $$

    2.  **Covariance** is a measure of the joint variability of two random variables.

       The covariance between two jointly distributed real-valued random variables  X and Y with finite second moments is defined as the expected product of their deviations from their individual expected values.
       $$
       cov(X,Y)=\frac{(X-E(X)(Y-E(Y)))}{n-1}
       $$
       Where E(X) and E(Y) are expectations or mean.

       Correlation,
       $$
       r_{(x,y)}=\frac{cov(x,y)}{s_xs_y}
       $$

14. ### **Stochastic Process** and Markov Chain

    1. Stochastic process represents numerical values of some system randomly changing over time.

    2. A Markov chain is a stochastic model describing a sequence of possible events in which the probability of each event depends only on the state attained in the previous event.

    3. The Markov property refers to the memoryless property of a stochastic process. 

       A stochastic process has the Markov property if the conditional  probability distribution of future states of the process depends only  upon the present state, not on the sequence of events that preceded it. 

    ![img](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2b/Markovkate_01.svg/800px-Markovkate_01.svg.png)

    ​	Markov Chains are probabilistic whereas Finite State Machines are generally deterministic.

    ​	In simpler Markov models (like a Markov chain), the state is directly visible to the observer, 	and therefore the state transition probabilities are the only parameters, while in the hidden 	Markov model, the state is not directly visible, but the output dependent on the state, is	           	visible.

    4. A Stochastic matrix is a square matrix used to describe the transitions of a Markov chain. Each of its entries is a nonnegative real number representing a probability.
    5. **A Stochastic vector** (also called **probability vector**) as a vector whose elements are nonnegative real numbers which sum to 1.

    $$
    P=\left[\begin{matrix}
    P_{1,1}&P_{1,2}&\dots&P_{1,j}&\dots&P_{1,S}\\
    P_{2,1}&P_{2,2}&\dots&P_{2,j}&\dots&P_{2,S}\\
    \vdots&\vdots&\ddots&\vdots&\ddots&\vdots\\
    P_{i,1}&P_{i,2}&\dots&P_{i,j}&\dots&P_{i,S}\\
    \vdots&\vdots&\ddots&\vdots&\ddots&\vdots\\
    P_{S,1}&P_{S,2}&\dots&P_{S,j}&\dots&P_{S,S}\\
    \end{matrix}\right]
    $$

    $$
    \sum_{j=1}^S P_{i,j}=1\
    $$

    Since the total of transition probability from a state ![i](https://wikimedia.org/api/rest_v1/media/math/render/svg/add78d8608ad86e54951b8c8bd6c8d8416533d20) to all other states must be 1.

    A **right stochastic matrix** is a real square matrix, with each row summing to 1.

    A **left stochastic matrix** is a real square matrix, with each column summing to 1.

## Calculus 

1. ### Limits

   1. Limit is the value that a function approaches when the input approaches some value
   2. ![{\displaystyle f(x)\to L{\text{ as }}x\to c.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/107c9e2e66ea05b4d6ecbba70bdf35953f10b565)

   $$
   \displaystyle \lim _{x\to c}{f(x)=L}
   $$

2. ### Basic Differential Calculus

   1. A derivative is rate of change of a function (can be represented as a slope graphically) or slope of a line at specific point.
   2. ![_images/slope_formula.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/slope_formula.png)
   3. Derivative can be represented as

   $$
   \lim _{h\to 0} \frac {f(x+h)−f(x)}h
   $$

   4. Machine learning uses derivatives in optimization problems. Optimization algorithms like *gradient descent* use derivatives to decide whether to increase or decrease weights in order to maximize or minimize some objective.

   5. Chain Rule: *f*(*x*)=*h*(*g*(*x*))

      then, 
      $$
      \frac {df} {dx}=\frac {dh} {dg}⋅\frac {dg} {dx}
      $$

   6. A gradient is a vector that stores the partial derivatives of multivariable functions. 

      It helps us calculate the slope at a specific point on a curve for functions with multiple independent variables. 

   7. In functions with 2 or more variables, the **partial derivative** is the derivative of one variable with respect to the others.

   8. 
      $$
      For \:f(x,y), \\
      \frac{\partial x}{\partial y}
      \:,\:
      \frac{\partial y}{\partial x}\\
      are\: partial\: derivatives
      $$

   9. Gradient Vector can be represented as

   $$
   \nabla f = \frac{\partial f}{\partial x} \mathbf{i} + \frac{\partial f}{\partial y} \mathbf{j} + \frac{\partial f}{\partial z} \mathbf{k}
   $$

   $$
   \nabla f=\begin{pmatrix}  \frac{\partial f}{\partial x} \\ \frac{\partial f}{\partial y} \\ \frac{\partial f}{\partial z}\end{pmatrix}
   $$

   10. Directional derivatives help us find the slope if we move in a direction different from the one specified by the gradient.

       If v is the directional vector, directional derivative is the dot product of gradient and v
       $$
       Directional\: Derivative=\nabla.\vec v
       $$
       It can also be written as
       $$
       \nabla _\vec v f
       $$
       Where f is the function.

3. ### Basic Integral Calculus

   1. The integral of *f*(*x*) corresponds to the computation of the area under the graph of *f*(*x*). The area under *f*(*x*) between the points *x*=*a* and *x*=*b* is denoted as follows:

   2. $$
      A(a,b)=\int_a^bf(x)dx=F(b)−F(a)
      $$

   3. ![_images/integral_definition.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/integral_definition.png)

   4. Integrals can be used to calculate Probability,Expectation and Variance of continuous distributions 

## Optimization and Numerical Methods

### Gradient Descent (Batch Gradient Descent)

Gradient descent is a first-order iterative optimization algorithm for finding the minimum of a function. 

To find a local minimum of a function using gradient descent, one takes steps proportional to the negative of the gradient (or approximate gradient) of the function at the current point.

If, instead, one takes steps proportional to the positive of the gradient, one approaches a local maximum of that function; the procedure is then known as gradient ascent.

![Image result for gradient descent](https://mukulrathi.com/static/b4793bf4ff6f9063ff9a3d00f1ebf6ec/e2622/grad-descent.png)



Given cost function J for linear regression
$$
J(\theta_0,\theta_1)=\frac{1}{2}\sum_{i=0}^m (h_\theta(x^{(i)})-y^{(i)})^2
$$
Gradient Descent algorithm :

* Start with some random values for theta0 and theta1. Keep changing the values until we end up at minimum

$$
repeat\:until\:convergence\:\{\\
\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\:\
\theta_j=\theta_j-\alpha\:\frac{\partial(\theta_0,\theta_1)}{\partial\theta_j} \:for\:j=0,1
\\\}
$$



#### 	Stochastic Gradient Descent

Stochastic gradient descent (often abbreviated SGD) is an iterative method for optimizing an objective function .

It is called stochastic because the method uses randomly selected (or shuffled) samples to evaluate the gradients, hence SGD can be regarded as a stochastic approximation of gradient descent optimization.

![sgdns](https://cdncontribute.geeksforgeeks.org/wp-content/uploads/sgdn.png)

### Other Methods

#### Newton's Method

Newton's method is applied to the derivative f ′ of a twice-differentiable function f to find the roots of the derivative such as minima or maxima.
$$
x_{k+1}=x_k-\frac{f(x_k)}{f^\prime(x_k)}
$$

#### Momentum

Used in conjunction Stochastic Gradient Descent (sgd) or Mini-Batch Gradient Descent, Momentum takes into account past gradients to smooth out the update. This is seen in variable *v* which is an exponentially weighted average of the gradient on previous steps. This results in minimizing oscillations and faster convergence.
$$
v=\beta+(1-\beta)\theta_t \: where \:\theta=function
$$

$$
W=W-\alpha v
$$

#### RMSProp

Root Mean Square Prop (RMSProp) works by keeping an exponentially weighted average of the squares of past gradients.
RMSProp then divides the learning rate by this average to speed up convergence.
$$
W=W-\alpha\frac{\theta_t}{\sqrt{v_{corrected}}+\epsilon}
$$
Where epsilon is a small value to avoid dividing by zero

#### Adam

Adaptive Moment Estimation (Adam) combines ideas from both RMSProp and Momentum. It computes adaptive learning rates for each parameter and works as follows.

First, it computes the exponentially weighted average of past gradients. Then, it computes exponentially weighted average of squares of these gradients.

 These averages have a bias towards zero and to counteract this a bias correction is applied.

Lastly, the parameters are updated using the information from the calculated averages.
$$
W=W−α\frac{v_{corrected}}{\sqrt s_{corrected}+ε}
$$
Where,
$$
s=\beta+(1-\beta)\theta_t^2 \: where \:\theta=function
$$

$$
v_{corrected}=\frac{v}{(1-(\beta_1)^t)}\\
s_{corrected}=\frac{s}{(1-(\beta_1)^2)}
$$

### Curve Fitting

Curve fitting is the process of constructing a curve, or mathematical function, that has the best fit to a series of data points,possibly subject to constraints.

#### Fitting lines

The first degree polynomial equation

![Linear regression.svg](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Linear_regression.svg/220px-Linear_regression.svg.png)
$$
y = a x + b
$$
The one line that provides a minimum error is then the ‘best’ straight line. Least squares approach minimizes sum of squared errors.

![{\displaystyle S=\sum _{i=1}^{n}{r_{i}}^{2}.}](https://wikimedia.org/api/rest_v1/media/math/render/svg/1d981504049676791db33a65c6907f5b3f2c2cce)

#### Fitting Parabola

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/9/94/Linear_least_squares2.png/220px-Linear_least_squares2.png)

![y=ax^{2}+bx+c\;.](https://wikimedia.org/api/rest_v1/media/math/render/svg/225fdd72549b6b0e8b1986750ae6123fba845efd)

#### Fitting Third Degree Polynomial

![y=ax^{3}+bx^{2}+cx+d\;.](https://wikimedia.org/api/rest_v1/media/math/render/svg/30bc759aafe82340950f5d4f40b1995a0e101bed)

#### Exponential Curve Fitting

$$
y = a.b^x + c
$$



## Basic Python Refresher (From https://intellipaat.com/)

#### **Basic rules to write Python syntax:**

```php
Rule #1: Python is white-space dependent; code blocks are indented using spaces.

Rule #2: Python language is case sensitive. It matters for variables, functions and any keyword in general.
```

#### Data Types

```php
 	Numbers: a=2(Integer), b=2.0(Float), c=1+2j(Complex)
 	List: a=[1,2,3,’Word’]
 	Tuple: a= (1,2,4)
 	String: a=“New String”
 	Sets: a= {2,3,4,5}
 	Dictionary: x= {‘a’: [1,2],‘b’: [4,6]
```

#### **Operators**

In python, Operators are only the constructs which can manipulate the  value of operands. For example, in the expression 5 + 10 = 15. Here, 5  and 10 are operands and + is operator.

#####  	Numeric Operator (Say, a holds 5, b holds 10)


 	a + b = 15

 	a – b = -5

 	a * b = 50

 	b/a = 2

 	b % a = 0

 	a**b =510 

 	0//2.0 = 3.0, -11//3 = -4



 	Comparison Operator


 	(a == b): not true

 	(a!= b): true

 	(a > b): not true.

 	(a > b): not true

 	(a >= b): not true

 	(a <= b) is true



 	Boolean Operator


 	a and b

 	a or b

 	not a

#### **Operations**

Python provides some of the built-in operations on various data types.

```php
 	List Operations

 	List=[]:Defines an empty list
 	list[i]=a: Stores a at the ith position
 	list[i]: Retrieves the character at the ith position
 	list[i:j]: Retrieves characters in the range i to j
 	append(val): Adds item at the end
 	pop([i]): Removes and returns item at index i


 	String Operations

 	String[i]: Retrieves the character at the ith position
 	String[i:j]: Retrieves characters in the rangei to j


 	Dictionary Operations 

 	dict={} : Defines an empty dictionary
 	dict[i]=a: stores “a” to the key “i”
 	dict[i]: Retrieves the item with the key “i”
 	key: Gives all the key items
 	values: Gives all the values
```

#### **Flow Control Method:**

Python programming language provides various looping and control  statement that allow for more complicated execution paths.A loop  statement allows us to execute a statement or group of statements  multiple times.

```php
 	if-else (Conditional Statement):

if price>=700:
print(“Buy.”)
else:
print(“Don’t buy.”)


 	For loop (Iterative Loop Statement):

a=“New Text”
count=0
for i in a:
if i==‘e’:
count=count+1
print(count)


 	While loop (Conditional Loop Statement):

a=0
i=1
while i<10:
a=a*2
i=i+1
print(a)


 	Loop Control: Break, Pass and continue
```

#### Functions

A function is a block of code which only runs when it is called. We  can pass data (parameters) into a function and after executing a  function, it will return data as a result.

```php
def new_function():
print(“Hello World”)
new_function()
```

#### Lambda Function

A lambda function is a small anonymous function. It can take any number of arguments but can only have one expression.

```php
lambda a,b: a+b
lambda a,b: a*b
```

#### Generic Operations

In python, we have a huge a list of Python built-in functions. Some of them are:

```php
 	range(5): 0,1,2,3,4
 	S=input(“Enter:”)
 	Len(a): Gives item count in a
 	min(a): Gives minimum value in a
 	max(a): Gives minimum value in a
 	sum(a): Adds up items of an iterable and returns sum
 	sorted(a): Sorted list copy of a
 	importing modules:  import random
```

#### File Operations:

In python, we have several functions for creating, reading, updating,  and deleting files. Theopen() function takes two parameters – filename,  and mode.
 There are four different methods (modes) for opening a file:

```php
 	"r" - Read - Default value. Opens a file for reading, error if the file does not exist
 	"a" - Append - Opens a file for appending, creates the file if it does not exist
 	"w" - Write - Opens a file for writing, creates the file if it does not exist
 	"x" - Create - Creates the specified file, returns an error if the file exists

f= open(“File Name”,“opening mode”)
```

(Opening modes: r: read, w: write, a: append, r+: both read and write)

#### **Try & Except Block:**

The try block allow us to test a block of code for errors.The except block allow us to handle the error.

```php
try:
[Statement body block]
raise Exception()
except Exception as e:
[Error processing block]
```

#### Oops Concepts

Python is an object-oriented programming language. In Python, almost  everything is an object and has its own properties and methods. Here a  class is like an object constructor, or a “blueprint” for creating  objects.

```php
 	Inheritance: A process of using details from a new class without modifying existing class.
 	Polymorphism: A concept of using common operation in different ways for different data input.
 	Encapsulation: Hiding the private details of a class from other objects.
```

#### Class/object Example:

```php
Class: class Pen:
pass
object:obj=Pen()
```

# Data Science

Data Science Combines Fields of Statistics and Computer Science.

Common Subdomains and applications of Data Science are ML/AI, Data Mining, Data Warehousing, Big Data etc.

![1559744564514](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559744564514.png)

## Data Science Tasks

![1559744604018](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559744604018.png)

## Data Preprocessing

1. **Feature Selection:** Select relevant features removing unwanted features.
2. **Row Compression:** Rows with similar features can be aggregated.
3. **One-Hot Encoding:**  Each Categorical variable is converted to a feature. Each feature contains 0 or 1
4. **Binning(Discretization):** Numerical data is converted into categorical data.
5. **Missing Values:** Try filling with mode or median. If the data set is large enough, remove the row.
6. **Sampling:** Selecting a subset of data
7. **Dimensionality Reduction:** Reducing features using PCA, SVD or other algorithms
8. **Cross Validation:** Cross-validation is a resampling procedure used to evaluate machine learning models on a limited data sample.
9. **K-fold Cross Validation:** Divide data into k buckets and pick each bucket for testing and rest of the buckets for training.
10. **Normalization:** Scaling value to a range.

## Data Visualization

It is the creation and study of the visual representation of data.

### Bar Charts

Used in comparison of values for categorical variables

The bars can be plotted vertically or horizontally.

![Image result for bar chart](https://plot.ly/~RPlotBot/3512/count-vs-animals.png)

### Pie Chart

A pie chart (or a circle chart) is a circular statistical graphic, which is divided into slices to illustrate numerical proportion. In a pie chart, the arc length of each slice (and consequently its central angle and area), is proportional to the quantity it represents.

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/English_dialects1997.svg/800px-English_dialects1997.svg.png)



### Scatter Plot

It is a type of plot or mathematical diagram using Cartesian coordinates to display values for typically two variables for a set of data. If the points are coded (color/shape/size(Bubble Plots)), one additional variable can be displayed.

![Scatter diagram for quality characteristic XXX.svg](https://upload.wikimedia.org/wikipedia/commons/thumb/a/af/Scatter_diagram_for_quality_characteristic_XXX.svg/800px-Scatter_diagram_for_quality_characteristic_XXX.svg.png)

##### Bubble Plot:

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/8/86/Net_Present_Value_vs_Payback_time_Portfolio_Management_Simulation.jpg/1024px-Net_Present_Value_vs_Payback_time_Portfolio_Management_Simulation.jpg)

### Line Plot

A line chart or line plot or line graph is a type of chart which displays information as a series of data points called 'markers' connected by straight line segments.

It is generally used for continuous variables, generally changing over time.

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/0/02/ScientificGraphSpeedVsTime.svg/800px-ScientificGraphSpeedVsTime.svg.png)

### Box Plot

A box plot or boxplot is a method for graphically depicting groups of numerical data through their quartiles. Box plots may also have lines extending vertically from the boxes (whiskers) indicating variability outside the upper and lower quartiles, hence the terms box-and-whisker plot and box-and-whisker diagram. Outliers may be plotted as individual points. The upper and lower dashes represent maximum and minimum values, the mid-line represents median.

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/Michelsonmorley-boxplot.svg/800px-Michelsonmorley-boxplot.svg.png)

### Histograms

A histogram is an accurate representation of the distribution of numerical data. It is an estimate of the probability distribution of a continuous variable.

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Black_cherry_tree_histogram.svg/800px-Black_cherry_tree_histogram.svg.png)

**A Line Histogram:**

![img](https://i.stack.imgur.com/S6hqi.png)



# Introduction to Machine Learning

Machine learning (ML) is the scientific study of algorithms and statistical models that computer systems use in order to perform a specific task effectively without using explicit instructions, relying on patterns and inference instead. It is seen as a subset of artificial intelligence.

Machine learning algorithms are used in a wide variety of applications, such as email filtering, and computer vision, where it is infeasible to develop an algorithm of specific instructions for performing the task. Machine learning is closely related to computational statistics, which focuses on making predictions using computers.

* Supervised learning algorithms build a mathematical model of a set of data that contains both the inputs and the desired outputs.The data is known as training data, and consists of a set of training examples. Each training example has one or more inputs and a desired output. Supervised Learning tasks include Classification and Regression.
*  In the case of semi-supervised learning algorithms, some of the training examples are missing the desired output.
* Unsupervised learning algorithms take a set of data that contains only inputs, and find structure in the data, like grouping or clustering of data points. The algorithms therefore learn from test data that has not been labeled, classified or categorized. Instead of responding to 
  feedback, unsupervised learning algorithms identify commonalities in the data and react based on the presence or absence of such commonalities in each new piece of data.
* Reinforcement learning is an area of machine learning concerned with how software agents ought to take actions in an environment so as to maximize some notion of cumulative reward. Due to its generality, the field is studied in many other disciplines, such as game theory, control theory, operations research, information theory, simulation-based optimization, multi-agent systems, swarm intelligence, statistics and genetic algorithms.

![1559744974117](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559744974117.png)

![1559744988538](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559744988538.png)

### Anaconda

Anaconda is a free and open-source distribution of the Python and R programming languages for scientific computing, that aims to simplify package management and deployment. Package versions are managed by the package management system conda.

It has many useful libraries such as numpy, pandas, scikit-learn,seaborn,matplotlib etc.

It has Jupyter Notebook, Spyder, R Studio and other IDEs



## Algorithms

## Supervised - Regression

Regression is a supervised learning method used to predict continuous variables.

1. ### Linear Regression

   1. Derived from statistics, Linear regression fits a straight line which is as near to all data points as possible. 

   2. It is sensitive to outliers.

   3. It can be univariate or multivariate

   4. ![img](https://cdn-images-1.medium.com/max/800/0*szXvH1a4ZQytyqhg.png)

   5. Mathematical Background:

      Linear regression involves fitting a line of equation y=b+mx

      This can be written as

   $$
   h_\theta=\theta_0+\theta_1x
   $$

   ​	The cost function is given by:
   $$
   J(\theta_0,\theta_1)=\frac{1}{2}\sum_{i=0}^m (h_\theta(x^{(i)})-y^{(i)})^2
   $$
   ​	We can minimize the squared error using optimization techniques such as gradient descent 	to get the best fit.

   ​	For Multivariate data, the equation can be written as
   $$
   h_\theta=\theta_0+\theta_1x_1+\theta_2x_2+\theta_3x_3+...+\theta_nx_n
   $$

2. ### Logistic Regression

   1. Logistic Regression uses a logistic function to model a binary dependent variable

   2.  In regression analysis, logistic regression (or logit regression) is estimating the parameters of a logistic model

   3. Unlike other type of regression models, logistic regression is used for binary classification

   4. It uses a sigmoid function which generates an S shaped curve which generates values between 0 and 1

   5. Generally, 0.5 is the cutoff for labelling the classes

   6. ![img](https://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Logistic-curve.svg/1024px-Logistic-curve.svg.png)

   7. Mathematical Background:

      The model can be denoted as:
      $$
      h_\theta=\frac{1}{1+e^{-\theta^TX}}
      $$
      The model can also be denoted in terms of probability
      $$
      h_\theta=P(y=0|x;\theta)
      $$
      

3. ### Ridge Regression

   We add a level-2 regularization (keeps the weights small making the model simpler and avoiding overfitting.) parameter to our linear regression model.
   $$
   J(\theta_0,\theta_1)=\frac{1}{2}[\sum_{i=0}^m (h_\theta(x^{(i)})-y^{(i)})^2+\lambda\sum_{j=0}^n\theta^2]
   $$

4. ### LASSO Regression

   We add a level-1 regularization to our linear regression model
   $$
   J(\theta_0,\theta_1)=\frac{1}{2}[\sum_{i=0}^m (h_\theta(x^{(i)})-y^{(i)})^2+\lambda\sum_{j=0}^n|\theta|]
   $$

5. ### Multivariate Adaptive Regression Splines

   Multivariate adaptive regression splines (MARS) is a form of  regression analysis introduced by Jerome H. Friedman in 1991.It is a  non-parametric regression technique and can be seen as an extension of  linear models that automatically models nonlinearities and interactions  between variables.

   Multivariate adaptive regression splines, implemented by the Earth  class, is a flexible regression method that automatically searches for  interactions and non-linear relationships. Earth models can be thought  of as linear models in a higher dimensional basis space. Each term in an  Earth model is a product of so called “hinge functions”. A hinge  function is a function that’s equal to its argument where that argument  is greater than zero and is zero everywhere else. 

   ![alt text](https://contrib.scikit-learn.org/py-earth/_images/hinge.png)

6. ### Non Linear Regression

   Nonlinear regression is a form of regression analysis in which observational data are modeled by a function which is a nonlinear combination of the model parameters and depends on one or more independent variables.

   ![Image result for nonlinear regression](https://blog.minitab.com/hubfs/Imported_Blog_Media/fittedlp_bmi-1.gif)

   Mathematical Background: 

   A Quadratic regression can be represented as:
   $$
   h_\theta=\theta_0+\theta_1x+\theta_2x^2
   $$
   

   A Polynomial regression can be represented as:
   $$
   h_\theta=\theta_0+\theta_1x+\theta_2x^2+\theta_3x^3+...+\theta_nx^n
   $$
   

## Supervised - Classification

 Classification is a supervised learning method used to predict categorical variables.

1. ### K-Nearest Neighbors

   1. KNN is an instance based learning algorithm. The algorithm predicts the class which has maximum occurrences in the test record's K-Nearest Neighbors

   2. It is a lazy learner i.e, all computation is deferred until classification.

   3. A peculiarity of the *k*-NN algorithm is that it is sensitive to the local structure of the data.

   4. We compute the distance from test record to each training record. We can use many distance metric including Euclidian distance as shown 
      $$
      d(\mathbf{q},\mathbf{p}) =  \sqrt{\sum_{i=1}^n (q_i-p_i)^2}
      $$

   5. Then we choose K-nearest neighbors which have minimum distance.

   6. A Class label is assigned to the test record by majority voting.
      $$
      y'=\mathbf{argmax}\: \sum_{ (xi,yi) ∈ Dz} I(v=yi)
      $$
      Where (x,y) is a training record, I is the induction function to get class label

      ![1559750832898](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559750832898.png)

      

2. ### Decision Trees

   1. Decision trees use a tree based approach to classify. The leaf nodes of a tree are class labels needed to be predicted and the internal nodes are decision parameters (Attribute Value Pairs).
   2. **Decision tree learning** is the construction of a decision tree  from class-labeled training tuples. A decision tree is a flow-chart-like structure, where each internal (non-leaf) node denotes a test on an attribute, each branch represents the outcome of a test, and each leaf 
      (or terminal) node holds a class label. The topmost node in a tree is the root node.
   3. ![1559751582878](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559751582878.png)
   4. Information gain is used to decide which feature to split on at each step in building the tree.To do so, at each step we should choose the split that results in the purest daughter nodes.The information value "represents the expected amount of information that would be needed to specify whether a new instance should be classified yes or no, given that the example reached that node".
   5. Lots of algorithms can be used to build decision trees like CART, C4.5,ID3 etc.
   6. They tend to overfit to training data set.

3. ### Random Forest and Bagging

   1. Random forests or random decision forests are an ensemble learning method for classification, regression and other tasks that operates by constructing a multitude of decision trees at training time and outputting the class that is the mode of the classes (classification) or mean prediction (regression) of the individual trees.

   2. The training algorithm for random forests applies the general technique of bootstrap aggregating, or bagging, to tree learners. Given a training set ***X = x1, ..., xn*** with responses **Y = y1, ..., yn**, bagging repeatedly (B times) selects a random sample with replacement of the training set and fits trees to these samples

   3. Random forests differ in only one way from this general scheme: they use a modified tree learning algorithm that selects, at each candidate split in the learning process, a random subset of the features. This process is sometimes called "feature bagging". 

4. ### Boosting

   1. Boosting algorithms are a family of machine learning algorithms that convert weak learners to strong ones.

   2. ```
      Step 1:  The base learner takes all the distributions and assign equal weight or attention to each observation.
      
      Step 2: If there is any prediction error caused by first base learning algorithm, then we pay higher attention to observations having prediction error. Then, we apply the next base learning algorithm.
      
      Step 3: Iterate Step 2 till the limit of base learning algorithm is reached or higher accuracy is achieved.
      ```

      

   3. **AdaBoost(Adaptive Boosting):** It fits a sequence of weak learners on different weighted training data.It starts by predicting original data set and gives equal weight to each observation. If prediction is incorrect using the first learner, then it gives higher weight to observation which have been predicted incorrectly. Being an iterative process, it continues to add learner(s) until a limit is reached in the number of models or accuracy.

   4. **Gradient Boosting:** In gradient boosting, it trains many  model sequentially. Each new model gradually minimizes the loss function  (y = ax + b + e, e needs special attention as it is an error term) of  the whole system using Gradient Descent method. The learning procedure consecutively fit new models to provide a more accurate estimate of the response variable.

      The principle idea behind this algorithm  is to construct new base learners which can be maximally correlated  with negative gradient of the loss function, associated with the whole  ensemble.

   5. **XGBoost:** XGBoost is a popular implementation of gradient boosting. XGBoost stands for e**X**treme **G**radient **B**oosting.It adds regularization to gradient boosting. Three main forms of gradient boosting are supported

      1. **Gradient Boosting** algorithm also called gradient boosting machine including the learning rate.
      2. **Stochastic Gradient Boosting** with sub-sampling at the row, column and column per split levels.
      3. **Regularized Gradient Boosting** with both L1 and L2 regularization.

      It uses Scikit-learn like syntax.

      ```python
      import xgboost as xgb
      model=xgb.XGBClassifier(random_state=1,learning_rate=0.01)
      model.fit(x_train, y_train)
      model.score(x_test,y_test)
      0.82702702702702702
      ```

      

5. ### Naïve Bayes

   1. Naïve Bayes uses Bayes Theorem to classify. It assumes that the features are conditionally independent of each other.

   2. The naïve Bayes classifier combines this model with a decision rule. One common rule is to pick the hypothesis that is most probable; this is known as the maximum a posteriori or MAP decision rule. The corresponding classifier, a Bayes classifier, is the function that assigns a class label  ![{\hat  {y}}=C_{k}](https://wikimedia.org/api/rest_v1/media/math/render/svg/6fe719eda4ce62ee2f2104455abc5233fdf69e01) for some k as
      $$
      \hat{y} = \underset{k \in \{1, \dots, K\}}{\operatorname{argmax}} \ p(C_k) \displaystyle\prod_{i=1}^n p(x_i \mid C_k).
      $$

   3. A class's prior may be calculated by assuming equiprobable classes (i.e., priors = 1 / (number of classes)), or by calculating an estimate for the class probability from the training set (i.e., (prior for a given class) = (number of samples in the class) / (total number of samples)). To estimate the parameters for a feature's distribution, one must assume a distribution or generate nonparametric models for the features from the training set.

   4. Any probability distribution such as Gaussian, Multinomial or Bernoulli's distribution.

6. ### Support Vector Machines

   1. Support Vector Machine classifies by drawing a hyperplane (line) that separates two classes.  

   2. Support vectors are the data points that lie closest to the hyperplane.

   3. SVMs maximize the margin between hyperplane and support vectors.

   4. ![Image result for support vector machine](https://cdn-images-1.medium.com/max/1200/1*QJZVKh-YHhPn5Q83kzJ96Q.png)

   5. Any hyperplane can be written as the set of points **x** satisfying **w**⋅**x**+*b*=0 . or:

   6. $$
      w^Tx=0
      $$

   7. For **linear kernel**  the equation for prediction for a new input using the dot product  between the input (x) and each support vector (xi) is calculated as  follows:
      $$
      f(x) = B(0) + \sum(ai * (x,xi))
      $$
      This is an equation that involves calculating the inner products of a new input vector (x) with all support vectors in training data. The coefficients B0 and ai (for each input) must be estimated from the training data by the learning algorithm.

   8. The **polynomial kernel** can be written as
      $$
      K(x,xi) = 1 + \sum(x\times xi)^d
      $$
      and **exponential** as 
      $$
      K(x,xi) = exp(-gamma * \sum((x — x_i²))
      $$

   9. Polynomial and exponential kernels calculates separation line in higher dimension. This is called **kernel trick**

      ![Image result for non linear kernels in svm](https://www.researchgate.net/profile/Catarina_Moreira2/publication/260283043/figure/fig13/AS:297261608259591@1447884098165/Figure-A15-The-non-linear-SVM-classifier-with-the-kernel-trick.png)

      ![Image result for non linear kernels in svm](https://kgpdag.files.wordpress.com/2015/08/11850866_1042104839148149_308987681_n.jpg)

   10. The gamma parameter defines how far the influence of a single training example reaches, with low values meaning ‘far’ and high values meaning ‘close’. 

7. ### Linear Discriminant Analysis

   1. LDA models the distribution of predictors separately in each of the response classes, and then it uses Bayes’ theorem to estimate the probability.

   2. Find the linear combination 
      $$
      Z=a^T\times X
      $$
       such that the between class variance is maximized

   3. It calculates probability using Bayes Theorem

   $$
   P(y=k | X) = \frac{P(X | y=k) P(y=k)}{P(X)}
   $$

   4. It can also be used for Dimensionality Reduction as Score Z captures variance of multiple features.
   5. ![Image result for linear discriminant analysis](https://slideplayer.com/slide/4557543/15/images/3/Linear+Discriminant+Analysis+%28LDA%29.jpg)
   6. ![Related image](https://sebastianraschka.com/images/blog/2014/linear-discriminant-analysis/lda_pca_recap.png)

8. ### Rule Based Classifiers 

   1. Rule Based Classifiers use if-then rules to classify.

   2. A rule can be of the form:

   3. $$
      \mathbf R_i:x\rightarrow y 
      $$

   4. Where x is the rule precondition of the form:

   $$
   (A\and B\and C...)
   $$

   5. y is the class label
   6. Rules can be generated directly from the dataset or indirectly from decision trees.

## Unsupervised - Clustering

1. ### K-Means

   1. K-Means forms spherical clusters using partition based clustering.
   2. K denotes number of clusters.
   3. We choose K random points as centroids and assign each point to nearest centroid
   4. We now find the mean of each cluster and choose the nearest point to the mean as new centroid. We then repeat the process until mean doesn't change.
   5. ![Image result for K Means](https://d2908q01vomqb2.cloudfront.net/f1f836cb4ea6efb2a0b1b99f41ad8b103eff4b59/2018/11/02/k-means-sagemaker-1.gif)

2. ### Agglomerative Hierarchical Clustering

   1. Agglomerative Clustering uses bottom up approach to produce hierarchical nested clusters.
   2. We assign each data point as a cluster.
   3. We combine two nearest points to form a cluster
   4. We combine two nearest cluster to form higher level cluster
   5. We repeat it until a single cluster is formed
   6. ![Image result for agglomerative clustering](https://www.datanovia.com/en/wp-content/uploads/dn-tutorials/003-hierarchical-clustering-in-r/figures/002-agglomerative-clustering-cutree-cut-dendrogram-1.png)

   

3. ### DBSCAN

   1. It stands for **Density-based spatial clustering of applications with noise**

   2.  Given a set of points in some space, it groups together points that are closely packed together (points with many nearby neighbors), marking as outliers points that lie alone in low-density regions (whose nearest neighbors are too far away).

   3. A point *p* is a *core point* if at least minPts points are within distance *ε* of it (including *p*).

   4. A point *q* is *directly reachable* from *p* if point *q* is within distance *ε* from core point *p*. Points are only said to be directly reachable from core points.

   5. A point *q* is *reachable* from *p* if there is a path *p*1, ..., *pn* with *p*1 = *p* and *pn* = *q*, where each *pi*+1 is directly reachable from *pi*. Note that this implies that all points on the path must be core points, with the possible exception of *q*.

   6. All points not reachable from any other point are *outliers* or *noise points*.

   7. ```
      The DBSCAN algorithm can be abstracted into the following steps:
      
          Find the points in the ε (eps) neighborhood of every point, and identify the core points with more than minPts neighbors.
          Find the connected components of core points on the neighbor graph, ignoring all non-core points.
          Assign each non-core point to a nearby cluster if the cluster is an ε (eps) neighbor, otherwise assign it to noise.
      ```

   8. ![img](https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/DBSCAN-density-data.svg/800px-DBSCAN-density-data.svg.png)

   9. DBSCAN can form clusters in irregular shapes

4. ### EM Clustering

   1. Expectation–maximization (EM) algorithm is an iterative method to find maximum likelihood or maximum a posteriori (MAP) estimates of parameters here the model depends on unobserved latent variables. It is an optimization algorithm used to cluster using Gaussian Mixture Models
   2. The EM iteration alternates between performing an expectation (E) step, which creates a function for the expectation of the log-likelihood evaluated using the current estimate for the parameters, and a maximization (M) step, which computes parameters maximizing the expected log-likelihood found on the E step.
   3. EM is frequently used for data clustering in machine learning and computer vision.
   4. Gaussian mixture models are a probabilistic model for representing normally distributed subpopulations within an overall population.
   5. We have two parameters to describe the shape of the clusters: the mean and the standard deviation, so clusters can take elliptical shape
   6. We begin by selecting the number of clusters (like K-Means does) and randomly initializing the Gaussian distribution parameters for each cluster.
   7. Given these Gaussian distributions for each cluster, compute the probability that each data point belongs to a particular cluster. The closer a point is to the Gaussian’s center, the more likely it belongs to that cluster. 
   8. Based on these probabilities, we compute a new set of parameters for the Gaussian distributions such that we maximize the probabilities of data points within the clusters. We compute these new parameters using a weighted sum of the data point positions, where the weights are the probabilities of the data point belonging in that particular cluster.
   9. Repeat the algorithm until convergence.![img](https://cdn-images-1.medium.com/max/800/1*OyXgise21a23D5JCss8Tlg.gif)

## Unsupervised - Dimensionality Reduction

1. ### Principle Component Analysis

   1. PCA is one of the most widely used dimensionality reduction methods
   2. It assumes all features as a matrix.
   3. The features are scaled to get uniform values.
   4. We compute covariance matrix from the scaled features
   5. We then find eigenvalues and eigenvectors for the covariance matrix
   6. The eigenvalue is sorted in descending order
   7. The highest eigenvalue captures the features with most variance
   8. The eigenvector corresponding to the eigenvalue points to the direction in which variance is maximum.

2. ### Singular Value Decomposition

   1. Matrix decomposition, also known as matrix factorization, involves describing a given matrix using its constituent elements.

   2. We have 
      $$
      A = U . \Sigma . V^T
      $$
      Where A is the real m x n matrix that we wish to decompose, U is an m x m matrix, Sigma is an m x n diagonal matrix, and V^T is the  transpose of an n x n matrix where T is a superscript.

      The diagonal values in the Sigma matrix are known as the singular values of the original matrix A. The columns of the U matrix are called the left-singular vectors of A, and the columns of V are called the right-singular vectors of A

      Every rectangular matrix has a singular value decomposition, although the resulting matrices may contain complex numbers and the limitations of floating point arithmetic may cause some matrices to fail to decompose neatly.

   3. Data with a large number of features, such as more features (columns)than observations (rows) may be reduced to a smaller subset of features that are most relevant to the prediction problem.

   4. To do this we can perform an SVD operation on the original data and select the top k largest singular values in Sigma. These columns can be selected from Sigma and the rows selected from V<sup>T</sup>.

# Deep Learning

■Deep Learning makes use of Deep Neural Networks

■A Neural Network generally contains 3 types of layers: Input Layer, Hidden layer, Output Layer.

■A Deep Neural Network contains a large number of hidden layers

■Nodes are connect with Weights and Biases. Each node is activated if the activation function produces a value greater than the threshold value

![1559759062486](C:\Users\PareeKatti\AppData\Roaming\Typora\typora-user-images\1559759062486.png)

## Activation Functions [From ML Cheatsheets]

## Linear

A straight line function where activation is proportional to input ( which is the weighted sum from neuron ).

| Function               | Derivative |
| ---------------------- | ---------- |
| *R*(*z*,*m*)={*z*∗*m*} |            |

|      | *R*′(*z*,*m*)={*m*} |
| ---- | ------------------- |
|      |                     |

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [![_images/linear.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/linear.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/linear.png) | [![_images/linear_prime.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/linear_prime.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/linear_prime.png) |
|                                                              |                                                              |

Pros

- It gives a range of activations, so it is not binary activation.
- We can definitely connect a few neurons together and if more than 1  fires, we could take the max ( or softmax) and decide based on that.

Cons

- For this function, derivative is a constant. That means, the gradient has no relationship with X.
- It is a constant gradient and the descent is going to be on constant gradient.
- If there is an error in prediction, the changes made by back  propagation is constant and not depending on the change in input  delta(x) !



## ELU

Exponential Linear Unit or its widely known name ELU is a function  that tend to converge cost to zero faster and produce more accurate  results. Different to other activation functions, ELU has a extra alpha  constant which should be positive number.

ELU is very similiar to RELU except negative inputs. They are both in  identity function form for non-negative inputs. On the other hand, ELU  becomes smooth slowly until its output equal to -α whereas RELU sharply  smoothes.

| Function                                | Derivative |
| --------------------------------------- | ---------- |
| *R*(*z*)={*z**α*.(*e**z*–1)*z*>0*z*<=0} |            |

|      | *R*′(*z*)={1*α*.*e**z**z*>0*z*<0} |
| ---- | --------------------------------- |
|      |                                   |

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [![_images/elu.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/elu.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/elu.png) | [![_images/elu_prime.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/elu_prime.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/elu_prime.png) |
|                                                              |                                                              |

Pros

- ELU becomes smooth slowly until its output equal to -α whereas RELU sharply smoothes.
- ELU is a strong alternative to ReLU.
- Unlike to ReLU, ELU can produce negative outputs.

Cons

- For x > 0, it can blow up the activation with the output range of [0, inf].



## [ReLU](https://ml-cheatsheet.readthedocs.io/en/latest/activation_functions.html#id8)

A recent invention which stands for Rectified Linear Units. The formula is deceptively simple: *m**a**x*(0,*z*)

. Despite its name and appearance, it’s not linear and provides the same benefits as Sigmoid but with better performance.

| Function                   | Derivative |
| -------------------------- | ---------- |
| *R*(*z*)={*z*0*z*>0*z*<=0} |            |

|      | *R*′(*z*)={10*z*>0*z*<0} |
| ---- | ------------------------ |
|      |                          |

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [![_images/relu.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/relu.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/relu.png) | [![_images/relu_prime.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/relu_prime.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/relu_prime.png) |
|                                                              |                                                              |

Pros

- It avoids and rectifies vanishing gradient problem.
- ReLu is less computationally expensive than tanh and sigmoid because it involves simpler mathematical operations.

Cons

- One of its limitation is that it should only be used within Hidden layers of a Neural Network Model.
- Some gradients can be fragile during training and can die. It can  cause a weight update which will makes it never activate on any data  point again. Simply saying that ReLu could result in Dead Neurons.
- In another words, For activations in the region (x<0) of ReLu,  gradient will be 0 because of which the weights will not get adjusted  during descent. That means, those neurons which go into that state will  stop responding to variations in error/ input ( simply because gradient  is 0, nothing changes ). This is called dying ReLu problem.
- The range of ReLu is [0, inf). This means it can blow up the activation.

Further reading

- [Deep Sparse Rectifier Neural Networks](http://proceedings.mlr.press/v15/glorot11a/glorot11a.pdf) Glorot et al., (2011)
- [Yes You Should Understand Backprop](https://medium.com/@karpathy/yes-you-should-understand-backprop-e2f06eab496b), Karpathy (2016)



## [LeakyReLU](https://ml-cheatsheet.readthedocs.io/en/latest/activation_functions.html#id9)

LeakyRelu is a variant of ReLU. Instead of being 0 when *z*<0

, a leaky ReLU allows a small, non-zero, constant gradient 

*α*

 (Normally, α=0.01). However, the consistency of the benefit across tasks is presently unclear. [[1\]](https://ml-cheatsheet.readthedocs.io/en/latest/activation_functions.html#id5)

| Function                        | Derivative |
| ------------------------------- | ---------- |
| *R*(*z*)={*z**α**z**z*>0*z*<=0} |            |

|      | *R*′(*z*)={1*α**z*>0*z*<0} |
| ---- | -------------------------- |
|      |                            |

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [![_images/leakyrelu.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/leakyrelu.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/leakyrelu.png) | [![_images/leakyrelu_prime.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/leakyrelu_prime.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/leakyrelu_prime.png) |
|                                                              |                                                              |

Pros

- Leaky ReLUs are one attempt to fix the “dying ReLU” problem by having a small negative slope (of 0.01, or so).

Cons

- As it possess linearity, it can’t be used for the complex  Classification. It lags behind the Sigmoid and Tanh for some of the use  cases.

Further reading

- [Delving Deep into Rectifiers: Surpassing Human-Level Performance on ImageNet Classification](https://arxiv.org/pdf/1502.01852.pdf), Kaiming He et al. (2015)



## [Sigmoid](https://ml-cheatsheet.readthedocs.io/en/latest/activation_functions.html#id10)

Sigmoid takes a real value as input and outputs another value between  0 and 1. It’s easy to work with and has all the nice properties of  activation functions: it’s non-linear, continuously differentiable,  monotonic, and has a fixed output range.

| Function            | Derivative |
| ------------------- | ---------- |
| *S*(*z*)=11+*e*−*z* |            |

|      | *S*′(*z*)=*S*(*z*)⋅(1−*S*(*z*)) |
| ---- | ------------------------------- |
|      |                                 |

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [![_images/sigmoid.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/sigmoid.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/sigmoid.png) | [![_images/sigmoid_prime.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/sigmoid_prime.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/sigmoid_prime.png) |
|                                                              |                                                              |

Pros

- It is nonlinear in nature. Combinations of this function are also nonlinear!
- It will give an analog activation unlike step function.
- It has a smooth gradient too.
- It’s good for a classifier.
- The output of the activation function is always going to be in range  (0,1) compared to (-inf, inf) of linear function. So we have our  activations bound in a range. Nice, it won’t blow up the activations  then.

Cons

- Towards either end of the sigmoid function, the Y values tend to respond very less to changes in X.
- It gives rise to a problem of “vanishing gradients”.
- Its output isn’t zero centered. It makes the gradient updates go too  far in different directions. 0 < output < 1, and it makes  optimization harder.
- Sigmoids saturate and kill gradients.
- The network refuses to learn further or is drastically slow (  depending on use case and until gradient /computation gets hit by  floating point value limits ).

Further reading

- [Yes You Should Understand Backprop](https://medium.com/@karpathy/yes-you-should-understand-backprop-e2f06eab496b), Karpathy (2016)



## [Tanh](https://ml-cheatsheet.readthedocs.io/en/latest/activation_functions.html#id11)

Tanh squashes a real-valued number to the range [-1, 1]. It’s non-linear. But unlike Sigmoid, its output is zero-centered. Therefore, in practice the tanh non-linearity is always preferred to the sigmoid nonlinearity. [[1\]](https://ml-cheatsheet.readthedocs.io/en/latest/activation_functions.html#id5)

| Function                                       | Derivative |
| ---------------------------------------------- | ---------- |
| *t**a**n**h*(*z*)=*e**z*−*e*−*z**e**z*+*e*−*z* |            |

|      | *t**a**n**h*′(*z*)=1−*t**a**n**h*(*z*)2 |
| ---- | --------------------------------------- |
|      |                                         |

|                                                              |                                                              |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [![_images/tanh.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/tanh.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/tanh.png) | [![_images/tanh_prime.png](https://ml-cheatsheet.readthedocs.io/en/latest/_images/tanh_prime.png)](https://ml-cheatsheet.readthedocs.io/en/latest/_images/tanh_prime.png) |
|                                                              |                                                              |

Pros

- The gradient is stronger for tanh than sigmoid ( derivatives are steeper).

Cons

- Tanh also has the vanishing gradient problem.

## [Softmax](https://ml-cheatsheet.readthedocs.io/en/latest/activation_functions.html#id12)

Softmax function calculates the probabilities distribution of the  event over ‘n’ different events. In general way of saying, this function  will calculate the probabilities of each target class over all possible  target classes. Later the calculated probabilities will be helpful for  determining the target class for the given inputs.

## Perceptron

1. A Perceptron is the most simple neural network consisting of a single neuron.
2. the perceptron is an algorithm for learning a binary classifier called a threshold function: a function that maps its input x (a real-valued vector) to an output value f ( x )(a single binary value): 
3. ![{\displaystyle f(\mathbf {x} )={\begin{cases}1&{\text{if }}\ \mathbf {w} \cdot \mathbf {x} +b>0,\\0&{\text{otherwise}}\end{cases}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/c27b30e07934b4fc8f346ec6fafd5b077d0d4efc)
4. where![\mathbf {w} ](https://wikimedia.org/api/rest_v1/media/math/render/svg/20795664b5b048744a2fd88977851104cc5816f8) is a vector of real-valued weights
5. We can use it for multiclass classification using a majority voting
6. ![{\hat {y}}=\operatorname {argmax} _{y}f(x,y)\cdot w.](https://wikimedia.org/api/rest_v1/media/math/render/svg/dc5b83e57ad0de11c737317732783fcf03b8cf1b)
7. ![Image result for perceptron](https://cdn-images-1.medium.com/max/1600/1*_Zy1C83cnmYUdETCeQrOgA.png)

## Feed Forward Neural Networks

A feedforward neural network is an artificial neural network wherein connections between the nodes do not form a cycle.

A Multi Layer Perceptron is an example for feed forward networks.

A multilayer perceptron (MLP) is a class of feedforward artificial neural network. A MLP consists of at least three layers of nodes: an input layer, a hidden layer and an output layer. Except for the input nodes, each node is a neuron that uses a nonlinear activation function. MLP utilizes a supervised learning technique called backpropagation for training.

Multilayer perceptrons are sometimes colloquially referred to as "vanilla" neural networks, especially when they have a single hidden layer.

![Image result for multilayer perceptron](https://cdn-images-1.medium.com/max/1600/1*q_o8pu8aPRGKo2Bq5KvzCQ.png)



## Convolutional Neural Networks

A convolutional neural network (CNN, or ConvNet) is a class of deep neural networks, most commonly applied to analyzing visual imagery. 

CNNs are regularized versions of multilayer perceptrons.

![Image result for convolutional neural network](https://cdn-images-1.medium.com/max/1600/1*uAeANQIOQPqWZnnuH-VEyw.jpeg)

A convolutional neural network consists of an input and an output layer, as well as multiple hidden layers. The hidden layers of a CNN typically consist of convolutional layers, RELU layer i.e. activation function, pooling layers, fully connected layers and normalization layers.

When programming a convolutional layer, each convolutional layer within a neural network should have the following attributes: 

- Input is a tensor with shape (number of images) x (image width) x (image height) x (image depth).
- Number of convolutional kernels. 
  - Width and height of kernels are hyper-parameters.
  - Depth of kernels must be equal to the image depth. Convolutional  layers apply a convolution operation to the input, passing the result to  the next layer. The convolution emulates the response of an individual  neuron to visual stimuli

Convolutional networks may include local or global pooling layers. Pooling layers reduce the dimensions of the data by combining the outputs of neuron clusters at one layer into a single neuron in the next layer. Local pooling combines small clusters, typically 2 x 2.  Global 
pooling acts on all the neurons of the convolutional layer.

Fully connected layers connect every neuron in one layer to every neuron in another layer. It is in principle the same as the traditional multi-layer perceptron neural network (MLP). The flattened matrix goes through a fully connected layer to classify the images. 

Finally, A Softmax Layer is used to predict a class.

## Recurrent Neural Networks

Recurrent Neural Network(RNN) are a type of Neural Network where the output from previous step are fed as input to the current step.

They are used extensively in NLP and Time Series Forecasting.

Recurring n times has same complexity has having n layers.

In a RNN, the information cycles through a loop. When it makes a decision, it takes into consideration the current input and also what it has learned from the inputs it received previously.

A usual RNN has a short-term memory. 

![Image result for RNN](https://cdn-images-1.medium.com/max/2600/0*c1L9jjcsASagk_Hu.png)





**Recurrent Neural Networks add the immediate past to the present.**

Therefore a Recurrent Neural Network has two inputs, the present and the recent past.

RNN’s apply weights to the current and also to the previous input. Furthermore they also tweak their weights for both through gradient descent and Backpropagation Through Time.

There are two major obstacles RNN’s have or had to deal with. 

#### Exploding Gradients

the algorithm assigns a stupidly high importance to the weights, without much reason. But fortunately, this problem can be easily solved if you truncate or squash the gradients.

#### Vanishing Gradients

When the values of a gradient are too small and the model stops learning or takes way too long because of that.

### LSTM

Long Short-Term Memory (LSTM) networks are an extension for recurrent neural networks, which basically extends their memory. It solves vanishing gradient problem. The units of an LSTM are used as building units for the layers of a RNN, which is then often called an LSTM network.

LSTM’s enable RNN’s to remember their inputs over a long period of time. This is because LSTM’s contain their information in a memory, that is much like the memory of a computer because the LSTM can read, write and delete information from its memory.

This memory can be seen as a gated cell, where gated means that the cell decides whether or not to store or delete information. based on the importance it assigns to the information. The assigning of 
importance happens through weights, which are also learned by the algorithm. This simply means that it learns over time which information is important and which not.

In an LSTM you have three gates: input, forget and output gate. These gates determine whether or not to let new input in (input gate), delete the information because it isn’t important (forget gate) or to let it impact the output at the current time step (output gate).

![img](https://cdn-images-1.medium.com/max/1254/0*YEVLdwY6verYMBEa.png)

The problematic issues of vanishing gradients is solved through LSTM because it keeps the gradients steep enough and therefore the training relatively short and the accuracy high.

## Restricted Boltzmann Machine

It is a two layer shallow neural network where the second layer tries to reconstruct te input and adjusts weights and biases along the way. It is a generative model.

No two nodes in the same layer share a connection.

This was designed to solve Vanishing Gradient Problem in Backpropogation.

![img](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Restricted_Boltzmann_machine.svg/800px-Restricted_Boltzmann_machine.svg.png)

It is useful for dimensionality reduction, classification, regression, collaborative filtering, feature learning and topic modeling.

 

## Deep Belief Networks

A deep-belief network can be defined as a stack of restricted Boltzmann machines, in which each RBM layer communicates with both the previous and subsequent layers. The nodes of any single layer don’t communicate with each other laterally.

This stack of RBMs might end with a a Softmax layer to create a classifier, or it may simply help cluster unlabeled data in an unsupervised learning scenario.

![Image result for deep belief networks](https://cdn-images-1.medium.com/max/1600/1*35ThREiCBzVIjGByNmI9hA.png)

With the exception of the first and final layers, each layer in a deep-belief network has a double role: it serves as the hidden layer to the nodes that come before it, and as the input (or “visible”) layer to the nodes that come after. It is a network built of single-layer networks.

Deep-belief networks are used to recognize, cluster and generate images, video sequences and motion-capture data. A continuous deep-belief network is simply an extension of a deep-belief network that accepts a continuum of decimals, rather than binary data. 

## Autoencoders

An autoencoder is a type of artificial neural network used to learn efficient data codings in an unsupervised manner.

Autoencoders are generally shallow.

 The aim of an autoencoder is to learn a representation (encoding) for a set of data, typically for dimensionality reduction, by training the network to ignore signal “noise”. Along with the reduction side, a reconstructing side is learnt, where the autoencoder tries to generate from the reduced encoding a representation as close as possible to its original input, hence its name. Recently, the autoencoder concept has become more widely used for learning generative models of data.

![img](https://upload.wikimedia.org/wikipedia/commons/2/28/Autoencoder_structure.png)

Z in the above diagram is called a bottleneck.

An autoencoder learns to compress data from the input layer into a short code, and then uncompress that code into something that closely matches the original data. This forces the autoencoder to engage in dimensionality reduction, for example by learning how to ignore noise. 
Some architectures use stacked sparse autoencoder layers for image recognition.

Various techniques exist to prevent autoencoders from learning the identity function and to improve their ability to capture important information and learn richer representations:

Denoising autoencoders take a partially corrupted input whilst training to recover the original undistorted input.

Contractive autoencoder adds an explicit regularizer in their objective function that forces the model to learn a function that is robust to slight variations of input values.

## Transformers

 A recently introduced model (By Google) which is explicitly good at NLP tasks.

 Sequence-to-Sequence (or Seq2Seq) is a neural net that transforms a given sequence of elements, such as the sequence of words in a sentence,into another sequence.

Seq2Seq models are particularly good at translation, where the sequence of words from one language is transformed into a sequence of different words in another language. A popular choice for this type of model is Long-Short-Term-Memory (LSTM)-based models. 

Seq2Seq models consist of an Encoder and a Decoder. The Encoder takes the input sequence and maps it into a higher dimensional space (n-dimensional vector). That abstract vector is fed into the Decoder which turns it into an output sequence. The output sequence can be in another language, symbols, a copy of the input, etc.

**Attention:** The attention-mechanism looks at an input sequence and decides at each step which other parts of the sequence are important.

for each input that the LSTM (Encoder) reads, the attention-mechanism takes into account several other inputs at the same time and decides which ones are important by attributing different weights to those inputs. The Decoder will then take as input the encoded sentence and the weights provided by the attention-mechanism.

Transformer is an architecture for transforming one sequence into another one with the help of two parts (Encoder and Decoder), but it differs from the previously described/existing sequence-to-sequence models because it does not imply any Recurrent Networks .

![img](https://cdn-images-1.medium.com/max/800/1*BHzGVskWGS_3jEcYYi6miQ.png)

The Encoder is on the left and the Decoder is on the right. Both Encoder and Decoder are composed of modules that can be stacked on top of each other multiple times, which is described by *Nx* in the figure.

We see that the modules consist mainly of Multi-Head Attention and Feed Forward layers. The inputs and outputs (target sentences) are first embedded into an n-dimensional space since we cannot use strings directly.

One slight but important part of the model is the positional encoding of the different words. Since we have no recurrent networks that can remember how sequences are fed into a model, we need to somehow give every word/part in our sequence a relative position since a sequence depends on the order of its elements. These positions are added to the embedded representation (n-dimensional vector) of each word.

## Generative Adversarial Networks

Generative adversarial networks (GANs) are deep neural net architectures comprised of two nets, pitting one against the other (thus the “adversarial”).

GANs’ potential is huge, because they can learn to mimic any distribution of data. That is, GANs can be taught to create worlds eerily similar to our own in any domain: images, music, speech, prose.

To understand GANs, you should know how generative algorithms work, and for that, contrasting them with discriminative algorithms is instructive. Discriminative algorithms try to classify input data; that is, given the features of an instance of data, they predict a label or category to which that data belongs.

One neural network, called the *generator*, generates new data instances, while the other, the *discriminator*,evaluates them for authenticity; i.e. the discriminator decides whether
each instance of data that it reviews belongs to the actual training dataset or not.

![GAN schema](https://skymind.ai/images/wiki/gan_schema.png)

![GANs](https://skymind.ai/images/wiki/GANs.png)



# Python Packages

## NumPy

NumPy is a python array and matrix processing library. It allows for fast numerical computations.

A numpy array is a grid of values, all of the same type, and is indexed by a tuple of nonnegative integers. The number of dimensions is the *rank* of the array; the *shape*of an array is a tuple of integers giving the size of the array along each dimension.

```python
import numpy as np

a = np.array([1, 2, 3])   # Create a rank 1 array
print(type(a))            # Prints "<class 'numpy.ndarray'>"
print(a.shape)            # Prints "(3,)"
print(a[0], a[1], a[2])   # Prints "1 2 3"
a[0] = 5                  # Change an element of the array
print(a)                  # Prints "[5, 2, 3]"

b = np.array([[1,2,3],[4,5,6]])    # Create a rank 2 array
print(b.shape)                     # Prints "(2, 3)"
print(b[0, 0], b[0, 1], b[1, 0])   # Prints "1 2 4"

```

```python
import numpy as np

a = np.zeros((2,2))   # Create an array of all zeros
print(a)              # Prints "[[ 0.  0.]
                      #          [ 0.  0.]]"

b = np.ones((1,2))    # Create an array of all ones
print(b)              # Prints "[[ 1.  1.]]"

c = np.full((2,2), 7)  # Create a constant array
print(c)               # Prints "[[ 7.  7.]
                       #          [ 7.  7.]]"

d = np.eye(2)         # Create a 2x2 identity matrix
print(d)              # Prints "[[ 1.  0.]
                      #          [ 0.  1.]]"

e = np.random.random((2,2))  # Create an array filled with random values
print(e)                     # Might print "[[ 0.91940167  0.08143941]
                             #               [ 0.68744134  0.87236687]]"

```

#### Array indexing

Numpy offers several ways to index into arrays.

**Slicing:** Similar to Python lists, numpy arrays can be sliced. Since arrays may be multidimensional, you must specify a slice for each dimension of the array:

```python
import numpy as np

# Create the following rank 2 array with shape (3, 4)
# [[ 1  2  3  4]
#  [ 5  6  7  8]
#  [ 9 10 11 12]]
a = np.array([[1,2,3,4], [5,6,7,8], [9,10,11,12]])

# Use slicing to pull out the subarray consisting of the first 2 rows
# and columns 1 and 2; b is the following array of shape (2, 2):
# [[2 3]
#  [6 7]]
b = a[:2, 1:3]

# A slice of an array is a view into the same data, so modifying it
# will modify the original array.
print(a[0, 1])   # Prints "2"
b[0, 0] = 77     # b[0, 0] is the same piece of data as a[0, 1]
print(a[0, 1])   # Prints "77"

```

#### Boolean Indexing

```python
import numpy as np

a = np.array([[1,2], [3, 4], [5, 6]])

bool_idx = (a > 2)   # Find the elements of a that are bigger than 2;
                     # this returns a numpy array of Booleans of the same
                     # shape as a, where each slot of bool_idx tells
                     # whether that element of a is > 2.

print(bool_idx)      # Prints "[[False False]
                     #          [ True  True]
                     #          [ True  True]]"

# We use boolean array indexing to construct a rank 1 array
# consisting of the elements of a corresponding to the True values
# of bool_idx
print(a[bool_idx])  # Prints "[3 4 5 6]"

# We can do all of the above in a single concise statement:
print(a[a > 2])     # Prints "[3 4 5 6]"

```

```python
import numpy as np

x = np.array([1, 2])   # Let numpy choose the datatype
print(x.dtype)         # Prints "int64"

x = np.array([1.0, 2.0])   # Let numpy choose the datatype
print(x.dtype)             # Prints "float64"

x = np.array([1, 2], dtype=np.int64)   # Force a particular datatype
print(x.dtype)                         # Prints "int64"
```

```python
import numpy as np

x = np.array([[1,2],[3,4]], dtype=np.float64)
y = np.array([[5,6],[7,8]], dtype=np.float64)

# Elementwise sum; both produce the array
# [[ 6.0  8.0]
#  [10.0 12.0]]
print(x + y)
print(np.add(x, y))

# Elementwise difference; both produce the array
# [[-4.0 -4.0]
#  [-4.0 -4.0]]
print(x - y)
print(np.subtract(x, y))

# Elementwise product; both produce the array
# [[ 5.0 12.0]
#  [21.0 32.0]]
print(x * y)
print(np.multiply(x, y))

# Elementwise division; both produce the array
# [[ 0.2         0.33333333]
#  [ 0.42857143  0.5       ]]
print(x / y)
print(np.divide(x, y))

# Elementwise square root; produces the array
# [[ 1.          1.41421356]
#  [ 1.73205081  2.        ]]
print(np.sqrt(x))
```

We use the `dot` function to compute inner products of vectors, to multiply a vector by a matrix, and to multiply matrices. `dot` is available both as a function in the numpy module and as an instance method of array objects:

```python
import numpy as np

x = np.array([[1,2],[3,4]])
y = np.array([[5,6],[7,8]])

v = np.array([9,10])
w = np.array([11, 12])

# Inner product of vectors; both produce 219
print(v.dot(w))
print(np.dot(v, w))

# Matrix / vector product; both produce the rank 1 array [29 67]
print(x.dot(v))
print(np.dot(x, v))

# Matrix / matrix product; both produce the rank 2 array
# [[19 22]
#  [43 50]]
print(x.dot(y))
print(np.dot(x, y))

#x.T is used to get transpose of a matrix
print(x.T)
```

```
import numpy as np

# Compute outer product of vectors
v = np.array([1,2,3])  # v has shape (3,)
w = np.array([4,5])    # w has shape (2,)
# To compute an outer product, we first reshape v to be a column
# vector of shape (3, 1); we can then broadcast it against w to yield
# an output of shape (3, 2), which is the outer product of v and w:
# [[ 4  5]
#  [ 8 10]
#  [12 15]]
print(np.reshape(v, (3, 1)) * w)

# Add a vector to each row of a matrix
x = np.array([[1,2,3], [4,5,6]])
# x has shape (2, 3) and v has shape (3,) so they broadcast to (2, 3),
# giving the following matrix:
# [[2 4 6]
#  [5 7 9]]
print(x + v)

# Add a vector to each column of a matrix
# x has shape (2, 3) and w has shape (2,).
# If we transpose x then it has shape (3, 2) and can be broadcast
# against w to yield a result of shape (3, 2); transposing this result
# yields the final result of shape (2, 3) which is the matrix x with
# the vector w added to each column. Gives the following matrix:
# [[ 5  6  7]
#  [ 9 10 11]]
print((x.T + w).T)
# Another solution is to reshape w to be a column vector of shape (2, 1);
# we can then broadcast it directly against x to produce the same
# output.
print(x + np.reshape(w, (2, 1)))

# Multiply a matrix by a constant:
# x has shape (2, 3). Numpy treats scalars as arrays of shape ();
# these can be broadcast together to shape (2, 3), producing the
# following array:
# [[ 2  4  6]
#  [ 8 10 12]]
print(x * 2)
```

#### Reshaping

```python
import numpy as np

# Compute outer product of vectors
v = np.array([1,2,3])  # v has shape (3,)
w = np.array([4,5])    # w has shape (2,)
# To compute an outer product, we first reshape v to be a column
# vector of shape (3, 1); we can then broadcast it against w to yield
# an output of shape (3, 2), which is the outer product of v and w:
# [[ 4  5]
#  [ 8 10]
#  [12 15]]
print(np.reshape(v, (3, 1)) * w)

# Add a vector to each row of a matrix
x = np.array([[1,2,3], [4,5,6]])
# x has shape (2, 3) and v has shape (3,) so they broadcast to (2, 3),
# giving the following matrix:
# [[2 4 6]
#  [5 7 9]]
print(x + v)

# Add a vector to each column of a matrix
# x has shape (2, 3) and w has shape (2,).
# If we transpose x then it has shape (3, 2) and can be broadcast
# against w to yield a result of shape (3, 2); transposing this result
# yields the final result of shape (2, 3) which is the matrix x with
# the vector w added to each column. Gives the following matrix:
# [[ 5  6  7]
#  [ 9 10 11]]
print((x.T + w).T)
# Another solution is to reshape w to be a column vector of shape (2, 1);
# we can then broadcast it directly against x to produce the same
# output.
print(x + np.reshape(w, (2, 1)))

# Multiply a matrix by a constant:
# x has shape (2, 3). Numpy treats scalars as arrays of shape ();
# these can be broadcast together to shape (2, 3), producing the
# following array:
# [[ 2  4  6]
#  [ 8 10 12]]
print(x * 2)
```

Mathematical Operations: https://docs.scipy.org/doc/numpy/reference/routines.math.html

The NumPy linspace function (sometimes called np.linspace) is a tool in Python for creating numeric sequences.

```python
np.linspace(start = 0, stop = 100, num = 5)
```

## SciPy

SciPy is a scientific computing library for Python. It is built into numpy so we can use it by just importing numPy as well.

SciPy provides some basic functions to work with images.

```python
from scipy.misc import imread, imsave, imresize

# Read an JPEG image into a numpy array
img = imread('assets/cat.jpg')
print(img.dtype, img.shape)  # Prints "uint8 (400, 248, 3)"

# We can tint the image by scaling each of the color channels
# by a different scalar constant. The image has shape (400, 248, 3);
# we multiply it by the array [1, 0.95, 0.9] of shape (3,);
# numpy broadcasting means that this leaves the red channel unchanged,
# and multiplies the green and blue channels by 0.95 and 0.9
# respectively.
img_tinted = img * [1, 0.95, 0.9]

# Resize the tinted image to be 300 by 300 pixels.
img_tinted = imresize(img_tinted, (300, 300))

# Write the tinted image back to disk
imsave('assets/cat_tinted.jpg', img_tinted)
```

The functions `scipy.io.loadmat` and `scipy.io.savemat` allow you to read and write MATLAB files.

#### Distance between points

SciPy defines some useful functions for computing distances between sets of points.

The function `scipy.spatial.distance.pdist` computes the distance between all pairs of points in a given set:

```python
import numpy as np
from scipy.spatial.distance import pdist, squareform

# Create the following array where each row is a point in 2D space:
# [[0 1]
#  [1 0]
#  [2 0]]
x = np.array([[0, 1], [1, 0], [2, 0]])
print(x)

# Compute the Euclidean distance between all rows of x.
# d[i, j] is the Euclidean distance between x[i, :] and x[j, :],
# and d is the following array:
# [[ 0.          1.41421356  2.23606798]
#  [ 1.41421356  0.          1.        ]
#  [ 2.23606798  1.          0.        ]]
d = squareform(pdist(x, 'euclidean'))
print(d)
```

SciPy also provides useful linear algebra functions . scipy.linalg contains all the functions that are in numpy.linalg. Additionally, scipy.linalg also has some other advanced functions that are not in numpy.linalg. 

The **scipy.linalg.solve** feature solves the linear equation a * x + b * y = Z, for the unknown x, y values.

```python
#importing the scipy and numpy packages
from scipy import linalg
import numpy as np

#Declaring the numpy arrays
a = np.array([[3, 2, 0], [1, -1, 0], [0, 5, 1]])
b = np.array([2, 4, -1])

#Passing the values to the solve function
x = linalg.solve(a, b)

#printing the result array
print x
```

#### Finding a Determinant

```python
#importing the scipy and numpy packages
from scipy import linalg
import numpy as np

#Declaring the numpy array
A = np.array([[1,2],[3,4]])

#Passing the values to the det function
x = linalg.det(A)

#printing the result
print x
```

#### Eigenvalues and Eigenvectors

```python
#importing the scipy and numpy packages
from scipy import linalg
import numpy as np

#Declaring the numpy array
A = np.array([[1,2],[3,4]])

#Passing the values to the eig function
l, v = linalg.eig(A)

#printing the result for eigen values
print l

#printing the result for eigen vectors
print v
```

#### Singular Value Decomposition

```python
#importing the scipy and numpy packages
from scipy import linalg
import numpy as np

#Declaring the numpy array
a = np.random.randn(3, 2) + 1.j*np.random.randn(3, 2)

#Passing the values to the eig function
U, s, Vh = linalg.svd(a)

# printing the result
print U, Vh, s
```

## Pandas

Pandas is a data manipulation library for python.

It is built on the Numpy package and its key data structure is called the DataFrame. DataFrames allow you to store and manipulate tabular data in rows of observations and columns of variables.

```python
dict = {"country": ["Brazil", "Russia", "India", "China", "South Africa"],
       "capital": ["Brasilia", "Moscow", "New Dehli", "Beijing", "Pretoria"],
       "area": [8.516, 17.10, 3.286, 9.597, 1.221],
       "population": [200.4, 143.5, 1252, 1357, 52.98] }

import pandas as pd
brics = pd.DataFrame(dict)
print(brics)
# Set the index for brics
brics.index = ["BR", "RU", "IN", "CH", "SA"]

# Print out brics with new index values
print(brics)
```

Another way to create a DataFrame is by importing a csv/excel/json/sql file using Pandas.

```python
import pandas as pd

# Import the cars.csv data: cars
cars = pd.read_csv('cars.csv')

# Print out cars
print(cars)
```

Indexing:

```python
# Import pandas and cars.csv
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Print out country column as Pandas Series
print(cars['cars_per_cap'])

# Print out country column as Pandas DataFrame
print(cars[['cars_per_cap']])

# Print out DataFrame with country and drives_right columns
print(cars[['cars_per_cap', 'country']])

# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Print out first 4 observations
print(cars[0:4])

# Print out fifth, sixth, and seventh observation
print(cars[4:6])

# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)

# Print out observation for Japan
print(cars.iloc[2])

# Print out observations for Australia and Egypt
print(cars.loc[['AUS', 'EG']])
```

#### Exploratory data analysis

```python
df = pd.read_csv(path)
df.head()#First 5 rows
df.tail() #Last 5 rows
df.dtypes #Datatypes of each column
df.describe()#Descriptive Stats
df.info()#Info About Each Column
df.ndim #Dimensions
df.shape #shape
df.size #size
df.to_csv("automobile.csv", index=False) #save csv

```

#### Data Cleaning and Manipulating in Pandas

```python
df.groupby(by =[‘class’, ‘doctor_name’]).size() #Aggregation
df.isna().sum() #Number of Missing Values
df = df.dropna(axis = 0, how = 'any') #Remove missing valued rows
df.nunique() #Checking Duplicates
#Remove duplicates
df[df.duplicated(subset = 'patient_id', keep =False)].sort_values('patient_id') 
repeat_patients = df.groupby(by = 'patient_id').size().sort_values(ascending =False)
filtered_patients = repeat_patients[repeat_patients > 2].to_frame().reset_index()
filtered_df = df[~df.patient_id.isin(filtered_patients.patient_id)]

#One Hot Encoding
categorical_df = df[['patient_id','doctor_name']]
categorical_df['doctor_count'] = 1 
doctors_one_hot_encoded = pd.pivot_table( categorical_df,
                                  index = categorical_df.index, 
                                  columns = ['doctor_name'], 
                                   values = ['doctor_count'] )
doctors_one_hot_encoded = doctors_one_hot_encoded.fillna(0)
doctors_one_hot_encoded.columns = doctors_one_hot_encoded.columns.droplevel()
leftJoin_df = pd.merge(df1, df2, on ='col_name', how='left') #Merge Back
combined_df = pd.merge(df, one_hot_encoded, left_index = True,right_index =True, how =’left’)


#Removing a column
combined_df = combined_df.drop(columns=['doctor_name'])

#Filling Missing Values
df.fillna(0) #fill with zero
>>> values = {'A': 0, 'B': 1, 'C': 2, 'D': 3}
>>> df.fillna(value=values) #filling with values

```

## Matplotlib

#### Basic Plot

```python
from matplotlib import pyplot as plt

x = [5,8,10]
y = [12,16,6]

plt.plot(x,y)

plt.title('Epic Info')
plt.ylabel('Y axis')
plt.xlabel('X axis')

plt.show()
```

![adding labels and title to our matplotlib graph](https://pythonprogramming.net/static/images/basics/matplotlib-labels-and-title-tutorial.png)

#### Bar Plot

```python
from matplotlib import pyplot as plt
x = [5,8,10]
y = [12,16,6]

x2 = [6,9,11]
y2 = [6,15,7]


plt.bar(x, y, align='center')

plt.bar(x2, y2, color='g', align='center')


plt.title('Epic Info')
plt.ylabel('Y axis')
plt.xlabel('X axis')

plt.show()
```

![Matplotlib centered bar chart](https://pythonprogramming.net/static/images/basics/matplotlib-bar-chart-tutorial.png)

#### Scatter Plot

```python
from matplotlib import pyplot as plt
from matplotlib import style

style.use('ggplot')

x = [5,8,10]
y = [12,16,6]

x2 = [6,9,11]
y2 = [6,15,7]

plt.scatter(x, y)#, align='center')

plt.scatter(x2, y2, color='g')#, align='center')
#we can have label="String"
#plt.legends() to show legends

plt.title('Epic Info')
plt.ylabel('Y axis')
plt.xlabel('X axis')

plt.show()
```

![matplotlib graphing tutorial series](https://pythonprogramming.net/static/images/basics/matplotlib-scatter-plot-tutorial.png)

#### Histogram

```
import matplotlib.pyplot as plt

population_ages = [22,55,62,45,21,22,34,42,42,4,99,102,110,120,121,122,130,111,115,112,80,75,65,54,44,43,42,48]

bins = [0,10,20,30,40,50,60,70,80,90,100,110,120,130]

plt.hist(population_ages, bins, histtype='bar', rwidth=0.8)

plt.xlabel('x')
plt.ylabel('y')
plt.title('Interesting Graph\nCheck it out')
plt.legend()
plt.show()
```

![img](https://pythonprogramming.net/static/images/matplotlib/matplotlib-histogram-tutorial.png)

#### Pie Charts

```python
import matplotlib.pyplot as plt

slices = [7,2,2,13]
activities = ['sleeping','eating','working','playing']
cols = ['c','m','r','b']

plt.pie(slices,
        labels=activities,
        colors=cols,
        startangle=90,
        shadow= True,
        explode=(0,0.1,0,0),
        autopct='%1.1f%%')

plt.title('Interesting Graph\nCheck it out')
plt.show()
```



## Seaborn

Seaborn is built upon matplotlib to give enriched visualizations. Seaborn is also easier to use than matplotlib

#### Aesthetics

The interface for manipulating the styles is **set_style()**. Using this function you can set the theme of the plot. As per the latest updated version, below are the five themes available.

- Darkgrid
- Whitegrid
- Dark
- White
- Ticks

Let us try applying a theme from the above-mentioned list. The default theme of the plot will be **darkgrid** .

```python
import numpy as np
from matplotlib import pyplot as plt
def sinplot(flip=1):
   x = np.linspace(0, 14, 100)
   for i in range(1, 5):
      plt.plot(x, np.sin(x + i * .5) * (7 - i) * flip)
import seaborn as sb
sb.set_style("whitegrid")
sinplot()
plt.show()
```

#### Color Palette

```python
from matplotlib import pyplot as plt
import seaborn as sb
current_palette = sb.color_palette()
sb.palplot(current_palette)
plt.show()
```

#### Histogram (Distplot)

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('iris')
sb.distplot(df['petal_length'],kde = False)
plt.show()
```

Line Histogram

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('iris')
sb.distplot(df['petal_length'],hist=False)
plt.show()
```

#### Scatter Plot

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('iris')
sb.jointplot(x = 'petal_length',y = 'petal_width',data = df)
plt.show()
```

#### **Box Plot**

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('iris')
sb.swarmplot(x = "species", y = "petal_length", data = df)
plt.show()
```

#### **Bar Plot**

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('titanic')
sb.barplot(x = "sex", y = "survived", hue = "class", data = df)
plt.show()
```

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('titanic')
sb.countplot(x = " class ", data = df, palette = "Blues");
plt.show()
```

#### Regression Plot

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('tips')
sb.regplot(x = "total_bill", y = "tip", data = df)
sb.lmplot(x = "total_bill", y = "tip", data = df)
plt.show()
```

![Zoomed and Magnifier](https://www.tutorialspoint.com/seaborn/images/zoomed_magnifier.jpg)

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('anscombe')
sb.lmplot(x = "x", y = "y", data = df.query("dataset == 'II'"),order = 2)
plt.show()
```

![parabola](https://www.tutorialspoint.com/seaborn/images/parabola.jpg)

#### Pair Grid

PairGrid allows us to draw a grid of subplots using the same plot type to visualize data.

Unlike FacetGrid (2 variables), it uses different pair of variable for each  subplot. It forms a matrix of sub-plots. It is also sometimes called as  “scatterplot matrix”.

The usage of pairgrid is similar to facetgrid. First initialise the grid and then pass the plotting function.

```python
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df = sb.load_dataset('iris')
g = sb.PairGrid(df)
g.map_diag(plt.hist)
g.map_offdiag(plt.scatter);
plt.show()
```

![Colored ](https://www.tutorialspoint.com/seaborn/images/colored.jpg)

## Scikit-Learn

Scikit-Learn is a machine learning library for python. It contains lots of algorithms implemented and ready to use.

The general procedure to use scikit-learn is as follows

1. Import an algorithm from sklearn
2. Create a model
3. Fit training data to the model
4. Evaluate/Predict test data.

#### Preprocessing

```python
#import the necessary module
from sklearn import preprocessing
# create the Labelencoder object
le = preprocessing.LabelEncoder()
#convert the categorical columns into numeric
encoded_value = le.fit_transform(["paris", "paris", "tokyo", "amsterdam"])
print(encoded_value)

from sklearn.model_selection import train_test_split
setsdata_train, data_test, target_train, target_test = train_test_split(data,target, test_size = 0.30, random_state = 10)
```

#### Creating a Model

```python
# import the necessary module
from sklearn.naive_bayes import GaussianNB
from sklearn.metrics import accuracy_score
#create an object of the type GaussianNB
gnb = GaussianNB()
#train the algorithm on training data and predict using the testing data
pred = gnb.fit(data_train, target_train).predict(data_test)
#print(pred.tolist())
#print the accuracy score of the model
print("Naive-Bayes accuracy : ",accuracy_score(target_test, pred, normalize = True))
```

## Keras

Keras is a high level API for tensorflow to quickly create deep neural networks.

A 3 layer Neural network using keras

```python
from keras.models import Sequential
from keras.layers import Dense
import numpy
```

```python
model = Sequential()
model.add(Dense(12, input_dim=11, init='uniform', activation='relu'))
model.add(Dense(8, init='uniform', activation='relu'))
model.add(Dense(1, init='uniform', activation='sigmoid'))
```

```python
model.compile(loss='binary_crossentropy', optimizer='adam', metrics=['accuracy'])
```

```python
model.fit(X, Y, nb_epoch=200, batch_size=30)
```

```python
scores = model.evaluate(X, Y)
print("%s: %.2f%%" % (model.metrics_names[1], scores[1]*100))
```

A simple CNN using Keras

```python
import tensorflow as tf

class myCallback(tf.keras.callbacks.Callback):
  def on_epoch_end(self, epoch, logs={}):
    if(logs.get('acc')>0.998):
      print("\nReached 99.8% accuracy so cancelling training!")
      self.model.stop_training = True

mnist = tf.keras.datasets.mnist
(training_images, training_labels), (test_images, test_labels) = mnist.load_data()

training_images=training_images.reshape(60000, 28, 28, 1)
training_images=training_images / 255.0
test_images = test_images.reshape(10000, 28, 28, 1)
test_images=test_images/255.0

callbacks=myCallback()

model = tf.keras.models.Sequential([
    tf.keras.layers.Conv2D(32,(3,3),activation='relu', input_shape=(28, 28, 1)),
    tf.keras.layers.MaxPooling2D(2,2),
    tf.keras.layers.Flatten(),
    tf.keras.layers.Dense(128, activation='relu'),
    tf.keras.layers.Dense(10, activation='softmax')
])

model.compile(optimizer='adam',loss='sparse_categorical_crossentropy',metrics=['accuracy'])

model.fit(training_images,training_labels,epochs=20,callbacks=[callbacks])
```

## Tensorflow

It is a high performance tensor computing library. It is the most popular deep learning library.

```python
import tensorflow as tf
```

Building a graph

```python
graph1 = tf.Graph()
```

Creating Variables

```python
with graph1.as_default():
    a = tf.constant([2], name = 'constant_a')
    b = tf.constant([3], name = 'constant_b')
   
with graph1.as_default():
    c = tf.add(a, b)
    #c = a + b is also a way to define the sum of the terms
```

Running a graph as a session

```python
with tf.Session(graph = graph1) as sess:
    result = sess.run(c)
    print(result)
```

Defining Matrices, Vectors etc..

```python
graph2 = tf.Graph()
with graph2.as_default():
    Scalar = tf.constant(2)
    Vector = tf.constant([5,6,2])
    Matrix = tf.constant([[1,2,3],[2,3,4],[3,4,5]])
    Tensor = tf.constant( [ [[1,2,3],[2,3,4],[3,4,5]] , [[4,5,6],[5,6,7],[6,7,8]] , [[7,8,9],[8,9,10],[9,10,11]] ] )
with tf.Session(graph = graph2) as sess:
    result = sess.run(Scalar)
    print ("Scalar (1 entry):\n %s \n" % result)
    result = sess.run(Vector)
    print ("Vector (3 entries) :\n %s \n" % result)
    result = sess.run(Matrix)
    print ("Matrix (3x3 entries):\n %s \n" % result)
    result = sess.run(Tensor)
    print ("Tensor (3x3x3 entries) :\n %s \n" % result)
```

Placeholders

```python
x  = tf.placeholder(tf.float32, shape=[None, 784])
y_ = tf.placeholder(tf.float32, shape=[None, 10])
```

Weights and Biases

```python
# Weight tensor
W = tf.Variable(tf.zeros([784, 10],tf.float32))
# Bias tensor
b = tf.Variable(tf.zeros([10],tf.float32))
```

```python
# run the op initialize_all_variables using an interactive session
sess.run(tf.global_variables_initializer())
```

```python
# mathematical operation to add weights and biases to the inputs
tf.matmul(x,W) + b
```

```python
y = tf.nn.softmax(tf.matmul(x,W) + b)
```

### Cost function

It  is a function that is used to minimize the difference between the right  answers (labels) and estimated outputs by our Network. 

```python
cross_entropy = tf.reduce_mean(-tf.reduce_sum(y_ * tf.log(y), reduction_indices=[1]))
```

### Type of optimization: Gradient Descent

This  is the part where you configure the optimizer for your Neural Network.  There are several optimizers available, in our case we will use Gradient  Descent because it is a well established optimizer.

```python
train_step = tf.train.GradientDescentOptimizer(0.5).minimize(cross_entropy)
```

### Training batches

Train using minibatch Gradient Descent.

In practice, Batch Gradient Descent is not often used because is too  computationally expensive. The good part about this method is that you  have the true gradient, but with the expensive computing task of using  the whole dataset in one time. Due to this problem, Neural Networks  usually use minibatch to train.

```python
#Load 50 training examples for each training iteration   
for i in range(1000):
    batch = mnist.train.next_batch(50)
    train_step.run(feed_dict={x: batch[0], y_: batch[1]})
```

### Test

```python
correct_prediction = tf.equal(tf.argmax(y, 1), tf.argmax(y_, 1))
accuracy = tf.reduce_mean(tf.cast(correct_prediction, tf.float32))
acc = accuracy.eval(feed_dict={x: mnist.test.images, y_: mnist.test.labels}) * 100
print("The final accuracy for the simple ANN model is: {} % ".format(acc) )
#The final accuracy for the simple ANN model is: 91.82999730110168 % 
sess.close() #finish the session
```

# Quick R Revision

R is an open source programming language mainly used for statistical analysis.

## Basic R

##  Variables in R 

We can also **store** our output in **variables**, so we can use them later on. For example:

```r
x <- 139 + 121
```

To return the value of **x**, we can simply run the variable as a command:

```r
x
```

We can also perform operations on **x** and save the result to a **new variable**:

```r
y <- x / 60
y
```

If we save something to an **existing variable**, it will **overwrite** the previous value:

```r
x <- x / 60
x
```

It's good practice to use **meaningful variable names**, so you don't have to keep track of what variable is what:

```r
total <- 139 + 121
total
total_hr <- total / 60
total_hr
```

You can put this all into a single expression, but remember to use **round brackets** to add together the movie lengths first, before dividing by 60.

```r
total_hr <- (139 + 121) / 60
total_hr
```

## Vectors in R

What if we want to know the **movie length in hours**, not minutes, for *Toy Story* and for *Akira*?

- **Toy Story (1995)**: 81 min
- **Akira (1998)**: 125 min

```r
c(81, 125) / 60
```

As you see above, we've applied a single math operation to both of the items in **c(81, 125)**. You can even assign **c(81, 125)** to a variable before performing an operation.

```r
ratings <- c(81, 125)
ratings / 60
```

What we just did was create vectors, using the combine function **c()**. The **c()** function takes multiple items, then combines them into a **vector**. 

It's important to understand that **vectors** are used everywhere in R, and vectors are easy to use.

```r
c(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
c(1:10)
c(10:1) # 10 to 1
```

## Strings in R

R isn't just about numbers -- we can also have strings too. For example:

```r
movie <- "Toy Story"
movie
```

In R, you can identify **character strings** when they are wrapped with **matching double (") or single (') quotes**.

Let's create a **character vector** for the following **genres**:

- Animation
- Comedy
- Biography
- Horror
- Romance
- Sci-fi

```r
genres <- c("Animation", "Comedy", "Biography", "Horror", "Romance", "Sci-fi")
genres
```

Conditional Statements

We often want to check a conditional statement and then do something in response to that condition being true or false.

Vectors

**Vectors**  are strings of numbers, characters or logical data (one-dimension  array). In other words, a vector is a simple tool to store your grouped  data.

In R, you create a vector with the combine function **c()**.  You place the vector elements separated by a comma between the  brackets. Vectors will be very useful in the future as they allow you to  apply operations on a series of data easily.

Note that the items in a vector must be of the same class, for example all should be either number, character, or logical.

### Numeric, Character and Logical Vectors

Let's say we have four movie release dates (1985, 1999, 2015, 1964) and we want to assign them to a single variable, `release_year`. This means we'll need to create a vector using **c()**.

Using numbers, this becomes a **numeric vector**.

```r
release_year <- c(1985, 1999, 2015, 1964)
release_year
```

What if we use quotation marks? Then this becomes a **character vector**.

```r
# Create genre vector and assign values to it 
titles <- c("Toy Story", "Akira", "The Breakfast Club")
titles
```

There are also **logical vectors**, which consist of TRUE's and FALSE's. They're particular important when you want to check its contents

```r
titles == "Akira" # which item in `titles` is equal to "Akira"?
```

------

####  [Tip] TRUE and FALSE in R 

Did you know? R only recognizes `TRUE`, `FALSE`, `T` and `F` as special values for true and false. That means all other spellings, including *True* and *true*, are not interpreted by R as logical values.



------



Vector Operations

### Adding more elements to a vector

You can add more elements to a vector with the same **c()** function you use the create vectors:

```r
release_year <- c(1985, 1999, 2015, 1964)
release_year
release_year <- c(release_year, 2016:2018)
release_year
```

### Length of a vector

How do we check how many items there are in a vector? We can use the **length()** function:

```r
release_year
length(release_year)
```

### Head and Tail of a vector

We can also retrieve just the **first few items** using the **head()** function:

```r
head(release_year) #first six items
head(release_year, n = 2) #first n items
head(release_year, 2)
```

We can also retrieve just the **last few items** using the **tail()** function:

```r
tail(release_year) #last six items
tail(release_year, 2) #last two items
```

### Sorting a vector

We can also sort a vector:

```r
sort(release_year)
```

We can also **sort in decreasing order**:

```r
sort(release_year, decreasing = TRUE)
```

But if you just want the minimum and maximum values of a vector, you can use the **min()** and **max()** functions

```r
min(release_year)
max(release_year)
```

### Average of Numbers

If you want to check the  average cost of movies produced in 2014, what would you do? Of course,  one way is to add all the numbers together, then divide by the number of  movies:

```r
cost_2014 <- c(8.6, 8.5, 8.1)

# sum results in the sum of all elements in the vector
avg_cost_2014 <- sum(cost_2014)/3
avg_cost_2014
```

You also can use the **mean** function to find the average of the numeric values in a vector:

```r
mean_cost_2014 <- mean(cost_2014)
mean_cost_2014
```

### Giving Names to Values in a Vector

Suppose you want to remember which year corresponds to which movie.

With vectors, you can give names to the elements of a vector using the **names() ** function:

```r
#Creating a year vector
release_year <- c(1985, 1999, 2010, 2002)

#Assigning names
names(release_year) <- c("The Breakfast Club", "American Beauty", "Black Swan", "Chicago")

release_year
```

Now, you can retrieve the values based on the names:

```r
release_year[c("American Beauty", "Chicago")]
```

Note that the values of the vector are still the years. We can see this in action by adding a number to the first item:

```r
release_year[1] + 100 #adding 100 to the first item changes the year
```

And you can retrieve the names of the vector using **names()**

```r
names(release_year)[1:3]
```

### Summarizing Vectors

You can also use the **"summary"** function for simple descriptive statistics: minimum, first quartile, mean, third quartile, maximum:

```r
summary(cost_2014)
```

### Using Logical Operations on Vectors

A vector can also be comprised of **TRUE** and **FALSE**, which are special **logical values** in R. These boolean values are used used to indicate whether a condition is true or false.  

Let's check whether a movie year of 1997 is older than (**greater in value than**) 2000.

```r
movie_year <- 1997
movie_year > 2000
```

You  can also make a logical comparison across multiple items in a vector.  Which movie release years here are "greater" than 2014?

```r
movies_years <- c(1998, 2010, 2016)
movies_years > 2014
```

We can also check for **equivalence**, using **==**. Let's check which movie year is equal to 2015.

```r
movies_years == 2015 # is equal to 2015?
```

If you want to check which ones are **not equal** to 2015, you can use **!=**

```r
movies_years != 2015
```

------

####  [Tip] Logical Operators in R 



 You can do a variety of logical operations in R including:   

 Checking equivalence: **1 == 2** 

 Checking non-equivalence: **TRUE != FALSE** 

 Greater than: **100 > 1** 

 Greater than or equal to: **100 >= 1** 

 Less than: **1 < 2** 

 Less than or equal to: **1 <= 2** 

------



Subsetting Vectors

What if you wanted to retrieve the second year from the following **vector of movie years**?

```r
movie_years <- c(1985, 1999, 2002, 2010, 2012)
movie_years
```

To retrieve the **second year**, you can use square brackets **[]**:

```r
movie_years[2] #second item
```

To retrieve the **third year**, you can use:

```r
movie_years[3]
```

And if you want to retrieve **multiple items**, you can pass in a vector:

```r
movie_years[c(1,3)] #first and third items
```

**Retrieving a vector without some of its items**

To retrieve a vector without an item, you can use negative indexing. For example, the following returns a vector slice **without the first item**.

```r
titles <- c("Black Swan", "Jumanji", "City of God", "Toy Story", "Casino")
titles[-1]
```

You can save the new vector using a variable:

```r
new_titles <- titles[-1] #removes "Black Swan", the first item
new_titles
```

** Missing Values (NA)**

Sometimes values in a vector are missing and you have to show them  using NA, which is a special value in R for "Not Available". For  example, if you don't know the age restriction for some movies, you can  use NA.

```r
age_restric <- c(14, 12, 10, NA, 18, NA)
age_restric
```

####  [Tip] Checking NA in R 



 You can check if a value is NA by using the **is.na()** function, which returns TRUE or FALSE.  

 Check if NA: **is.na(NA)** 

 Check if not NA: **!is.na(2)** 

### Subsetting vectors based on a logical condition

What if we want to know  which movies were created after year 2000? We can simply apply a logical  comparison across all the items in a vector:

```r
release_year > 2000
```

To retrieve the actual movie years after year 2000, you can simply subset the vector using the logical vector within **square brackets "[]"**:

```r
release_year[movie_years > 2000] #returns a vector for elements that returned TRUE for the condition
```

As you may notice, subsetting vectors in R works by retrieving items that were TRUE for the provided condition. For example, `year[year > 2000]` can be verbally explained as: *"From the vector year, return only values where the values are TRUE for year > 2000"*.

You can even manually write out TRUE or T for the values you want to subset:

```r
release_year
release_year[c(T, F, F, F)] #returns the values that are TRUE
```



Factors

Factors are variables in R which take on a limited number of different values; such variables are often refered to as  **categorical variables**.  The difference between a categorical variable and a continuous variable  is that a categorical variable can belong to a limited number of  categories. A continuous variable, on the other hand, can correspond to  an infinite number of values. For example, the height of a tree is a  continuous variable, but the titles of books would be a categorical  variable.

One of the most important uses of factors is in statistical modeling;  since categorical variables enter into statistical models differently  than continuous variables, storing data as factors insures that the  modeling functions will treat such data correctly. 

Let's start with a ***vector*** of genres:

```r
genre_vector <- c("Comedy", "Animation", "Crime", "Comedy", "Animation")
genre_vector
```

As you may have noticed, you can theoretically group the items above into three categories of genres: *Animation*, *Comedy* and *Crime*. In R-terms, we call these categories **"factor levels"**.

The function **factor()** converts a vector into a factor, and creates a factor level for each unique element.

```r
genre_factor <- as.factor(genre_vector)
levels(genre_factor)
```

### Summarizing Factors

When you have a large  vector, it becomes difficult to identify which levels are most common  (e.g., "How many 'Comedy' movies are there?").

To answer this, we can use **summary()**, which produces a **frequency table**, as a named vector.

```r
summary(genre_factor)
```

And recall that you can sort the values of the table using **sort()**.

```r
sort(summary(genre_factor)) #sorts values by ascending order
```

### Ordered factors

There are two types of categorical variables: a **nominal categorical variable** and an **ordinal categorical variable**.

A **nominal variable** is a categorical variable for  names, without an implied order. This means that it is impossible to say  that 'one is better or larger than the other'. For example, consider **movie genre** with the categories *Comedy*, *Animation*, *Crime*, *Comedy*, *Animation*. Here, there is no implicit order of low-to-high or high-to-low between the categories. 

In contrast, **ordinal variables** do have a natural ordering. Consider for example, **movie length** with the categories: *Very short*, *Short* , *Medium*, *Long*, *Very long*. Here it is obvious that *Medium* stands above *Short*, and *Long* stands above *Medium*.

```r
movie_length <- c("Very Short", "Short", "Medium","Short", "Long",
                        "Very Short", "Very Long")
movie_length
```

**movie_length** should be converted to an ordinal factor since its categories have a natural ordering. By default, the function **factor()** transforms `movie_length` into an unordered factor. 

To create an **ordered factor**, you have to add two additional arguments: `ordered` and `levels`. 

- `ordered`: When set to `TRUE` in `factor()`, you indicate that the factor is ordered. 
- `levels`: In this argument in `factor()`, you give the values of the factor in the correct order.

```r
movie_length_ordered <- factor(movie_length, ordered = TRUE , 
                                 levels = c("Very Short" , "Short" , "Medium", 
                                            "Long","Very Long"))
movie_length_ordered
```

Now, lets look at the summary of the ordered factor, **factor_mvlength_vector**:

```r
summary(movie_length_ordered)
```

### If Statements

**If** statements are composed of a conditional check and a block of code that is executed if the check results in **true**. For example, assume we want to check a movie's year, and print something if it greater than 2000:

```r
movie_year = 2002

# If Movie_Year is greater than 2000...
if(movie_year > 2000){

    # ...we print a message saying that it is greater than 2000.
    print('Movie year is greater than 2000')

}
```

Notice that the code in the above block **{}** will only be executed if the check results in **true**. 

You can also add an `else` block to `if` block -- the code in `else` block will only be executed if the check results in **false**.

**Syntax:** 

if (condition) {

```
# do something
```

} else {

```
# do something else
```

}

 **Tip**: This syntax can be spread over multiple lines for ease of creation and legibility. 

Let's create a variable called **Movie_Year** and attribute it the value 1997. Additionally, let's add an `if` statement to check if the value stored in **Movie_Year**  is greater than 2000 or not -- if it is, then we want to output a  message saying that Movie_Year is greater than 2000, if not, then we  output a message saying that it is not greater than 2000.

```r
movie_year = 1997

# If Movie_Year is greater than 2000...
if(movie_year > 2000){

    # ...we print a message saying that it is greater than 2000.
    print('Movie year is greater than 2000')

}else{ # If the above conditions were not met (Movie_Year is not greater than 2000)...
    
    # ...then we print a message saying that it is not greater than 2000.
    print('Movie year is not greater than 2000') 

}
```

Feel free to change **movie_year**'s value to other values -- you'll see that the result changes based on it!

To create our conditional statements to be used with **if** and **else**, we have a few tools:

### Comparison operators

When comparing two values you can use this operators

- equal: `==` 
- not equal: `!=` 
- greater/less than: `>` `<` 
-  greater/less than or equal: `>=` `<=` 

### Logical operators

Sometimes you want to check more than one condition at once. For example you might want to check if one condition **and** other condition are true. Logical operators allow you to combine or modify conditions.

-  and: `&` 
-  or: `|` 
-  not: `!` 

Let's try using these operators:

```r
movie_year = 1997

# If Movie_Year is BOTH less than 2000 AND greater than 1990 -- both conditions have to be true! -- ... 
if(movie_year < 2000 & movie_year > 1990 ) {
    # ...then we print this message.
    print('Movie year between 1990 and 2000') 
}

# If Movie_Year is EITHER greater than 2010 OR less than 2000 -- any of the conditions have to be true! -- ... 
if(movie_year > 2010 | movie_year < 2000 ) {
    # ...then we print this message.
    print('Movie year is not between 2000 and 2010') 
}
```

 **Tip**: All the expressions will return the value in Boolean format -- this format can only house two values: true or false! 

### Subset

Sometimes, we don't want an entire dataset -- maybe in a dataset of  people we want only people with age 18 and over, or in the movies  dataset, maybe we want only movies that were created after a certain  year. This means we want a **subset** of the dataset. In R, we can do this by utilizing the **subset** function.

Suppose we want a subset of the **movies_Data** data frame composed of movies from a given year forward (e.g. year 2000) if a selected variable is **recent**, or from that given year back if we select **old**. We can quite simply do that in R by doing this:

```r
decade = 'recent'

# If the decade given is recent...
if(decade == 'recent' ){
    # Subset the dataset to include only movies after year 2000.
    subset(movies_data, year >= 2000)
} else { # If not...
    # Subset the dataset to include only movies before 2000.
    subset(movies_data, year < 2000)
}
```

------



Loops

Sometimes,  you might want to repeat a given function many times. Maybe you don't  even know how many times you want it to execute, but have an idea like `once for every row in my dataset`. Repeated execution like this is supplemented by **loops**. In R, there are two main loop structures, **for** and **while**.

### The `for` loop

The `for` loop structure enables you to execute a code  block once for every element in a given structure. For example, it would  be like saying **execute this once for every row in my dataset**, or "execute this once for every element in this column bigger than 10". **for** loops are a very useful structure that make the processing of a large amount of data very simple.

Let's try to use a **for** loop to print all the years present in the **year** column in the **movies_Data** data frame. We can do that like this:

```r
# Get the data for the "year" column in the data frame.
years <- movies_data['year']

# For each value in the "years" variable...
# Note that "val" here is a variable -- it assumes the value of one of the data points in "years"!
for (val in years) {
    # ...print the year stored in "val".
    print(val)
}
```

### The `while` loop

As you can see, the `for` loop is useful for a controlled  flow of repetition. However, what if we don't know when we want to stop  the loop? What if we want to keep executing a code block until a certain  threshold has been reached, or maybe when a logical expression finally  results in an expected fashion?

The `while` loop exists as a tool for repeated execution  based on a condition. The code block will keep being executed until the  given logical condition returns a `False` boolean value.

Let's try using `while` to print the first five movie names of our dataset. It can be done like this:

```r
# Creating a start point.
iteration = 1

# We want to repeat until we reach the sixth operation -- but not execute the sixth time.
# While iteration is less or equal to five...
while (iteration <= 5) {
    
    print(c("This is iteration number:",as.character(iteration)))
    
    # ...print the "name" column of the iteration-th row.
    print(movies_data[iteration,]$name)
    
    # And then, we increase the "iteration" value -- so that we actually reach our stopping condition
    # Be careful of infinite while loops!
    iteration = iteration + 1
}
```

### Applying Functions to Vectors

One of the most common uses of loops is to **apply a given function to every element in a vector of elements**.  Any of the loop structures can do that, however, R conveniently  provides us with a very simple way to do that: By inferring the  operation.

R is a very smart language when it comes to element-wise operations.  For example, you can perform an operation on a whole list by utilizing  that function directly on it. Let's try that out:

```r
# First, we create a vector...
my_list <- c(10,12,15,19,25,33)

# ...we can try adding two to all the values in that vector.
my_list + 2

# Or maybe even exponentiating them by two.
my_list ** 2

# We can also sum two vectors element-wise!
my_list + my_list
```

R  makes it very simple to operate over vectors -- anything you think  should work will probably work. Try to mess around with vectors and see  what you find out!

This is the end of the **Loops and Conditional Execution in R**  notebook. Hopefully, now you know how to manipulate the flow of your  code to your needs. Thank you for reading this notebook, and good luck  on your studies.

What is a Function?

A function is a re-usable block of code which performs operations specified in the function.

There are two types of functions :

- **Pre-defined functions**
- **User defined functions**

**Pre-defined** functions are those that are already defined for you, whether it's in R or within a package. For example, **sum()** is a pre-defined function that returns the sum of its numeric inputs.

**User-defined** functions are custom functions created and defined by the user. For example, you can create a custom function to print **Hello World**.

### **Pre-defined functions**

There are many pre-defined functions, so let's start with the simple ones.

Using the **mean()** function, let's get the average of these three movie ratings:

- **Star Wars (1977)** - rating of 8.7 
- **Jumanji** - rating of 6.9
- **Back to the Future** - rating of 8.5

```r
ratings <- c(8.7, 6.9, 8.5)
mean(ratings)
```

We can use the **sort()** function to sort the movies rating in *ascending order*.

```r
sort(ratings)
```

You can also sort by *decreasing* order, by adding in the argument **decreasing = TRUE**.

```r
sort(ratings, decreasing = TRUE)
```

####  [Tip] How do I learn more about the pre-defined functions in R? 



 We will be introducing a variety of **pre-defined functions** to you as  you learn more about R. There are just too many functions, so there's no  way we can teach them all in one sitting. But if you'd like to take a  quick peek, here's a short reference card for some of the commonly-used  pre-defined functions:    https://cran.r-project.org/doc/contrib/Short-refcard.pdf 

### User-defined functions

Functions are very easy to create in R:

```r
printHelloWorld <- function(){
    print("Hello World")
}
printHelloWorld()
```

To use it, simply run the function with **()** at the end:

```r
printHelloWorld()
```

But what if you want the function to provide some **output** based on some **inputs**?

```r
add <- function(x, y) {
    x + y
}
add(3, 4)
```

As  you can see above, you can create functions with the following syntax  to take in inputs (as its arguments), then provide some output.

**f <- function(<arguments>) {  Do something  Do something  return(some_output)}**

------



Explicitly returning outputs in user-defined functions

In R, the last line in the function is automatically inferred as the output the function. 

#### You can also explicitly tell the function to return an output.

```r
add <- function(x, y){
    return(x + y)
}
add(3, 4)
```

It's good practice to use the `return()` function to explicitly tell the function to return the output.

------



Using IF/ELSE statements in functions

The **return()** function is particularly  useful if you have any IF statements in the function, when you want your  output to be dependent on some condition:

```r
isGoodRating <- function(rating){
    #This function returns "NO" if the input value is less than 7. Otherwise it returns "YES".
    
    if(rating < 7){
        return("NO") # return NO if the movie rating is less than 7
    
    }else{
        return("YES") # otherwise return YES
    }
}

isGoodRating(6)
isGoodRating(9.5)
```

------



Setting default argument values in your custom functions

You can a set a default value for arguments in your function. For example, in the **isGoodRating()** function, what if we wanted to create a threshold for what we consider to be a good rating?  

Perhaps by default, we should set the threshold to 7:

```r
isGoodRating <- function(rating, threshold = 7){
    if(rating < threshold){
        return("NO") # return NO if the movie rating is less than the threshold
    }else{
        return("YES") # otherwise return YES
    }
}

isGoodRating(6)
isGoodRating(10)
```

Notice  how we did not have to explicitly specify the second argument  (threshold), but we could specify it. Let's say we have a higher  standard for movie ratings, so let's bring our threshold up to 8.5:

```r
isGoodRating(8, threshold = 8.5)
```

Great! Now you know how to create default values. **Note that** if you know the order of the arguments, you do not need to write out the argument, as in:

```r
isGoodRating(8, 8.5) #rating = 8, threshold = 8.5
```

------



Using functions within functions

Using functions within functions is no big deal. In fact, you've already used the **print()** and **return()** functions. So let's try making our **isGoodRating()** more interesting.

Let's create a function  that can help us decide on which movie to watch, based on its rating. We  should be able to provide the name of the movie, and it should return **NO** if the movie rating is below 7, and **YES** otherwise.

First, let's read in our movies data:

```r
my_data <- read.csv("movies-db.csv")
head(my_data)
```

Next, do you remember how to check the value of the **average_rating** column if we specify a movie name?
Here's how:

```r
# Within myData, the row should be where the first column equals "Akira"
# AND the column should be "average_rating"

akira <- my_data[my_data$name == "Akira", "average_rating"]
akira

isGoodRating(akira)
```

Now, let's put this all together into a function, that can take any **moviename** and return a **YES** or **NO** for whether or not we should watch it.

```r
watchMovie <- function(data, moviename){
    rating <- data[data["name"] == moviename,"average_rating"]
    return(isGoodRating(rating))
}

watchMovie(my_data, "Akira")
```

**Make sure you take the time to understand the function above.** Notice how the function expects two inputs: `data` and `moviename`, and so when we use the function, we must also input two arguments.

*But what if we only want to watch really good movies? How do we set our rating threshold that we created earlier? * 
 Here's how:

```r
watchMovie <- function(data, moviename, my_threshold){
    rating <- data[data$name == moviename,"average_rating"]
    return(isGoodRating(rating, threshold = my_threshold))
}
```

Now our watchMovie takes three inputs: **data**, **moviename** and **my_threshold**

```r
watchMovie(my_data, "Akira", 7)
```

*What if we want to still set our default threshold to be 7?* 
 Here's how we can do it:

```r
watchMovie <- function(data, moviename, my_threshold = 7){
    rating <- data[data[,1] == moviename,"average_rating"]
    return(isGoodRating(rating, threshold = my_threshold))
}

watchMovie(my_data,"Akira")
```

As you can imagine, if we assign the output to a variable, the variable will be assigned to **YES**

```r
a <- watchMovie(my_data, "Akira")
a
```

While the **watchMovie** is easier to use, I can't tell what the movie rating actually is. How do I make it *print* what the actual movie rating is, before giving me a response? To do so, we can simply add in a **print** statement before the final line of the function.  

We can also use the built-in **paste()** function to concatenate a sequence of character strings together into a single string.

```r
watchMovie <- function(moviename, my_threshold = 7){
    rating <- my_data[my_data[,1] == moviename,"average_rating"]

    memo <- paste("The movie rating for", moviename, "is", rating)
    print(memo)
    
    return(isGoodRating(rating, threshold = my_threshold))
}

watchMovie("Akira")
```

Just note that the returned output is actually the resulting value of the function:

```r
x <- watchMovie("Akira")
print(x)
```

------



Global and local variables

So far, we've been creating variables within functions, but did you  notice what happens to those variables outside of the function?  

Let's try to see what **memo** returns:

```r
watchMovie <- function(moviename, my_threshold = 7){
    rating <- my_data[my_data[,1] == moviename,"average_rating"]
    
    memo <- paste("The movie rating for", moviename, "is", rating)
    print(memo)
    
    isGoodRating(rating, threshold = my_threshold)
}

watchMovie("Akira")
memo
```

**We got an error:**  `object 'memo' not found`. **Why?**  

It's because all the variables we create in the function remain within the function. In technical terms, this is a **local variable**, meaning that the variable assignment does not persist outside the function. The `memo` variable only exists within the function.    

But there is a way to create **global variables** from within a function -- where you can use the global variable outside of the function. It is typically *not*  recommended that you use global variables, since it may become harder  to manage your code, so this is just for your information.  

To create a **global variable**, we need to use this syntax:

> **x <<- 1**

Here's an example of a global variable assignment:

```r
myFunction <- function(){
    y <<- 3.14
    return("Hello World")
    }
myFunction()
y #created only in the myFunction function
```

------

## What is an Array?

 An array is a structure that holds values grouped together, like a 2 x 2  table of 2 rows and 2 columns. Arrays can also be **multidimensional**,  such as a 2 x 2 x 2 array.

#### What is the difference between an array and a vector?

Vectors are always one dimensional like a single row of data. On the  other hand, an array can be multidimensional (stored as rows and  columns). The "dimension" indicates how many rows of data there are.

#### Let's create a 4 x 3 array (4 rows, 3 columns)

The example below is a vector of 9 movie names, hence the data type is the same for all the elements.

```r
#lets first create a vector of nine movies
movie_vector <- c("Akira", "Toy Story", "Room", "The Wave", "Whiplash",
                  "Star Wars", "The Ring", "The Artist", "Jumanji")
movie_vector
```

To create an array, we can use the **array()** function.

```r
movie_array <- array(movie_vector, dim = c(4,3))
movie_array
```

Note that **arrays are created column-wise**. Did you also notice that there were only 9 movie names, but the array was 4 x 3? The original **vector doesn't have enough elements**  to fill the entire array (that should have 3 x 4 = 12 elements). So R  simply fills rest of the empty values by going back to the beginning of  the vector and starting again ("Akira", "Toy story", "Room" in this  case).

We also needed to provide **c(4,3)** as a second *argument* to specify the number of rows (4) and columns (3) that we wanted.

 **[Tip] What is an "argument"? How are "arguments" different from "_parameters_"?**    

 Arguments and parameters are terms you will hear constantly when talking about **functions**.   - The _**parameters**_ are the input variables used in a function, like **dim** in the function **array()**.    - The _**arguments**_ refer to the _values_ for those parameters that a function takes as inputs, like **c(4,3)**   

 We actually don't need to write out the name of the parameter (dim) each time, as in:   `array(movie_vector, c(4,3))`   As long as we write the arguments out in the correct order, R can interpret the code.    

 Arguments in a function may sometimes need to be of a **specific type**.  For more information on each function, you can open up the help file by  running the function name with a ? beforehand, as in:   `?array` 



## Array Indexing

Let's look at our array again:

```r
movie_array
```

To access an element of an array, we should pass in **[row, column]** as the row and column number of that element.
For example, here we retrieve **Whiplash** from row 1 and column 2:

```r
movie_array[1,2] #[row, column]
```

To  display all the elements of the first row, we should put 1 in the row  and nothing in the column part. Be sure to keep in the comma after the `1`.

```r
movie_array[1,]
```

Likewise, you can get the elements by column as below.

```r
movie_array[,2]
```

To get the dimension of the array, **dim()** should be used.

```r
dim(movie_array)
```

We can also do math on arrays. Let's create an array of the lengths of each of the nine movies used earlier.

```r
length_vector <- c(125, 81, 118, 81, 106, 121, 95, 100, 104)
length_array <- array(length_vector, dim = c(3,3))
length_array
```

Let's add 5 to the array, to account for a 5-min bathroom break:

```r
length_array + 5
```

 **Tip**: Performing operations on objects, like adding 5 to an array,  does not change the object. **To change the object, we would need to  assign the new result to itself**. 



## Using Logical Conditions to Subset Arrays

Which  movies can I finish watching in two hours? Using a logical condition,  we can check which movies are less than 2 hours long.

```r
mask_array <- length_array > 120
mask_array
```

Using this array of TRUEs and FALSEs, we can subset the array of movie names:

```r
x_vector <- c("Akira", "Toy Story", "Room", "The Wave", "Whiplash",
              "Star Wars", "The Ring", "The Artist", "Jumanji")
x_array <- array(x_vector, dim = c(3,3))

x_array[mask_array]
```

## What is a Matrix?

Matrices are a subtype of arrays. A matrix **must** have 2 dimensions, whereas arrays are more flexible and can have, 1, 2 or more dimensions.  

To create a matrix out of a vector , you can use **matrix()**, which takes in an argument for the vector, an argument for the number of rows and another for the number of columns.

```r
movie_matrix <- matrix(movie_vector, nrow = 3, ncol = 3)
movie_matrix
```

### Accessing elements of a matrix

As with arrays, you can use **[row, column]** to access elements of a matrix. To retrieve "Akira", you should use [1,1] as it lies in the first row and first column.

```r
movie_matrix[1,1]
```

To get data from a certain range, the folowing code can help. This takes the elements from rows 2 to 3, and from columns 1 to 2.

```r
movie_matrix[2:3, 1:2]
```

## Concatenation function

A concatenation function is used to combine two vectors into one vector. It combines values of both vectors.
 Lets create a new vector for the upcoming movies as upcoming_movie and  add them to the movie_vector to create a new_vector of movies.

```r
upcoming_movie <- c("Fast and Furious 8", "xXx: Return of Xander Cage", "Suicide Squad")
new_vector <- c(movie_vector, upcoming_movie)
new_vector
```

## Download the Data

We've  made it easy for you to get the data, which we've hosted online. Simply  run the code cell below (Shift + Enter) to download the data to your  current folder.

```r
# Download datasets

# CSV file
download.file("https://ibm.box.com/shared/static/n5ay5qadfe7e1nnsv5s01oe1x62mq51j.csv", 
              destfile="movies-db.csv")

# XLS file
download.file("https://ibm.box.com/shared/static/nx0ohd9sq0iz3p871zg8ehc1m39ibpx6.xls", 
              destfile="movies-db.xls")
```

**If you ran the cell above, you have now downloaded the following files to your current folder:**

> movies-db.csv
> movies-db.xls



Reading CSV Files

#### What are CSV files?

Let's read data from a  CSV file. CSV (Comma Separated Values) is one of the most common formats  of structured data you will find. These files contain data in a table  format, where in each row, columns are separated by a delimiter --  traditionally, a comma (hence comma-separated values).   

Usually, the first line in a CSV file contains the column names for  the table itself. CSV files are popular because you do not need a  particular program to open it.

#### Reading CSV files in R

In the **movies-db.csv** file, the first line of text is the header (names of each of the columns), followed by rows of movie information.

To read CSV files into R, we use the core function **read.csv**.  

`read.csv` easy to use. All you need is the filepath to the CSV file. Let's try loading the file using the filepath to the `movies-db.csv` file we downloaded earlier:

```r
# Load the CSV table into the my_data variable.
my_data <- read.csv("movies-db.csv")
my_data
```

The data was loaded into the `my_data` variable. But instead of viewing all the data at once, we can use the `head` function to take a look at only the top six rows of our table, like so:

```r
# Print out the first six rows of my_data
head(my_data)
```

Additionally, you may want to take a look at the **structure** of your newly created table. R provides us with a function that summarizes an entire table's properties, called `str`. Let's try it out.

```r
# Prints out the structure of your table.
str(my_data)
```

When we loaded the file with the `read.csv` function, we had to only pass it one parameter -- the **path** to our desired file.

If you're using Data Scientist Workbench, it is simple to find the path to your uploaded file. In the **Recent Data**  section in the sidebar on the right, you can click the arrow to the  left of the filename to see extra options -- one of these commands  should be **Insert Path**, which automatically copies the path to your file into Jupyter Notebooks.

------



Reading Excel Files

Reading  XLS (Excel Spreadsheet) files is similar to reading CSV files, but  there's one catch -- R does not have a native function to read them.  However, thankfully, R has an extremely large repository of user-created  functions, called *CRAN*. From there, we can download a library package to make us able to read XLS files.

To download a package, we use the `install.packages` function. Once installed, you do not need to install that same library ever again, unless, of course, you uninstall it.

```r
# Download and install the "readxl" library
install.packages("readxl")
```

Whenever  you are going to use a library that is not native to R, you have to  load it into the R environment after you install it. In other words, you  need to install once only, but to use it, you must load it into R for  every new session. To do so, use the `library` function, which loads up everything we can use in that library into R.

```r
# Load the "readxl" library into the R environment.
library(readxl)
```

Now that we have our library and its functions ready, we can move on to actually reading the file. In `readxl`, there is a function called `read_excel`, which does all the work for us. You can use it like this:

```r
# Read data from the XLS file and attribute the table to the my_excel_data variable.
my_excel_data <- read_excel("movies-db.xls")
```

Since `my_excel_data`  is now a dataframe in R, much like the one we created out of the CSV  file, all of the native R functions can be applied to it, like `head` and `str`.

```r
# Prints out the structure of your table.
# Tells you how many rows and columns there are, and the names and type of each column.
# This should be the very same as the other table we created, as they are the same dataset.
str(my_excel_data)
```

Much like the `read.csv` function, `read_excel` takes as its main parameter the **path** to the desired file.

 **[Tip]**    A **Library** is basically a collection of different classes and  functions which are used to perform some specific operations. You can  install and use libraries to add more functions that are not included on  the core R files. For example, the **readxl** library adds functions to read data from  excel files. 

 It's important to know that there are many other libraries too which can  be used for a variety of things. There are also plenty of other  libraries to read Excel files -- readxl is just one of them. 

------

Accessing Rows and Columns

Whenever  we use functions to read tabular data in R, the default method of  structuring this data in the R environment is using Data Frames -- R's  primary data structure. Data Frames are extremely versatile, and R  presents us many options to manipulate them.

Suppose we want to access the "name" column of our dataset. We can  directly reference the column name on our data frame to retrieve this  data, like this:

```r
# Retrieve a subset of the data frame consisting of the "name" columns
my_data['name']
```

Another way to do this is by using the `$` notation which at the output will provide a vector:

```r
# Retrieve the data for the "name" column in the data frame.
my_data$name
```

You can also do the same thing using **double square brackets**, to get a vector of `names` column.

```r
my_data[["name"]]
```

Similarly,  any particular row of the dataset can also be accessed. For example, to  get the first row of the dataset with all column values, we can use:

```r
# Retrieve the first row of the data frame.
my_data[1,]
```

The first value before the comma represents the **row** of the dataset and the second value (which is blank in the above example) represents the **column**  of the dataset to be retrieved. By setting the first number as 1 we say  we want data from row 1. By leaving the column blank we say we want all  the columns in that row.

We can specify more than one column or row by using **c**, the **concatenate** function. By using `c` to concatenate a list of elements, we tell R that we want these observations out of the data frame. Let's try it out.

```r
# Retrieve the first row of the data frame, but only the "name" and "length_min" columns.
my_data[1, c("name","length_min")]
```

------



Accessing Built-in Datasets in R

R  provides various built-in datasets for users to utilize for different  purposes. To know which datasets are available, R provides a simple  function -- `data` -- that returns all of the present datasets' names with a small description beside them. The ones in the `datasets` package are all inbuilt.

```r
# Displays a list of the inbuilt datasets. Opens in a new "window".
data()
```

As  you can see, there are many different datasets already inbuilt in the R  environment. Having to go through each of them to take a look at their  structure and try to find out what they represent might be very tiring.  Thankfully, R has documentation present for each inbuilt dataset. You  can take a look at that by using the `help` function.

For example, if we want to know more about the `women` dataset, we can use the following function:

```r
# Opens up the documentation for the inbuilt "women" dataset.
help(women)
```

Since  the datasets listed are inbuilt, you do not need to import or load them  to use them. If you reference them by their name, R already has the  data frame ready.

```r
women
```

Lists

First of all, we're gonna take a look at lists in R. A list is a  sequenced collection of different objects of R, like vectors, numbers,  characters, other lists as well, and so on. You can consider a list as a  container of correlated information, well structured and easy to read. A  list accepts items of different types, but a vector (or a matrix, which  is a multidimensional vector) doesn't. To create a list just type **list()** with your content inside the parenthesis and separated by commas. Let’s try it!

```r
movie <- list("Toy Story", 1995, c("Animation", "Adventure", "Comedy"))
```

In  the code above, the variable movie contains a list of 3 objects, which  are a string, a numeric value, and a vector of strings. Easy, eh? Now  let's print the content of the list. We just need to call its name.

```r
movie
```

A  list has a sequence and each element of a list has a position in that  sequence, which starts from 1. If you look at our previous example, you  can see that each element has its position represented by double square  brackets "**[[ ]]**".

### Accessing items in a list

It is possible to retrieve only a part of a list using the **single _square** bracket operator_ "**[ ]**". This operator can be also used to get a single element in a specific position. Take a look at the next example:

The index number 2 returns the second element of a list, if that element exists:

```r
movie[2]
```

Or  you can select a part or interval of elements of a list. In our next  example we are retrieving the 1st, 2nd, and 3rd elements:

```r
movie[2:3]
```

It looks a little confusing, but lists can also store names for its elements.

### Named lists

The following list is a named list:

```r
movie <- list(name = "Toy Story",
             year = 1995,
             genre = c("Animation", "Adventure", "Comedy"))
```

Let me explain that: the list **movie** has some named objects within it. **name**, for example, is an object of type **character**, **year** is an object of type **number**, and **genre** is a vector with objects of type **character**.

Now take a look at this list. This time, it's full of information and  well organized. It's clear what each element means. You can see that  the elements have different types, and that's ok because it's a list.

```r
movie
```

You can also get separated information from the list. You can use **listName$selectorName**. The *dollar-sign operator* **$** will give you the block of data that is related to selectorName.

Let's get the genre part of our movies list, for example.

```r
movie$genre
```

Another way of selecting the genre column:

```r
movie["genre"]
```

You can also use numerical selectors like an array. Here we are selecting elements from 2 to 3.

```r
movie[2:3]
```

The function **class()** returns the type of a object. You can use that function to retrieve the type of specific elements of a list:

```r
class(movie$name)
class(movie$foreign)
```

### Adding, modifying, and removing items

Adding a new element is also very easy. The code below adds a new field named **age**  and puts the numerical value 0 into it. In this case we use the double  square brackets operator, because we are directly referencing a list  member (and we want to change its content).

```r
movie[["age"]] <- 5
movie
```

In order to modify, you just need to reference a list member that already exists, then change its content.

```r
movie[["age"]] <- 6
# Now it's 6, not 5
movie
```

And removing is also easy! You just put **NULL**, which means missing value/data, into it.

```r
movie[["age"]] <- NULL
movie
```

### Concatenating lists

Concatenation is the proccess of puting things together, in sequence. And yes, you can do it with lists. Just call the function **c()**. Take a look at the next example:

```r
# We split our previous list in two sublists
movie_part1 <- list(name = "Toy Story")
movie_part2 <- list(year = 1995, genre = c("Animation", "Adventure", "Comedy"))

# Now we call the function c() to put everything together again
movie_concatenated <- c(movie_part1, movie_part2)

# Check it out
movie_concatenated
```

Lists  are really handy for organizing different types of elements in R, and  also easy to use. Additionally, lists are also important since this type  of data structure is essential to create data frames, our next covered  topic.

------



DataFrames

A  DataFrame is a structure that is used for storing data tables.  Underneath it all, a data frame is a list of vectors of same length,  exactly like a table (each vector is a column). We call a function  called  **data.frame()** to create a data frame and pass  vector, which are our columns, as arguments. It is required to name the  columns that will compose the data frame.

```r
movies <- data.frame(name = c("Toy Story", "Akira", "The Breakfast Club", "The Artist",
                              "Modern Times", "Fight Club", "City of God", "The Untouchables"),
                    year = c(1995, 1998, 1985, 2011, 1936, 1999, 2002, 1987),
                    stringsAsFactors=F)
```

Let's print its content of our recently created data frame:

```r
movies
```

It's very easy! You can note how it looks like a table.

We can also use the **"$"** selector to get some type of  information. This operator returns the content of a specific column of a  data frame (that's why we have to choose a name for each column).

```r
movies$name
```

You retrieve data using numeric indexing, like in lists:

```r
# This returns the first (1st) column
movies[1]
```

The function called **str()**  is one of most useful functions in R. With this function you can obtain  textual information about an object. In this case,  it delivers  information about the objects whitin a data frame. Let's see what it  returns:

```r
str(movies)
```

It shouws this data frame has 8 observations, for 2 columns, so called **name** and **year**. The "name" column is a factor with 8 levels and "year" is a numerical column. 

The class() function works for data frames as well. You can use it to determine the type of a column of a data frame.

```r
class(movies$year)
```

You can use numerical selectors to reach information inside the table.

```r
movies[1,2] #1-Toy Story, 2-1995
```

The **head()**  function is very useful when you have a large table and you need to  take a peek at the first elements. This function returns the first 6  values of a data frame (or event a list).

```r
head(movies)
```

Similar to the previous function, **tail()** returns the last 6 values of a data frame or list.

```r
tail(movies)
```

Now let's try to add a new column to our data frame with the length of each movie in minutes.

```r
movies['length'] <- c(81, 125, 97, 100, 87, 139, 130, 119)
movies
```

A  new column was included into our data frame with just one line of code.  We just needed to add a vector to data frame, then it will be our new  column.

Now let's try to add a new movie to our data set.

```r
movies <- rbind(movies, c(name="Dr. Strangelove", year=1964, length=94))
movies
```

Remember, you can't add a list with more variables than the data frame, and vice-versa.

We don't need this movie  anymore, so let's delete it. Here we are deleting row 12 by assigning to  itself the movies dataframe without the 12th row.

```r
movies <- movies[-12,]
movies
```

To delete a column you can just set it as **NULL**.

```r
movies[["length"]] <- NULL
movies
```

What is an Object?

Everthing that you manipulate in R, literally every entity in R, is considered an **object**.  In real life, we think of an object as something that we can hold and  look at. R objects are a lot like that. For example, vector is one of  the objects in R. 

An object in R has different kinds of properties or attributes. One of the attributes in objects is called the **class** of the object. The **class**  of an object is the data type of this object. For instance, the class  of vector can be numeric if it's composed of numeric values or character  if it's composed of string values. The various classes (data types) of  objects in R are important for data science programming.

### Class

The most common classes (data types) of objects in R are:

- numeric (real numbers)
- character
- integer
- logical (True/False)
- complex

If you want to know about the data type of your values, you can use the **"class()"**  function and add the variables' name to it. Let's create a variable  from the average rating of some movies and then find which data types  they belong to:

```r
movie_rating <- c(8.3, 5.2, 9.3, 8.0) # create a vector from average ratings 
movie_rating # print the variable
```

To check what is the data type, let's use **class()**

```r
class(movie_rating) # show the variable's data type
```

As you see, the **class()** function shows that the data type of values in the vector is **numeric**.

 **Tip:** A vector can only contain objects of the same class. However, a list can have different data types.  

### Numeric

Decimal values are called numerics. They are the default  computational data type in R. In the example below, If we assign a  decimal value to a variable average_rating, then average_rating will be  of numeric type.

```r
average_rating <- 8.3       # assign a decimal value
average_rating           
```

Using **class** to check the data type results in **numeric**

```r
class(average_rating)      
```

### Character

A character object is used to represent string values in R, strings are simply text values. 

```r
movies <-c("Toy Story", "Akira", "The Breakfast Club", "The Artist")
movies
class(movies)
```

If numbers and texts are combined in a vector, everything is converted to the class **character**. Let's make a vector from combined movie names and their production year, then find the data type for the vector

```r
combined <- c("Toy Story", 1995, "Akira", 1998)
combined
class(combined)
```

When you simply enter numbers into R, they will be saved as class **numeric** by default. For example in the following vector, even though the numbers are integers, they are stored as numeric type in R:

```r
movie_length <- c(80, 110, 90, 80) # create a vector from movie length
movie_length # print the variable
class(movie_length)
```

### Integer

An integer is a number that can be written without a fractional  component. For example, 21, 4, 0, and −2048 are integers, while 9.75, 5  1⁄2, and √2 are not. In R, when you create a variable from the mentioned  numbers, they are not going to be stored as integer data type. In order  to get the integer class we need to convert the variable type from  numeric to integer using **as.integer()** function. Let's create a vector and check if the data type is numeric.

```r
age_restriction <- c(12, 10, 18, 18) # create a vector from age restriction
age_restriction # print the vector

class(age_restriction)
integer_vector <- as.integer(age_restriction)
class(integer_vector)
```

### Logical

The logical class contains True/False values (Boolean values). Let's create a vector with logical values and check its class: 

```r
logical_vector <- c(T,F,F,T,T) # creating the vector
class(logical_vector)
```

A logical value is often created via comparison between variables. In the below example, we will compare the length of movies **Toy Story and Akira**.

```r
length_Akira <- 125
length_ToyStory <- 81
```

If  we assign the result of the compare statement to a variable the  variable will have FALSE if the statement was false, and TRUE if the  statement is true.

```r
x <- length_ToyStory > length_Akira      # is ToyStory larger than akira? 
x              
x <- length_Akira > length_ToyStory # is akira larger than ToyStory?               
x # print the logical value
```

The resulting variable is of type logical

```r
class(x)       # print the class name of x
```

### Complex

A complex number is a number that can be expressed in the form a +  bi, where a and b are real numbers and i is the imaginary unit.

```r
z = 8 + 6i     # create a complex number 
z
class(z)
```

------



Converting One Class to Another

We can convert (coerce) one data type to another if we desire. For  example, we can convert objects from other data types into character  values with the **"as.character()"** function. In the following example, we convert numeric value into character:

```r
year <- as.character(1995) # convert integer into character data type
year                    # print the value of year in character data type
```

As we mentioned before, in order to create an integer variable in R, we can use the **"as.integer()"**  function. In the following example, even though the number is an  integer data type, R saves the number as numeric data type by default.  So you need to change the number to integer later if it is necessary.

```r
Length_ToyStory <- 81
class(81)
length_ToyStory <- as.integer(81) 
class(length_ToyStory)       # print the class name of length_ToyStory
```

------



Difference between Class and Mode

For a simple vector, the class and mode of the vector are the same  thing: the data type of the values inside the vector (character,  numeric, integer, etc). However, in some of other objects such as  matrix, array, data frame, and list, class and mode means different  things. 

In those mentioned objects, the **class()** function shows the type of the data structure. What does that mean? The class of matrix will be **matrix** regardless of what data types are **inside** the matrix. The same applies to list, array and data frame.

**Mode** on the other hand, determines what types of  data can be found within the object and how that values are stored. So,  you need to use the **mode()** function to find the data type of values inside a matrix (character, numeric, integer, etc).

So, in addition to the classes such as numeric, character, integer,  logical, and complex, we have other classes such as matix, array,  dataframe, and list

### Matrix

Let’s create a matrix storing the genre for each movie. Then, we will  find the class and mode of the created matrix to see which information  we will get from them.

First, let's check the effect of class and mode on a **vector**.

```r
movies <- c("Toy Story", "Akira", "The Breakfast Club", "The Artist") # creating two vectors
genre <- c("Animation/Adventure/Comedy", "Animation/Adventure/Comedy", "Comedy/Drama", "Comedy/Drama")

class(movies)
mode(movies)
```

As  you see in the above, for the vector the class and mode shows the data  type of values. Now lets create a matrix from these two vectors.

```r
movies_genre <- cbind(movies, genre)
movies_genre 
```

Now **class()** shows that the data type is **matrix**.

```r
class(movies_genre)
```

And **mode** shows the data type of the elements of the matrix

```r
mode(movies_genre)
```

For the matrix, the **class()** shows how the values are stored and shown in R, in this case, in a matrix. However, **mode()** shows the data type of values in the matrix. In the above example we have made a matrix filled with **character** values.

### Array

A slightly more complicated version of the **matrix** data type is the **array** data type. The **array** data type  can still only have one data type inside of it, but the set of data types it can store is larger. In  addition to the data types an array can store matrices as its elements. In the following, we are going to create the array from  integer number (1 to 12) and then compare the class and mode in an  array: 

```r
sample_array <- array(1:12, dim = c(3, 2, 2)) # create an array with dimensions 3 x 2 x 2 
sample_array
class(sample_array)
mode(sample_array)
```

So, the array's class is **array** and its mode is **numeric**.

### Data Frame

Data frames are similar to arrays but they have certain advantages  over arrays. Data frames allow you to associate each row and each column  with a name of your choosing and allow **each column** of the data frame to have a **different data type** if you like. Let's create a data frame from the movie names, year and their length:

```r
Name <- c("Toy Story", "Akira", "The Breakfast Club", "The Artist")
Year <- c(1995, 1998, 1985, 2011)
Length <- c(81, 125, 97, 100)
RowNames = c("Movie 1", "Movie 2", "Movie 3", "Movie 4")

sample_DataFrame <- data.frame(Name, Year, Length, row.names=RowNames) 
sample_DataFrame

class(sample_DataFrame)
```

So, the class of the above table is "data.frame".

### List

The final data type that we are going to go over is **list**. Lists are similar to vectors, but they can contain multiple data types. For example:

```r
sample_List = list("Star Wars", 8.7, TRUE)
sample_List

class(sample_List)

mode(sample_List)

mode(sample_List[[3]])
```

As  you see, we have character, numeric, and logical data types in the  list. The data type of third element in the list is logical as the  "mode()" function shows us. The **mode** for the entire list is **list**, it could show the type of all the elements, since they don't all have the same data type.

------



Attributes

Objects have one or more **attributes** that can modify  how R thinks about the object. Imagine you have a  bowl of pasta and  cheese. If you add spice, you change it to something with new taste.  Different spices makes different dishes. 

Attributes are like spice. You can change any individual attribute of object with the **attr()** *function. You also can use the **attribute()** function to return a list of all of the attributes currently defined for that object.* 

For example in the following code, we will create a vector from the  average ratings (8.3, 8.1, 7.9, 8) and costs of four movies (30, 10.4,  1, 15), and then we change the **dim** attribute of the vector. R will now treat z as it were a 4-by-2 matrix.  

```r
z <- c(8.3, 8.1, 7.9, 8, 30, 10.4, 1, 15)
z
attr(z, "dim") <- c(4,2)
z
```

Now, we can find the class and mode of the above matrix.

```r
class(z)
mode(z)
```

## String Operations

There  are many string operation methods in R which can be used to manipulate  the data. We are going to use some basic string operations on the data  that we read before. 

### nchar()

The first function is **nchar()**  which will return the total number of characters in the given string.  Let's find out how many characters are there in the first element of **my_data** variable.

```r
nchar(my_data[1])
```



### toupper()

Now, sometimes we need the whole string to be in Upper Case. To do so, there is a function called **toupper()** in R which takes a string as input and provides the whole string in upper case at output.

```r
toupper(my_data[3])
```

**In above** code block, we convert the third element of the character vector in upper case.



### tolower()

Similarly, **tolower()**  method can be used to convert whole string into lower case. Let's  convert the same string that we convert in upper case, into lower case.

```r
tolower(my_data[3])
```

**We can** clearly see the difference between the outputs of last two methods.



### chartr()

`what if we want to replace any characters in given string?` This operation can also be performed in R using **chartr()**  method which takes three arguments. The first argument is the  characters which we want to replace in string, second argument is the  new characters and the last argument is the string on which operation  will be performed.

Let's replace **white spaces** in the string with the **hyphen (“-”) sign** in the first element of the **my_data** variable. 

```r
chartr(" ", "-", my_data[1])
```



### strsplit()

Previously, we learned that we can read file word by word using **scan()** function. `But what if we want to split the given string word by word?`

This can be done using **strsplit()** method. Let's split the string according to the white spaces.

```r
character_list <- strsplit(my_data[1], " ")
word_list <- unlist(character_list)
word_list
```

In above code block, we separate the string word by word, but **strsplit()**  method provides a list at the output which contains all the separated  words as single element which is more complex to read. So, to make it  more easy to read each word as single element, we used **unlist()** method which converts the list into character vector and now we can easily access each word as a single element.



### sort()

Sorting is also possible in R. Let's use **sort()** method to sort elements of the **word_list** character vector in ascending order.

```r
sorted_list <- sort(word_list)
sorted_list
```



### paste()

Now, we sort all the elements of ** word_list** character vector. Let's use **paste()** function here, which is used to concatenate strings. This method takes two arguments, the strings we want to concatenate and **collapse** argument which defines the separator in the words.

Here, we are going to concatenate all words of **sorted_list** character vector into a single string.

```r
paste(sorted_list, collapse = " ")
```



### substr()

There is another function **substr()** in R which is used to get a sub section of the string.

Let's take an example to understand it more. In example below, we use the **substr()**  method and provide it three arguments. First argument is the data  string from which we want the sub string. Second argument is the  starting point from where function will start reading the string and the  third argument is the stopping point till where we want the function to  read string.

```r
sub_string <- substr(my_data[1], start = 4, stop = 50)
sub_string
```

So,  from the character vector, we start reading the first element from 4th  position and read the string till 50th position and at the output, we  get the resulted string which we stored in **sub_string** variable.



### trimws()

As  the sub string that we get in code block above, have some white spaces  at the initial and end points. So, to quickly remove them, we can use **trimws()** method of R like shown below.

```r
trimws(sub_string)
```

So, at the output, we get the string which does not contain any white spaces at the both ends.



### str_sub()

To read string from last, we are using **stringr** library. This library contains **str_sub()** method, which takes same arguments as **sub_stirng** method but read string from last.

Like in the example below, we provide a data string and both starting  and end points with negative values which indicates that we are reading  string from last.

```r
library(stringr)
str_sub(my_data[1], -8, -1)
```

So, we read string from -1 till -8 and it gives **talkies.** with full stop mark at the output.

------



## Writing and Saving to Files

After reading files, we can also write data into files and save them in different file formats like **.txt, .csv, .xls (for excel files) etc**. Let's take a look at some examples.

### Exporting as Text File

Suppose we want to export a matrices or String in **.txt** file. To do so, we can use **write()** method which writes into file and save that on to disk.

Let's create a matrix and try to save it into file.

```r
m <- matrix(c(1, 2, 3, 4, 5, 6), nrow = 2, ncol = 3)
m
write(m, file = "my_text_file.txt", ncolumns = 3, sep = " ")
```

In  above code block, we provide the input data, file name in which we want  to store data along with its path and as we are using matrices to  output in file, we provide **ncolumns** argument value and **sep** argument.

Let's try to write a string from our **my_data** variable into file named as **my_text_file2.txt**

```r
write(my_data[1], file = "my_text_file2.txt", ncolumns = 1, sep = " ")
```

So, we get the first element from **my_data** variable and provide it as input to write function and this time we assign **ncolumn** argument with value 1 because we want a single column for string.



### Exporting as CSV File

As we export data in text files, we can export data into **CSV** files also. To do so, we need a data frame which have data. For this, we can use built-in datasets.

Let's use **CO2** dataset of R which contains data about Carbon Dioxide Uptake in Grass Plants. Let's see how data look like in **CO2**dataset.

```r
head(CO2)
```

Now, let's export this data into **CSV** file. We will use **write.csv()** method which takes data frame as input and a **file** argument to specify output filename.

```r
write.csv(CO2, file = "my_csv.csv")
```

Now,  when we will execute above code block, all data will be exported in CSV  file. Now, the first column of CSV file contains row numbers which we  do not want in our CSV file. So, we have to define **row.names** to **FALSE** in **write.csv()** method.

```r
write.csv(CO2, file = "my_csv.csv", row.names = FALSE)
```

Similarly, to remove column names just make **col.names** to **FALSE**. 



### Exporting as Excel File

To save data into excel files, we have to install an external library called **xlsx**, which will provide us easy methods to export data into **.xlsx** files.

Let's install this library. (This may take a minute or two)

```r
install.packages("xlsx")
library(xlsx)
write.xlsx(CO2, file = "my_excel.xlsx", row.names = FALSE)
```

So, exporting data in **.xlsx** files is similary to **.csv** files just function name is different plus we had to install external library to do this operation.



### Exporting as .RData File

In R, we can also save files in **.RData** format. **.RData** format provides a way to save and load our R objects.

Let's create simple variable objects and save that into file with extension**.RData**.

```r
var1 <- "var1"
var2 <- "var2"
var3 <- "var3"
```

Now, to write in **.RData** file, we will use **save()** method of R. It has a **list**  argument which is the list containing the variable names of all the  objects we want to save (which in this case are three vaiables), **file** argument which contains file name in which we are going to write/save data and **safe** argument is to specify whether you want the saving to be performed atomically.

```r
save(list = c("var1", "var2", "var3"), file = "variables.RData", safe = T)
```

The file with name **variables.RData** is generated on the provided location.

### plot

The `plot` library is the default R library for plotting  graphs. It's very simplistic in both syntax and aesthetics. To use it to  create a bar plot, you use the `barplot` function, like so:

```r
count <- table(mtcars$cyl)
barplot(count)
```

## ggplot2

### ggplot2

`ggplot2`, as mentioned above, is a specialized library made to create visually pleasing data visualizations. Before we can use `ggplot2`, we need to import it into the R environment. The code cell below will check if your system already has ggplot, as to not run `install.packages` for no reason. Then, using the `library` function, we can then import `ggplot2`.

```r
if("ggplot2" %in% rownames(installed.packages()) == FALSE) {install.packages("ggplot2")}
library(ggplot2)
```

Now, let's plot our graph. To plot a simple bar graph using `ggplot2`'s `qplot`, we use this:

```r
qplot(mtcars$cyl, geom = "bar")
```

#### ggplot2 have two principal functions, `qplot()` and `ggplot()`.

   • `qplot()` offers a simpler syntax similar to the default `plot` function, but is limited in customization.

   • `ggplot()` is the full-fledged function. It has far more possible customizations, but has a more complicated syntax than `qplot()`.

In this course, we will start using `qplot()` and then change to `ggplot()` as you advance.

The next graph is a demonstration of what is possible to do with `ggplot()`. In the end of this course you will be able to create graphs like this one below and even more complex ones. 

```r
ggplot(data= mtcars, aes(mtcars$hp))  + 
  geom_histogram(breaks=seq(40, 350, by = 25),  
                 colour = I("black"),
                 aes(fill=..count..))

```

![img](data:image/png;base64,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v9+/c+fOiooKwcHsnY8++qiqqurjjz9+8sknBQdTJ7xJmDFerzcQCJjL5iim6xpcSygU2rBhw8KFC0eNGiU4mL1z4403Pvnkk//2b//2H//xH4KDqROOdcaMHz++trZWKXXy5MkxY8bEXYO4lFLPPvtseXn55MmTzTUczB6LfYjf6/W2tbUJDqZOuA6672zcuPH06dMOh6OkpOThhx8WQlRXVx89elQIsXz58th75Z3WoKuDBw8+99xzxcXFQoiioqJFixYJDmZPvf/++6+88oqUMhQKLV68ePz48YKDqQ0CGgA0xSkOANAUAQ0AmiKgAUBTBDQAaIqARmasXbs2TR95WLVqVcdvDcNIx16APsBVHMgMu93e2tpqt/fks6zhcDjuP3z99defe+6506dPjx49+utf//pDDz0khDAMXuTIVoygkRaGYWzYsKGkpGTcuHH79+//l3/5l1tvvfXWW2/94IMPhBCVlZWRSGTWrFkzZ84MBoP79u2bOnVqSUlJaWnp3r17hRALFy687bbbSkpK7r///qampljN1atXz5s374UXXggGg1/5yldKSkr+8R//8b777hNCtLe3L1q0aNu2bQsWLNizZ0/HO80//fTTpaWl//AP/7B79+5YqYqKikWLFk2fPv21117r66MDJClDN2lCPyeEePHFF5VSO3bs8Hg8b731llLqhz/84Te+8Q3zATabLRQKKaUuXrw4bNiw3//+90qpcDjc1NRkrjQftn79+srKyljNl19+2Vyurq6+9957zeXm5malVHt7e35+/u9+97uVK1d26mTLli1KqZqamptuuqlTqUuXLn3uc5+7cOFCmo4D0BsENNJCCGHeEfTMmTNDhgwxVx44cKCsrMxcjgX0//zP/9x5552d/nlVVdXtt98+ffr0kpKSL3/5y7Gafr/fXD5z5szo0aOXLVu2Y8cOn88Xq3/33XcPHjx49uzZhw8f7tSJUio3N7e9vd1c2dLSYq6cO3fu7t27rT8EQK9xigPp4nK5hBA2m81cMJfD4XCnh3V9E+/YsWPPPvvs7t279+/fv3bt2tbW1tim2D3VRo8eXVtb+6UvfWnv3r0lJSXmrXzKyspef/31pUuXPvbYY3Pnzo29CRlrQEoZiUTM5dg9KEKhEG8kQk8ENDJj8ODBzc3NQoiysrITJ068++67QgjzFMfly5dHjhyZn58vhPjFL34R95+fO3dOCDF37txnnnnG7/dfunQpGAzW1dUJIQzDmDRpUnt7eyyL4/rJT34ihDh16tTRo0e/8IUvWP38AAtwP2hkxmOPPTZ9+nSXy3X48OFdu3Z95zvf8fl8Nptt8+bNs2bN2r59+5w5c/Lz82+44YaLFy92/efvv/9+RUWFUioajX7rW9+66aabfD7fypUrP/3007Nnz77xxhs/+tGPHA5Hggb8fn9JSUlbW9vWrVuHDRuWticK9BxXIKG/qaioePrppxM/hmvvkBU4xYH+5pZbbsl0C4A1GEcAgKYYQQOApghoANAUAQ0AmiKgAUBTBDQAaOr/A6KIs1Z+O2xMAAAAAElFTkSuQmCC)

### Qualitative vs Quantitative Data

One thing to always keep in mind is the type of data which you are  trying to create graphs for. In general, we categorize data in two big  groups: Qualitative data (also called Categorical data) and Quantitative  data (also called Numerical data).

What we refer to as **qualitative or categorical** data  is data that refers to, as seen from its name, categories. This can  include data for "Yes or No" questions, it could be the name of a  location, it could be a person's favourite ice cream flavour, or it  could be something else. It's something very distinct from **quantitative or numerical**  data. Quantitative data is data that is, quite simply, numbers. It  normally is a measurement of some sort, and can be manipulated using  simple math.

The plotting methods and the best types of chart for each type of  data are different - choosing the best one will help you greatly in  creating visually pleasant graphs.

## Making Bar Plots

Let's start our plotting with bar plots. As the name implies, it's a plot format that shows your data using bars. You probably have seen a lot of them already.

Before actually creating any bar plot, let's import our plotting library, `ggplot2`. There's no need to execute this block if you already executed the import in "Differences between R Libraries".

```r
if("ggplot2" %in% rownames(installed.packages()) == FALSE) {install.packages("ggplot2")}
library(ggplot2)
```

Now that we have loaded our libraries, let's start plotting. To plot easily using `ggplot2`, we can use the `qplot` function, which has simpler syntax, like so:

```r
qplot(mtcars$cyl, geom = "bar")

```

![img](data:image/png;base64,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)

As we can see, we plotted a bar plot, consisting of the count of every element with the same value. We can now exploit some of the possibilities of `ggplot2`'s `qplot` function.

```r
?qplot

```

You don't need to understand how exactly each parameter of the `qplot` function works, but you can always go to the help file to try to find what you need.

Our graph is plain as it  stands right now. A plain graph is an excellent choice for academic  papers, but for Internet content… simply being gray will not catch  people’s attention. Let's give it some colour using the `colour` and the `fill` parameters. `colour` will modify the colour of the outline, while `fill` will change the colour of the bars.

```r
qplot(mtcars$cyl, geom = "bar", fill = I("black"), colour = I("red"))

```

![img](data:image/png;base64,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2KGU+u53vzt16tSysrI5c+ZcuHChc59PPPHE17/+9Q0bNsRisW9+85tlZWVTpkyZPXu2Uqqjo+Oee+7ZuHFjVVXVtm3bZs6cmblV1s5XrVr10EMPZf7p7NmzN9xwgw9v2IiBxbuX1gPyQin14osvuq77yiuvRCKRP/7xj67r/vznP//+97+fuYJpmolEwnXdc+fOjRgx4q233nJdN5lMXrhwIbMxc7Vnnnmm8xVTlVK/+c1vMpe3bt361a9+NXP54sWLrut2dHQMGzbsz3/+82OPPdY5RvedNzY23nDDDc3Nza7rLlu27NFHH81cMxgMxmKx/P2HYOAg0JBOKZXp3YkTJ4qKijIbd+/eXV5enrncGejXXnvti1/8YtbN161b97nPfa6ioqKsrGzWrFmd+2xtbc1cPnHixMiRI+fPn//KK6+0tLR07v+uu+4aMmTIl770pb17915u5/fff/8vf/nLRCLxyU9+sr6+PrORQMMrPMWBq0Dm+VzTNDuf2DVNM5lMZl0t83riXe3bt2/NmjVbtmzZtWvXsmXLuv7srvOFBkeOHFlXV3fHHXfs2LGjrKws8zRFeXn5G2+8MW/evEWLFlVWVqbT6e47V0otXLhw3bp1W7ZsGTduXGlpqUefLvBfBBpXvSFDhly8eFEpVV5efuDAgb/+9a9KqcyzEOfPny8uLh42bJhS6ne/+13Om58+fVopVVlZuXr16tbW1g8++CAWix05ckQppbW+7bbbOjo6UqlU950rpSZOnFhUVPToo492PhkNeIhA46q3aNGiioqKyZMnRyKRzZs3P/zww5/61KemTJly8ODBmTNnlpSU3Hnnnd/5zndKSkpy3vzw4cPl5eWTJk369Kc//dBDD918882pVOqxxx6bPn36yy+//IUvfOH555+3bXv48OFZO8/cvLq62jCMu+66y8fPGAMFv2YHXNbixYtXrVp15etUV1ePHTt28eLF/oyEAYVH0MBljRs37gr/+v77748dO/bdd9/l+Q3kCY+gAUAoHkEDgFAEGgCEItAAIBSBBgChCDQACPX/xZP0TNYGBl4AAAAASUVORK5CYII=)

We can just change the fill, as the outline, if no parameter is passed, will receive the same value as the fill one. You can change the colors to blue, pink, green, yellow... And there's more colours! Here's a list: <http://sape.inf.usi.ch/quick-reference/ggplot2/colour>

We can also change the name of our axes to make it more easily understandable by passing the `xlab` and `ylab` parameters (`lab` stands for "label"):

```r
qplot(mtcars$cyl, geom = "bar", fill = I("blue"), xlab = "Cylinders", ylab = "Number of Vehicles")

```

![img](data:image/png;base64,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)

To finish our bar plot, we can give a name for our graph. We can do this using the `main` parameter.

```r
qplot(mtcars$cyl, geom = "bar", fill = I("blue"), xlab = "Cylinders", ylab = "Number of Vehicles", main = "Cylinders in mtcars")

```

![img](data:image/png;base64,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)

------



## Histograms

 Histograms can be defined as a graphical visualization of data counts. It is a particular type of a bar plot. A histogram shows the distribution of a quantitative variable. Normally, bar plots are used to compare variables. Usually, there's no space between the columns of a histogram.

Let's make a simple histogram, selecting the horsepower column from `mtcars`.

```r
qplot(mtcars$hp, geom="histogram")
`stat_bin()` using `bins = 30`. Pick better value with `binwidth`.

```

![img](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAeAAAAHgCAMAAABKCk6nAAACNFBMVEUAAAADAwMGBgYHBwcJCQkKCgoLCwsPDw8QEBARERESEhITExMUFBQVFRUWFhYYGBgZGRkbGxsdHR0eHh4fHx8hISEiIiIjIyMmJiYnJycpKSkqKiorKyssLCwtLS0uLi4vLy8xMTEzMzM1NTU2NjY3Nzc4ODg7Ozs8PDw9PT0+Pj4/Pz9AQEBCQkJDQ0NERERFRUVHR0dISEhJSUlLS0tMTExNTU1OTk5PT09QUFBRUVFTU1NWVlZYWFhZWVlaWlpdXV1fX19gYGBjY2NlZWVnZ2dpaWlqampra2tvb29wcHBxcXFycnJzc3N0dHR1dXV2dnZ3d3d4eHh5eXl6enp7e3t8fHx9fX1+fn5/f3+AgICBgYGDg4OGhoaHh4eIiIiJiYmKioqLi4uMjIyUlJSVlZWXl5eYmJiZmZmbm5ucnJydnZ2goKChoaGkpKSlpaWmpqaoqKipqamqqqqrq6usrKytra2urq6vr6+wsLCxsbGysrKzs7O1tbW4uLi5ubm7u7u8vLy+vr6/v7/AwMDBwcHCwsLDw8PExMTFxcXHx8fIyMjJycnKysrLy8vNzc3Q0NDR0dHS0tLT09PU1NTX19fY2NjZ2dna2trb29vc3Nzd3d3e3t7f39/g4ODh4eHj4+Pk5OTl5eXm5ubn5+fp6enq6urr6+vs7Ozt7e3u7u7v7+/w8PDx8fHy8vLz8/P09PT19fX29vb39/f4+Pj5+fn6+vr7+/v8/Pz9/f3+/v7////YBpEKAAAPzUlEQVR4nO2d+XucVR1HU9SiFFBEBRTaWjYFVHADpVRUQFCkpMS4tBRQoYKCCwhdFAqCLWVXNtm3rtmapM12/zkn8zYl7/d75/ZuYW7envND2ieTnHzuPc9M2+dhtMdAo+np9gBYWAjccAjccAjccI4RePRgZ8Ydj3lz2PUTfGGJprXEJ/C+vZ0ZczzmzdRABkmeJYMZJEUtIXANAlsU6RBYQ2BJUdeaDoElRV1rOgSWFHWt6RBYUtS1pkNgSVHXmg6BJUVdazoElhR1rekQWFLUtaZDYElR15oOgSVFXWs6BJYUda3pEFhS1LWmQ2BJUdeazsIHfrm//0ECx1DUko6BD68d4xkcR1FLOgZ+fv3tG95o/To2NLTPwbjrQV+mBjNImrbEee2etJZ0DPzYj8ff/2nr195Vqwbdf0RDwYy2P9oCP3ubMddOt3/bgJfoNTUcS46fl+jhn80MX28InHuJLwv/t+jt/eueJ3D2Jb7w72AJgTUEVksIrBXpEFhDYAmBNQRWSwisFekQWENgCYE1BFZLCKwV6RBYQ2AJgTUEVksIrBXpEFhDYAmBNQRWSwisFekQWENgCYE1BFZLCKwV6RBYQ2AJgTUEVksIrBXpEFhDYAmBNQRWSwisFekQWENgCYE1BFZLCKwV6RBYQ2AJgTUEVksIrBXpEFhDYAmBNQRWSwisFekQWENgCYE1BFZLCKwV6RBYQ2AJgTUEVksIrBXpEFhDYAmBNQRWSwisFekQWENgCYE1BFZLCKwV6RBYQ2AJgTUEVksIrBXpEFhDYAmBNQRWSwisFekQWENgCYE1BFZLCKwV6RBYQ2AJgTUEVksIrBXpEFhDYAmBNQRWSwisFekQWENgCYE1BFZLCKwV6RBY81EGHh3rzKTjMW9mDo2N1RNESJxLfO2zS5LJcifTeZYMFfMM9n2OxS3hGUzgagmBtSIdAmsIHLSEwASulhBYK9IhsIbAQUsITOBqCYG1Ih0CawgctITABK6WEFgr0iGwhsBBSwhM4GoJgbUiHQJrCBy0hMAErpYQWCvSIbCGwEFLCEzgagmBtSIdAmsIHLSEwASulhBYK9IhsIbAQUsITOBqCYG1Ih0CawgctITABK6WEFgr0iGwhsBBSwhM4GoJgbUiHQJrCBy0hMAErpYQWCvSIbCGwEFLCEzgagmBtSIdAmsIHLSEwASulhBYK9IhsIbAQUsITOBqCYG1Ih0CawgctITABK6WEFgr0iGwhsBBSwhM4GoJgbUiHQJrCBy0hMAErpYQWCvSIbCGwEFLCEzgagmBtSIdAmsIHLSEwASulhBYK9IhsIbAQUsITOBqCYG1Ih0Caz6CwG9e/jqBY1gsge9YR+AoFkngF+/bOBv4he3b9w935rDjMW+mR4eH6wkiJM4lvvbZJclku5NkDg8f6Bx4/Wg78N3XXTcw0Zlpx2PezExOTNQTREicS3zts0uSyXYnyUxPjHQMvOsBs5GX6CgWx0v0X/p+ffXaIQLnXuLLR/HPJJ7BcSyawHMQOOMSXwgctITABK6WEFgr0iGwhsBBSwhM4GoJgbUiHQJrCBy0hMAErpYQWCvSIbCGwEFLCEzgagmBtSIdAmsIHLSEwASulhBYK9IhsIbAQUsITOBqCYG1Ih0CawgctITABK6WEFgr0iGwhsBBSwhM4GoJgbUiHQJrCBy0hMAErpYQWCvSIbCGwEFLCEzgagmBtSIdAmsIHLSEwASulhBYK9IhsIbAQUsITOBqCYG1Ih0CawgctITABK6WEFgr0iGwhsBBSwhM4GoJgbUiHQJrCBy0hMAErpYQWCvSIbCGwEFLCNxm7OgHAidQbuCLZz+sJHAipQaenrxocnJy75kETqTUwOuX9CxZsuSkDQROpNTAxqzjL1nNDmzMxPj4OIETKTfw5tM/sXTpUgInUm7gVW/wEh3xk4OW+LIgga/iz+BmB751y2ECp1Nu4J42BE6k3MAdIHDGJb4QOGgJgdt8rA2BEyk38OTk5Ojf+gmcSLmB26xRgYcGO3PI8Zg30yODg/UEERLnEl/77JJkstzJ1MEMkkOD+v/i/b1zUwN7p1rTmajDeP+ozl/X8MDLli076TN/T32J9n6xdQSOezny/VGdv67hL9EDAwMjKi+Bsy7xZYH+DB4eJnAy5QZ+5dwTTjj/fwROpNzAl9w9PbXpawROpNzAy2c/fJHAiZQbeOUrxryU/F9VEjiDY2ECb1t22WUn/5PAiZQb2Hzw0EMfqL4EzrnElwUJ/K8BYw48QeBEyg18zpQxE8sJnEi5gVfMfuBv0amUG/iCZ4158jwCJ1Ju4CdOvfTSU3cQOJFyA5s9m7fsVX0JnHOJLwX/N1kEzuAgsM+S8E0EtigkBM7gILDPkvBNBLYoJATO4CCwz5LwTQS2KCQEzuAgsM+S8E0EtigkBM7gILDPkvBNBLYoJATO4CCwz5LwTQS2KCQEzuAgsM+S8E0EtigkBM7gILDPkvBNBLYoJATO4CCwz5LwTQS2KCQEzuAgsM+S8E0EtigkBM7gILDPkvBNBLYoJATO4CCwz5LwTQS2KCQEzuAgsM+S8E0EtigkBM7gILDPkvBNBLYoJATO4CCwz5LwTQS2KCQEzuAgsM+S8E0EtigkBM7gILDPkvBNBLYoJATO4CCwz5LwTQS2KCQEzuAgsM+S8E0EtigkBM7gILDPkvBNBLYoJATO4CCwz5LwTQS2KCQEzuAgsM+S8E0EtigkBM7gILDPkvBNBLYoJATO4Fj4wK/19vXtJnAMiyPw4LjZcSeBY1gcgVvs3ETgGBZL4IM3vNv6eF9v74FDnZnSn6pfpuN7HYEd3xWwJHzTzETETw5a4kumJcOdA0/0PzP7y9MPPrh/pDMT+lP1y3R8ryNw569zKLx/VOevmx5zSDz1tjsJJ3JJnYmRgY6BZ27fPvfbbr9EO3xxP6rz10W+MNbti+Mleufq/v57CezHYgw8DwIfCwJbIbADAh/roahNBLYoJASOcuRZUofAEgJbFBICRznyLKlDYAmBLQoJgaMceZbUIbCEwBaFhMBRjjxL6hBYQmCLQkLgKEeeJXUILCGwRSEhcJQjz5I6BJYQ2KKQEDjKkWdJHQJLCGxRSAgc5cizpA6BJQS2KCQEjnLkWVKHwBICWxQSAkc58iypQ2AJgS0KCYGjHHmW1CGwhMAWhYTAUY48S+oQWEJgi0JC4ChHniV1CCwhsEUhIXCUI8+SOgSWENiikBA4ypFnSR0CSwhsUUgIHOXIs6QOgSUEtigkBI5y5FlSh8ASAlsUEgJHOfIsqUNgCYEtCgmBoxx5ltQhsITAFoWEwFGOPEvqEFhCYItCQuAoR54ldQgsIbBFISFwlCPPkjoElhDYopAQOMqRZ0kdAksIbFFICBzlyLOkDoElBLYoJASOcuRZUofAEgJbFBICRznyLKlDYAmBLQoJgaMceZbUIbCEwBaFhMBRjjxL6hBYQmCLQkLgKEeeJXUILCGwRSEhcJQjz5I6BJYcn4FHxzozqT9Vv0zH9zoCd/46h8L7R3X+uplDDomn3nYn4UzHLakzOTYU+wx2xKkT912evvzP4AwnqT+DfReqJV7P4GPYE16iPVKEXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4ElBPY4YNy1RPkI7LYTWEJgjwPGXUuUj8BuO4Elx1Pgrb/65fsEjjjJIgm8b+3Mq7cSOOIkiyTwznuNuZbAESdZJIEffsCYa1q/9q5aNWh52CNFRdx3efqM4yHHD/b+wqiTxC2M45j20fZH1zN4bGhon4Nx14O+TA1mkDRtifPaPWkt6Ri49WfwKxuP/NbxGjHmeMybqYEMkjxLvF4Yj0FRSzoGNlv7+x1/i56nSIfAmoUPPO/J7FakQ2ANgSVFXWs6BJYUda3pEFhS1LWmQ2BJUdeaDoElRV1rOgSWFHWt6RBYUtS1pkNgSVHXmg6BJUVdazoElhR1rekQWFLUtaZDYElR15oOgSVFXWs6BJYUda3pEFhS1LWmU0rgoQwz9m57PYMky5J/vJFBkmXJP1/LIBnyC7zgfP+/XR5wlCtf6PaCOVY/l1FG4DkIvCA8OdTlAUd50vafCHeFXQcyyrodGBYYAjecbgWeWnvVo2bubW4fvtmtC7zW29e3u4gl+9f+ovft3Eu6FXhm/18fnXub27w3u3WBwXGz484ilkzPmP/ckXtJ916iZwNXb5KZ92a37rBzUylLnr4r95LuBq7e5jb3ZrducfCGd8tY8k7fj97LvYRnsJnof6aQJca8fkuznsHV29zmvdmtC8zcvt2UsWTCmN035l7StcC3XfOTP8y9ze3DN7t1gZ2r+/vvLWLJi339vS/lXsK/gxsOgRsOgRsOgRsOgRvOcRR4/bTr0d7ZDw28jQYeqRNLJvXn5j617Rufv+SeRt5GA49Uo2fjijP+feM557xs1vVcdPHYExesWPm4+cGqFd870Hqs78rfj61e8eUrzOFPvtM79WbrM3es/MKW1i83XX3h5m4vz0TjA99j7l/6sPndD9vP4D2nPGWmBsweY269pfXYn1tP3SuMGTQTn3rs5vZXbzLPnd5+YN9nd3d7eh4aH3jcvLXMmJ0XtgNvvrT9ybu++pWV3249NmrMW5+77v6Drce/c+Jlu9pfbT4+YXpGjLl8a5eXZ6LxgY155zRjdp3fDrylHfjZMw+YrV8/cvaRrdefMfs/+nfzw6dMtz+zdNz0tF6/v7Wti6szchwFPmmv2XvqU2bywCMXG7PmSOB3R8yhT7899pLp3X3ixNHAvzWvnryn29PzcBwF3nDWyrEd531p+eNTa7655udHAj+yYvnZG8zIdy847ew/maOBf7PiLP6S1TBumvf7Jl1Kk86SxB/n/b5Jl9Kks4AFAjccAjccAjccAjccAjec/wNP5Vh+zaMw+QAAAABJRU5ErkJggg==)

As you executed the code, you may receive the following error message: `stat_bin()` using `bins = 30`. We can pick better value with `binwidth`. Binwidth defines the width of your bar. Let's further improve our histogram, changing our binwidth.

```r
qplot(mtcars$hp, geom="histogram", binwidth = 25)

```

![img](data:image/png;base64,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)

Ok,  now each bar has a width of 25 pixels. However, we can see that the  visualization of data between 210 and 260 hp are not well illustrated.  Again, let's add a black outline to the histogram to make it better to  visualize.

```r
qplot(mtcars$hp, geom="histogram", binwidth = 25, colour = I("black"))

```

![img](data:image/png;base64,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)

We  can also define limits for our x axis. R will fit automatically the  best values according to our data, so the result will not change when  you use qplot and an adequate limit.

```r
qplot(mtcars$hp, geom="histogram", binwidth = 25, colour = I("black"),xlim=c(50,350))

```

![img](data:image/png;base64,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)

If it happens to "cut" any value, R will display an error message saying how many values are not being shown. Let's play with xlim values, to see this message. You can put any value that you wish here.

```r
qplot(mtcars$hp, geom="histogram", binwidth = 25, colour = I("black"),xlim=c(80,200))
Warning message:
: Removed 12 rows containing non-finite values (stat_bin).Warning message:
: Removed 1 rows containing missing values (geom_bar).

```

![img](data:image/png;base64,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)

Now let's give a name for our axes. We use the `xlab` and `ylab` parameters to modify them.

```r
qplot(mtcars$hp, geom="histogram", binwidth = 25, colour = I("black"), xlab = "Horsepower", ylab= "Number of Cars")

```

![img](data:image/png;base64,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)

We can remove the color that fill our bars using the parameter alpha.

```r
qplot(mtcars$hp, geom="histogram", binwidth = 25, colour = I("black"), xlab = "Horsepower", ylab= "Number of Cars", alpha = I(0))

```

![img](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAeAAAAHgCAMAAABKCk6nAAAC01BMVEUAAAABAQECAgIDAwMEBAQGBgYHBwcICAgKCgoLCwsMDAwNDQ0ODg4PDw8QEBARERESEhITExMUFBQVFRUWFhYXFxcYGBgZGRkaGhobGxscHBwdHR0eHh4fHx8gICAhISEjIyMlJSUmJiYnJycoKCgpKSkqKiorKyssLCwtLS0uLi4vLy8wMDAxMTEyMjIzMzM0NDQ1NTU2NjY3Nzc4ODg5OTk6Ojo7Ozs8PDw9PT0+Pj4/Pz9AQEBBQUFCQkJDQ0NERERFRUVGRkZHR0dISEhJSUlKSkpLS0tMTExNTU1OTk5PT09QUFBRUVFSUlJTU1NUVFRVVVVWVlZXV1dYWFhZWVlaWlpbW1tcXFxdXV1eXl5fX19gYGBhYWFjY2NlZWVmZmZnZ2doaGhpaWlqampra2tsbGxtbW1ubm5vb29wcHBxcXFycnJzc3N0dHR1dXV2dnZ3d3d5eXl6enp7e3t8fHx9fX1+fn6AgICBgYGCgoKDg4OEhISFhYWGhoaHh4eIiIiJiYmKioqLi4uMjIyNjY2Ojo6Pj4+QkJCRkZGSkpKTk5OUlJSVlZWWlpaXl5eYmJiZmZmampqbm5ucnJydnZ2enp6fn5+goKChoaGioqKjo6OkpKSlpaWmpqaoqKipqamqqqqrq6usrKytra2urq6vr6+xsbGysrKzs7O0tLS1tbW3t7e4uLi5ubm6urq7u7u8vLy9vb2/v7/BwcHCwsLDw8PExMTFxcXGxsbHx8fJycnKysrLy8vMzMzNzc3Pz8/Q0NDR0dHS0tLT09PU1NTV1dXW1tbX19fY2NjZ2dna2trb29vc3Nzd3d3e3t7f39/g4ODh4eHi4uLj4+Pk5OTl5eXm5ubn5+fo6Ojp6enq6urr6+vs7Ozt7e3u7u7v7+/w8PDx8fHy8vLz8/P09PT19fX29vb39/f4+Pj5+fn6+vr7+/v8/Pz9/f3+/v7///+dnDTYAAARm0lEQVR4nO3d/X/V5X3H8XSbdbe2EbWixA7vys0UHevU4qQTVIpQitxoO60VdYMOS5M0ujmH1ULVaQVabUdtK1QlbE5nt85YsBvbbKXhxoIILBBIyM3J/bn+hJ3bL/le53vlOhffz8k5uXi9foB8k++5fMfn4xxRDKlS5HVV5R5ApQ1gzwPY8wD2vGKBE132eoq4Z8S6++Ke4MeGhMwGJ+BjR+0lirhnxI4PxT0h/oa2wfJvODEQ94TW7tQPAEcFsDmAhTYAXMINAJsDWGgDwCXcALA5gIU2AFzCDQCbA1hoA8Al3ACwOYCFNgBcwg0AmwNYaAPAJdwAsDmAhTYAXMINAJsDWGgDwCXcALA550+sZXe491q1d+x1/swAzlQhwHdV2fqu65EAZ6oQ4PmPha8LXqI/s9b1SIAzAWwMYHMAC20AWHCDHsDmABbaALDgBj2AzQEstAFgwQ16AJsDWGgDwIIb9E5X4O6EvYEi7gm18MnwdU9Su2H+M65HOm/Q69U3uBd7Q99Q7A39icQJnsFRna7PYIBHcQPAghv0ADYHsNAGgAU36AFsDmChDQALbtAD2BzAQhsAFtygB7A5gIU2ACy4QQ9gcwALbQBYcIMewOYAFtoAsOAGPYDNASy0AWDBDXoAmwNYaAPAghv0ADYHsNAGgAU36AFsDmChDQALbtAD2BzAQhsAFtygB7A5gIU2ACy4QQ9gcwALbQBYcIMewOYAFtoAsOAGPYDNASy0AWDBDXoAmwNYaAPAghv0ADYHsNAGgAU36AFsDmChDQALbtAD2BzAQhsAFtygB7A5gIU2ACy4QQ9gcwALbQBYcIMewOYAFtoAsOAGPYDNASy0AWDBDXoAmwNYaAPAghv0ADYHsNCGUgM319WtWJV+o2dRXd0OgEd9wyg8g1/akgGu4xl8Co0F4BXHMsBLa5/oTP188N13j7bZ6y3inlCfXRO+7hjSbrj1CdcjnTfodeob3Iu9oWsw7gntPW1tx0YAfv9rmZ+Snarx2dTPT82de2jQXrKIe0Itelp7h9KuF6xzPdJ5g96QvsG9+Btin5De0DUC8Auv599qf4CX6FHfUPqX6PtS+sk21ZNUTWsAHvUNJQdufiT1Q9cy9c7K+oYWgEd9A/8eLLhBD2BzAAttAFhwgx7A5gAW2gCw4AY9gM0BLLQBYMENegCbA1hoA8CCG/QANgew0AaABTfoAWwOYKENAAtu0APYHMBCGwAW3KAHsDmAhTYALLhBD2BzAAttAFhwgx7A5gAW2gCw4AY9gM0BLLQBYMENegCbA1hoA8CCG/QANgew0AaABTfoAWwOYKENAAtu0APYHMBCGwAW3KAHsDmAhTYALLhBD2BzAAttAFhwgx7A5gAW2gCw4AY9gM0BLLQBYMENegCbA1hoA8CCG/QANgew0AaABTfoAWwOYKENAAtu0APYHMBCGwAW3KAHsDmAhTYALLhBD2BzAAttAFhwg97pCtxexDfr6XH97j4l+L5Jzhv0BL5vUuwNpf++SYV1FFFfMTcN73Nrw9ddSe2GeU+5Hum8Qa97KO4J8TckBuOe0Nnb0XGcl+ioTteXaIBHcQPAghv0ADYHsNAGgAU36AFsDmChDQALbtAD2BzAQhsAFtygB7C5SgTe9ryl7+0LPwBgc5UIPPvSGSP30Q3hBwBsrhKBZz1tecDMdeFrgM0BHL3BOYCL3wAwwOFrgM0BHL3BOYCL3wAwwOFrgM0BHL3BOYCL3wAwwOFrgM0BHL3BOYCL3wAwwOFrgM0BHL3BOYCL3wAwwOFrgM0BHL3BOYCL3wAwwOFrgM0BHL3BOYCL3wDwScPu/QD7CzzvROfHz30UYG+Br1Sb/rJnEsDeAk9V9zaqyQB7C/y5eRd1dQDsL3Bi63514HWAfQUeeNZsC3DMDc6V4hk8H+BsvgI//MNugNP5ClyVCWBvgW0BfOobnAO4+A0A5wCP190yc+ZMgL0Fnrd6auOSrwDsLfBkda1StwPsLfA0dd1xNRtgb4GXtK67eAbPYH+BU/38XwcB9hS4vy39Y1s/wJ4Cf/Xr6R/XPpjF7FlUV7cj81bjQw8eAjjuBufkgScm0j92X54Drss9bVtXJXetBjjuBufkgWuyihfmgJfWPtGZfqNpo1L3ABx3g3PywBdlLg5dlMVMdqrGzO8Pv/Zjpe5O/bzhjjsOD9gbKuKeUIueDl8PKu2GBetcj9Q3zHne8oDZG7UNSde/pHWDczIbOocB189JCbfMejD4NVX7A8OfwXu3bz/abq+3iHtCLVgTvu5Iajfc+qTrkfqG2essD/jzb4evO4dc/5LWDc51DcY94URqw/Dvm9S3+MzLLz/z9tyvonuSqmmNSral/xnc/Cgv0XE3OFeKfw/etWnTrvzT952V9Q0tqmtZ6lfRDQ38Ktq5igS2BfCpb3AO4OI3AAxw+NpP4HaA8/kJfJX6IsDZ/AS+fNu0HekA9hT4hWt/d1o6gD0FVmoFL9HZfAVOfxN3gI/6C9x89RlnTN8NsLfA139naHD9DQB7C5z52u/LAPYWeGqzUjunAuwt8NbqWbPOfhVgb4HV4VdeOWz2BTjGBuf4zYbiNwAMcPgaYHMAR29wDuDiNwCc9eOPUcrnKTB/jFI+X4H5Y5Ry+QrMH6OUy1dgWwCf+gbnSgLcO8LvFQIca4NzpQB+Y8JE9bNFAHsLfNWBGUpdCrC3wFeqGfx+cDpfga/9vxnq1WsB9hb4zUnjrqveBrC3wKq1cctRsy/AMTY4VxLglsatRwD2F/jlc2655ZwtAHsLfOl7Su25BGBvgTNflsT/Vekv8ENPtbd/82GAPQWuquJ3k3L5CWwP4FPf4BzAxW8AOAf4q7+4Zvr06QB7Czzpm03btvGfKj0G5iU6m6/AK14DOJOvwD/9nerx48cD7C3wxzfvO3DgAMDeAk8Z+RUa4BgbnCsF8N8/1wNwOl+B+U+VuXwFtgXwqW9wDuDiNwCcA/xwJoC9BR4YGOje1ACwt8CZlpiBuxP2Boq4J9TCJ8PXPUnthvnPuB6pb7j525YH3Pjd8HWvvsE9578Pen1DsTf0JxInCoAPXs0z2NtncHV19Uc/9hLA3gK3tbV1mnkBjrPBOXngnbkA9hT43Ey/z3/J8hU4XeKxc+8H2FvggfUXLN3LP4N9BU6+OPGm/x6BF+A4G5yTB76iZuOv0wHsKXB1LoA9BbYH8KlvcA7g4jcADHD4GmBzAEdvcA7g4jcADHD4GmBzAEdvcA7g4jcADHD4GmBzAEdvcA7g4jcADHD4GmBzAEdvcA7g4jcADHD4GmBzAEdvcA7g4jcADHD4GmBzAEdvcA7g4jcADHD4GmBzAEdvcG6sAD8319IFy8MPKAC+YqrlhPn/YdkAcAmBF85bO3IfmRd+QAHwx6ZZTpj0lGUDwKUEXm15wAVW4IWWE24GODKAgwAG2DWA8wEcHcBBAEcHcBDAALsGcD6AowM4CODoAA4CGGDXAM4HcHQABwEcHcBBAAPsGsD5AI4O4CCAowM46HQE3lNbX9+SfqNnUV3dDoBdq3jg9h715rcywHU8g0+higdO1bQ+A7y09on0d3L4r5dfPtJpr1+7Xvy45QEXLghfdye1G85fbDlhzrOWDTett5xw43Ph68SQ5QH29A3OJQbjntDV19nZNgJw14oP0j8lO1Xjs6mfN9fWtvTaG9Sul6y1PGDCwvB1X1K7YfwSywlzN1g23PKc5YRZ3wtf9+sb3NM3OBd/Q19qQ4cZuL/h7eDl+gFeol2r+Jfo5GNvpH9sUz1J1bQGYNcqHrjptoaGjaprmXpnZX1DC8CuVTxwVAAXH8D5AI4O4CCAowM4CGCAXQM4H8DRARwEcHQABwEMsGsA5wM4OoCDAI4O4CCAAXYN4HwARwdwEMDRARwEMMCu+QL8wX9q/VK7vvkRy4z4wLMesmz41D9YTrAC79c/Tb23fm7ZsOOIZYNehQDfeeZZI/cb8y0z4gOff4ZtwxctJ1iBZ/+25S/xoQ9bbvitzZYNehUCvPhh7R36S1PNHMuM+MDnLrFsGPd5ywlW4Ou/YznhD+63bPiT71tO0AM4CODoAA4CGGDLCQAbAzg6gIMAjg7gIIABtpwAsDGAowM4CODoAA4CGGDLCQAbAzg6gIMAjg7gIIABtpwAsDGAowM4CODoAA4CGGDLCQAbAzg6gIMAjg7gIIABtpwAsDGAowM4CODoAA4CGGDLCQAbAzg6gIMAjg7gIIABtpzgB3DE9+a5fbX2jj7t+qK5lu/uE//7Jp13h2XDOXdaTrB+36Qb/tFywlkrLBv+9EXLCXql/75JhbUdL2jpI9o7erTrms8UPijUBfPD1yeGtBvOv81ywnm3WzaM+4LlhE9vCF93DGo3XP+85YSz/sqy4ZM/sJyg1zng+ICC2hLHj7fyEp2Ol2iALScAbAzg6AAOAjg6gIMABthyAsDGAI4O4CCAowM4CGDPgafeuDzUl78avl4+4XHLCVbgi+csH7m//lX4AQXAz1sOWL5yV/gBAAdVT7EAn/klywlW4N+7ysJz3o/CDygAvvJWywnjXgo/AOCg6rvC1wUv0R+JD/xlywlXW4E3WU6YArApgAG2nACwMYCzAWwM4GwAGwMYYMsJABsDOBvAxgDOBrAxgAG2nACwMYCzAWwM4GwAGwMYYMsJABsDOBvAxgDOBrAxgAG2nACwMYCzAWwM4GwAGwMYYMsJABsDOBvAxgDOBrAxgAG2nACwMYCzAWwM4GwAGwMYYMsJABsDOBvAxgDOBrAxgAG2nACwMYCzAWwM4GwAGwMYYMsJABsDONuoAzc+9OCh8BsAmxt7wK2rkrtWh94AeITGHnDTRqXuCb0B8AiNPeDXfqzU3cPf+Ntp0w4W3rasikapD1nvaCr06S7+GZw4caK1sEN7tA5r1zub9Tu03t0Vvv51q+UG6wkFG6wn/HJ3+HrfUcsN1hMKNlhP+IV2vf+I5YbCNJtjidQPRuDUP3qbH1XJttwbppfogvSXJucKXqLdi72h4CW6DBtK/udFNzY0HFJdy3JvADzaGyrkDwQvCGChDQCXcAPA5gAW2gBwCTcAbA5goQ0Al3ADwOYAFtoAcAk3AGwOYKENAJdwA8DmABbaAHAJNwBsDmChDQCXcAPA5gAW2gBwCTcAPMKuuLP2bYl7QvwN7/1T+Tc0/0vcE1rTG5yAR6W9N5Z7gVL/89lyL1DqrS/InQWwFsAlrOun5V6gVPtb5V6gVOt2ubMqCpjkA9jzKgJ4cNXin6j8l7qd/IK3UW1PbX19S5k3HFv1tdr9whsqAjh57MWf5L/UbdgXvI1q7T3qzW+VecNQUv3v48IbKgJYqTRw9gtlhn3B22jXtL78G7avE95QQcDZL3ULvvJt1Ota8UG5Nxyov/Og8IYKAi7zs6e/4e2yb1Bqb52/z+Dsl7oN+4K3US352Buq3Bv6lWpZKbyhMoC/fvd9G/Jf6nbyC95GtabbGho2lnnDL+obancKb6gMYCpZAHsewJ4HsOcB7HneA1e/k/ph/I5yzyhbpyHwgOMJrvdXVqcN8Kt/NPmG3anPt37BM4nbplxxq1JvferKq/8t9Z6vfP6aLSr38fX3qe1Vb6t7NwQfTd1f7k8hVv4Dn19TU/ObOw6f3aw2/HHq8/2hUltTuu3q2OTD6v0Jven3tF7Ykvv47kvU6k8+qi7eM+yjYzv/gbPP4FdmKTV4Roeq6lZqX829m7tU47gZM2ZM3K2qOpWa25j/+IQDM//90+/XnPxod7k/gZiddsDp93U23v+H3Vuuy95QdVypm7bmP37nuknqE+vuUsFHyzRbrDH/CdjKAR+u3qnWT89+vh90qt7z9h+tfk2pn6Xe8w216+wj+Y+/UHOP+lLND1Tw0XLvj9uY/wRs5X+R9c9TL/uz3dnP9/Upkz/xdym+ay6buDD1nr+ZcknqF1m5jx+s2qw2VR06+dFy74/bmP8EYuf53wHPP70i8vzvgOefHgHseQB7HsCeB7DnAex5/w+KDIq+Yi3ubgAAAABJRU5ErkJggg==)

As we did with the bar plot, we can give a name for our graph. We can do this using the `main` parameter.

```r
qplot(mtcars$hp, geom="histogram", binwidth = 25, colour = I("black"), xlab = "Horsepower", ylab= "Number of Cars", alpha = I(0),
     main = "Histogram")

```

![img](data:image/png;base64,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)

**Expert Tip: Sharpening your qplot skills**

 Do you want to check all the qplot function parameters? Click 

here

 to access the function documentation ! 



------



## Pie charts

A  pie chart is a circular graph, most commonly used in business. It shows  the proportion that each part of data contributes to an overall total.  This is usually done as a representation of the counts of qualitative  data, like demographics. 

**Expert Tip: Choosing the right chart type**

 Unsure which type of chart to use for your data? Click 

here

 to learn more ! 



A pie chart in  ggplot2 is a transformed stacked bar plot. A stacked bar plot is a plot  that stacks all the values on the vertical axis, instead of creating  separate bars for each different data point. Let's start by creating a stacked bar plot.

```r
barp <- ggplot(mtcars, aes(x=1, y=sort(mtcars$carb), fill=sort(mtcars$carb))) +
        geom_bar(stat="identity")
print(barp)
```

![img](data:image/png;base64,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mZWVpW389NNP09PT77jjjszMzIqKCm2joigLFiwYN25cXl7e/PnzXS5XZmbmPffc09DQsHr16oceesiz27Jly1JTU7t3775z5865c+f26tWrV69e33zzjRCiyYE7duzo379/ampqWlpaUVGREGLSpEkZGRmpqaljx46tqalp3nTzgi9evDh58uS1a9dOmDBh27ZtmZmZ2lGtOLm25dlnn73rrrtuu+22jz/++D/7qKrq9eU7ffr03r17FUXp16/f9ddf78c3xm63OxyOFu6c+dt8PzYNoIW+WD6l5TvHxcX5ev5NmzatWbNGS6J///vfMTExJ0+e7NWr1+7du3v06PHGG2+sWbNm3759QghFUd59992JEydqB1osFofDYbFYhBA33HBDSUnJTTfdpO22evXqRx99dMOGDVOnTi0sLBw+fPhLL710+PDh/Pz8Sw88c+bM7bffvmnTpr59+7pcrrq6uuuuu+7MmTNa0C1durSurm7JkiVNmm5esNPpvOGGGwoLCz/77LPc3FytvNadXPt15cqVv/nNbyorKwcMGHD48OH4+HjvV3F8+OGHvXr1euONN/Ly8lJSUjxxDgB+cccddxw4cGDmzJkbNmzQ0nbPnj133XVXjx49hBCPPvrogQMH6urqtJ09XexLOZ3O06dPd+rUybNl0qRJQog+ffpYrdbhw4cLIfr16+fpiXvs3r07LS2tb9++Qgiz2XzdddcJIQoLCwcPHnz33Xe///77hw4d8uzsabp5wWFhYZs2bfrd736Xl5c3YsSIvXv3tvrkmqlTpwohunXr1rt3b+1s3gN6wYIFe/fu3bx58+bNm4uLi/0yBA4AHj/5yU/KyspGjBhRVFSUmppaX19/lZ0jIyObb7RYLFqn2LPFarUKIcxms/ZAe9x8hLf513ElJSUrV6785JNPdu7cuWjRokvP6Wnaa8EDBw7ctGnTjBkznnrqqTFjxrjd7tadvDntPN4DOioq6uabb9Yed+vWzfNsAcAv/vnPfwohxowZ89JLL/3www9nz57t379/SUmJdknG6tWr09PTo6Ojmx8YExNTW1srhFAU5bbbbjt69GgLW/QcOHDgwIMHD2rjJ42NjTU1NefOnUtISOjQoYMQ4r333mthwQ0NDVq1iqKkp6dfvHjR5XK17uSaP/7xj0KIysrKL7/8sl+/fuJK10GPGjXqlVde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OjfpUw86feyTAS0GgFdfffRyy3eOi4sLXCWhjBtVAEBSBDQASIqABgBJEdAAICkCGgAkRUADgKQIaACQFAENAJIioAFAUgQ0AEiKgAYASRHQACApAhoAJEVAA4CkCGgAkBQBDQCSIqABQFIENABIioAGAEkR0AAgKQIaACRFQAOApAhoAJAUAQ0AkiKgAUBSBDQASIqABgBJEdAAICkCGgAkRUADgKQIaACQFAENAJIioAFAUgQ0AEiKgAYASRHQACApAhoAJEVAA4CkCGgAkBQBDQCSIqABQFIENABIioAGAEkR0AAgKQIaACRFQAOApAhoAJAUAQ0AkiKgAUBSBDQASIqABgBJWfRv0mw2W61W/dsF0HJ8SGVgQEC73W6n06l/uwBajg+pDAwIaFVVXS6X/u0CaDk+pDJgDBoAJEVAA4CkCGgAkBQBDQCSIqABQFIENABIioAGAEkR0AAgKQIaACRFQAOApAhoAJAUAQ0AkiKgAUBSBDQASIqABgBJEdAAICkCGgAkRUADgKQIaACQFAENAJIioAFAUgQ0AEiKgAYASVmMLuBHNNScMroEADAGPWgAkBQBDQCSIqABQFIENABIioAGAEkR0AAgKQIaACRFQAOApAhoAJAUAQ0AkiKgAUBSBDQASIqABgBJEdAAICkCGgAkRUADgKQIaACQFAENAJIioAFAUgQ0AEiKgAYASRHQACApAhoAJEVAA4CkCGgAkBQBDQCSsgTipBs3biwtLVVVNTs7OyEhIRBNAEDQ838Purq6eteuXc8999wjjzySn5/v9/MDQIjwf0AfOXIkJSVFUZTk5OSqqiq/nx8AQoT/hzjsdntkZKT22O12e7YfPnx406ZNQojhw4fffvvtfm8XgB/ZbDajS0AAAtpms506dUp7bDL9t4ceGRl54403CiGsVqvL5Wrh2ar2feKXqsxmsxCi5e36kdlsDg8Pb2ho0L9pIUR4ePjFixcNadpqtTY2NjY2NurftMlkMplMRjVttVrr6+v1b1r49e025MOCJvwf0D179vzkk09UVT169GjXrl0927t169atWzchhN1u1z+twsLChBBOp1PndrWmLRaLUQFtMpmM/bfhwoUL+jdtsVjMZrNRTRv477FRb3dUVJT+jYYC/wd0x44dBw0atHDhQiHEzJkz/X5+AAgRAbnMbsyYMWPGjAnEmQEgdHCjCgBIioAGAEkR0AAgKQIaACRFQAOApAhoAJAUAQ0AkiKgAUBSBDQASIqABgBJEdAAICkCGgAkRUADgKQIaACQFAENAJIioAFAUoqqqkbXEORKSkpWr179+uuvG12I3p5++unRo0ffc889Rheiq6NHjz777LMFBQVGF4JgQA864BobG9ufhE8AAAM5SURBVI1aQtRY9fX1hiwCaSyXy2W3242uAkGCgA64qKioSxfPDR2JiYnt27c3ugq9Wa1WbXFkoO0Y4gAASdGDBgBJBWRV79C0cePG0tJSVVWzs7MTEhI828vLy/Pz84UQ9fX14eHhy5cvdzgcU6ZMSUpKEkJMmDAhLS3NqJrbyOVyzZ8///jx49OnT8/MzGzy1+YvyJVeomvOVZ54ZWXlm2++aTabhRBPPvlkfHx80LzdMIAKfzh79uy8efPcbnd5efmSJUu87vPBBx989NFHqqo2NDTMnz9f3wIDwu12V1dXv/fee9u2bWvyp+YvSEteomvFVZ54bW1tQ0ODqqo7d+589dVX1SB6u6E/hjj848iRIykpKYqiJCcnV1VVed1n586dgwcP1h5XVVXl5OSsWrXqmv7GX1GU2NhYr39q/oK05CW6VlzlicfExFitVm0frR8tguXthv4IaP+w2+2RkZHaY7fb3XyH48eP22w27VMdERGRl5e3bNmypKSkdevW6VqoXpq/ID/6EgWTH374YcOGDaNHjxah8XYjQAho/7DZbJ6LnU0mL69qUVGRp/usKIrNZhNCDBkypLKyUrci9dT8BfnRlyhoOJ3OZcuWTZo06cYbbxSh8XYjQIL5c6Knnj17lpWVqapaXl6uXfWsqmptba1nhz179gwcOFB77HA4VFUVQpSVlV3T35U153nWzV+Q5luCieeJq6q6cuXKIUOG9O7dW/tTEL/dCDSu4vCPjh07Dho0aOHChUKImTNnCiHq6+vnz5//2muvCSHKy8s7d+4cFRWl7VxRUbF27Vqr1WoymWbPnm1g2W2Xm5tbWVkZFhZWWVn52GOPeZ518xek+ZZr2pWeeHFxcWlpaV1dXVFRUXJy8uTJk4Pp7YbOuFEFACTFEAcASIqABgBJEdAAICkCGgAkRUADgKQIaPjf008/ffPNNyuKsnfvXqNrAa5hBDT8Lysra8eOHcxbD7QRN6rA/wYNGmR0CUAwoAcNAJIioAFAUgQ0AEiKgAYASTFZEvxvzpw5H3744cmTJ2NjYyMjI7/77jujKwKuSQQ0AEiKIQ4AkBQBDQCSIqABQFIENABI6v8DWIwAid1tnxUAAAAASUVORK5CYII=)

Now we need to transform this graph into a pie plot. We are going to plot our stacked bar graph in the polar coordinates system.

A really nice refresher abour polar coordinates can be seen in the following gif:

<img src="https://ibm.box.com/shared/static/me1bmbb54gneyr5epweqe88zg8ujkqst.gif"

Source: [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Cartesian_to_polar.gif)

We use the `coord_polar` helper function to do so:

```r
barp <- barp + coord_polar(theta='y')

print(barp)
```

![img](data:image/png;base64,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euiALcu6+uqrH3nkkcsuu+z//u//6rdm9XFx+plvfetbp59++sknn/yzn/3s0GNSc5odvQVXXIeLhiGWw/BCOuUuwNPsENAjaOqIO/ot09fX1/qRNT5Os1u3bt3KlStpEvX393d0dOzbt+/UU0/99a9/feKJJ/7nf/7nypUrX375ZTrOH//4x1dccQV9oiiKhmHQddxHHXXU5s2bjznmGPqwhx9++LrrrluzZs211167du3aCy+88P7773/jjTfofVDrT9y/f/8pp5yybt26s846y3GcUqnU2dm5f//+MWPGEEKWL19eKpXuvvvuQS89dMC1Wu2oo45au3btM888c++999Lh+bs4/e0DDzzwD//wDzt37vybv/mbN954Y+zYsempoBVFsW07NelMYiqlGS+ikc4BomcnxVVET5s27bXXXrvlllvWrFlD0/all146/fTTTzzxRELIdddd99prr5VKJfrgYW9OXavVPvjgg3HjxtU/c+WVVxJCzjzzTFVVL7zwQkLIrFmz6pV43a9//esZM2acddZZ5MNT4wkha9euPe+8884999yf/vSnr7/+ev3B9ZceOmBJktatW/fv//7vK1asmDdv3qZNm3xfnLr22msJIccdd9zHP/5xerVUBXQK+huDxNKVZjajkc6BizGgJ02atHXr1nnz5m3YsGH69On1W+INa9gbKoqiSIvi+mfoFnZBEOp72QVBGNrhHTodt3nz5gceeODJJ5984YUXli1bNvCa9ZcedsCzZ89et27dTTfddNttt1100UWu6/q7+FD0OikJaLp1tdmAZrl8HggLPKBBzU4V1mo1juNi2fa9d+9eQshFF110//33VyqVAwcOnH322Zs3b6ZLMh5++OGZM2fm8/mhT+zo6KC31uM47uSTT37rrbcafMX6E2fPnr1lyxbaP7Ftu7e39+DBg+PHj+/q6iKE/OQnP2lwwLqu09FyHDdz5kzLshzH8Xdx6gc/+AEhZOfOna+88sqsWbMIISnZjy9Jkm3bjPTTw0AzOrKu9IE/vhz9bbFGhvI5JLVajX77RPy6v//97++44w7P81zXXbhw4cSJEwkhjz766OWXX25Z1rhx4370ox8N+8TbbrvtnHPOUVX1pZdeuvjii9evX3/aaac18ooDn7h27dqvfe1r5XJZEITvfve7c+bMWbVq1fz587u6uiZMmPDB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vI0bNy5cuPDAgQOhjzlyiaygCboc6RJso2P4l0BN3RhBEKJIZ3896I+eZvetb32LfnDJJZf80z/90+jRowMbHDOSGtCO4yCg0ySCjD70QkjqEfE8H1FAu02fB324reH//d//HcCAmJTUgEYFDS1CUg8rmgY0wXGjjUlwQItiUgcPw4qsiB78ukjqASKroHHcaCOSmnGooFMprow+9OpI6ggraOK6BAF9JEnNOB896GfvuyacsUCQQl3U0egY2njtR6SThJ7b5K+2C2hU0ACHlYJDmppaY0ci7kGjgj6SBAe053mCIET0dgwiFG+j43AS2gDp6upyXde2bcuybNseVITu3r37scceo1sKvvSlL40ZM6ZWq910000TJ04khCxYsOCUU04Ja2Se2/SB/ZgkTBDHcURRRECnEpsZTSUrqavVqiRJkiSpqko339K8rtVqtm13d3d//etfVxTllVdeefrpp6+77jrHcSZOnHjnnXeGPTDPa3qZHW55lSS2bYuiaJpm3AOBNpWIpDZNs/49wnGcIAiiKEqSpGkaz/OdnZ2e5zmOo2kazfFarbZ3797ly5ePHTv28ssvz2azYY3M8wI5zS7dEhzQjuPIshz3KCAsLBfRgyQiqQkhnufZtm3btmEY9DM0r2u12hNPPHHHHXdkMplKpbJ8+fJsNrt+/frHH3/8qquuCmswzd/yqg0nCRM8z0Yr6KaegoUcycLCio6mJG75h+M4lUrlvvvuu+iii1RVtW3bcRxaNc+aNWv37t3hvbRHml7FgR50ktCVdlHdgRjikaA6eiBGauojLuHwPO/73//+rFmzpk+fTggRBKFarQqCwHHc9u3bx44dG97YUEE3IsEBTXtn9A1a3GMBGB4jSX04r7766htvvFGpVDZt2jR58uQbbrhh586dq1evVhSF5/lrrrkmxNf2PGxUOaIEBzQhxHEcQRAQ0OmW0CJ6EDaT+owzzjjjjDPox7IsO47zsY997J//+Z8jeOmgbnmVbskO6FqthhM52kE6MppiM6kJIaIoRnrvKLQ4GpDgSUJCiG3bkiQ19RTMEyZU4iYMjyjsGcVm9xDSNXYhDWYoH1u9UUEnTK1W43k+uvO3AELAQk3NcVzU0zleq4cl/fa3v7311ltpifbII49MmjQpwNExItkVNPFVRENCpa+IHiTGVXqiKLquG2Wh4+ewpI8u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)

We can use the `theme` helper function so that we don't warp the labels and axes with our transformation:

```r
barp <- barp + coord_polar(theta='y')
barp <- barp + theme(
    axis.line=element_blank(),
    axis.text.x=element_blank(),
    axis.text.y=element_blank(),
    axis.ticks=element_blank(),
    axis.title.y=element_blank())
print(barp)
```

![img](data:image/png;base64,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BKGgy7537tw5fDXrve997wsvvBDhwAR97nOfi3+ShXsN+r6fekCz5f+O40Q4tij9jYWQ0aNA+Zwjx3EKV0SzTdaGc/b+++9vNptnnXXWKIfHCeil9nfbv3//li1b9u7d+573vGfPnj3JnpxSmnpAV6e/MU/upTTAMmzbzneynWmaV1999bp1684777zLL7+cPflv//ZvGzZsWLt27ebNm3/605+yJwVB+Ku/+qsrr7xy165dn//8533f37x58yWXXGKa5u7du6+55prBy774xS+uW7fuLW95yyOPPPLZz352zZo1a9asOXToECFk3oEPP/zwhRdeuG7duvXr1z/00EOEkI9+9KNvf/vb161bd8UVV8zMzCx864UDdhznYx/72D//8z9/+MMf/o//+I/NmzezoyKcnD3zhS984fzzzz/nnHO+973vvfGapaJzdnY2kU1BG42G53nRNoAubgU9bOXb3pHP+579zjRO+8BN70/kPCifE/STe26PcNSKFStmZmYS+dS/cuXKcQ/Zv3//nj17WBLNzc21Wq3XXnttzZo1P/rRj84888x/+qd/2rNnz5NPPkkIEQThzjvv/MhHPsIOlCTJsizWnzn55JMPHDhw2mmnsZft3r37uuuuu/vuu6+99tp9+/Zt3br11ltvffbZZ++4447hAw8fPvy7v/u7+/fvf+c73+n7fqfTmZiYOHz48EknnUQIueWWWzqdzs033zzvrRcO2HXdk08+ed++fffdd9+XvvQlNrxoJ2e/ve222/78z//8pZde+r3f+71nn3121apVWVTQVetvzJNXKV2URgfkJd99OdauXfv0009/8pOfvPvuu1naPv744+eff/6ZZ55JCLnuuuuefvrpTqfDXjwosYe5rvv666+vXr168MxHP/pRQsgFF1ygadrWrVsJIRs3bhxU4gM/+tGP1q9f/853vpMQQimdmJgghOzbt+9d73rXxRdf/O1vf/uZZ54ZvHjw1gsHLMvy/v37//7v/37Xrl3btm174oknIp+cufbaawkhb37zm9/xjnews6Ub0LIsB0EQbf+NkkG7YxjK52RFvlQoy3LigxnRGWec8dxzz23btu2hhx5at25dv99f5sW1Wm3hk2z74uH919g2I5TSwX4jlNKFnYCFl+MOHDhw22233XvvvY888sjOnTuHzzl460UHvGnTpv3793/i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CupRyLKsqqqiKGEYossMZYKA5kUQBKzoEwSBJY5hGL7vO45j2zY2hViI/TxTFMXzPMdx5ubm8LcEJYOA5g4rAx3HYb1URVF0XWcZNPrdpstKFEVZllkrg/1FocUMJYaA5tegkSoIgqIorFUtiqJ7TEWCafC/z+7lyn5WoY8BVYCALoAwDG3bZjM9KKUsqnRdJ8f6167rluzTPevzMJIksVDudrue5+G6H1QHArpgfN9ns3oJIZIksQ/7hmEQQjzP8zzP9332IO+RjkcURekYSimllPXf+/2+67oIZagmBHSBsSBmd56mlLJ0Yzd5Ya2AQWTzNsNaEASWyINhDwbsOA77GYNQBkBAlwRL4cFK8UFBqigKK0jDMAyCgCX18H9TDW4WxJTSef8VRZG9NUvkUbaRAqggBHQ5BUHApoIMnhmOSEqpoijscXhMEATzHjAnfC+WwsIxg8fsAQti9sPAdV02ZZC9RZp/AQBlgICuiqWKZRaj81JVEARKKXswyplZlPu+v2jWp/B/A1AJCOiqY6ldskkgAOUg5j0AAABYHAIaAIBTCGgAAE4hoAEAOIWABgDgFAIaAIBTCGgAAE4hoAEAOIWABgDgFAIaAIBTCGgAAE4hoAEAOIWABgDgFAIaAIBTCGgAAE4hoAEAOCXghhcAAHxCBQ0AwCkENAAApxDQAACcQkADAHAKAQ0AwCkENAAApxDQAACcQkCXzc6dO4MgGPz2ve997wsvvBDhwAR97nOfi38SQRDmPeP7/gUXXHD48OH4JwfgEwK6PDzPI8fn7P33399sNs8666xRDo8T0OytF9q/f/+WLVv27t37nve8Z8+ePcmenFL6J3/yJ1/84hejnRagAELgUr/f//CHP7x27doNGzZ88IMfZE/+67/+6/r169esWXPppZe++OKL7ElCyE033fShD33oa1/7GqtV3/Wud7373e9mZ7j77rsHL7vlllvWrl375je/+eGHH/6Lv/iLc88999xzz33hhRfCMJx34EMPPbRx48a1a9euW7fuhz/8YRiGH/nIR84///y1a9defvnl09PTC9964YBt256YmHjllVf+8i//0vO8l19+mR0V4eTst3/zN39z3nnnnX322ffccw97zezs7EknneR5XtpfDoBcIKA59S//8i+DXJ6dnQ3D8NVXX125cuWhQ4fCMNy1a9cFF1zA/pQQcueddw4OpJS6rsser1q16he/+MXgZbt37w7DcO/evYZh3HfffWEY/t3f/d0f/uEfzjvw9ddfP+mkk5544okwDD3Pm5mZYU+yl918882f//znF771wgE7jjM5Ofnggw/eeOONg+FFOzn77W233RaG4U9/+tNVq1b95je/Yc+fe+65Bw4cGPvvF6AIENCc+vnPf37GGWf82Z/92d69e7vdbhiG3/3ud7du3cr+1PM8RVHa7XYYhoSQXq83OHCQs47jEEIcx2HPE0JM02RnXrFiBXvy0Ucf3bRp07wD77nnni1btswbzz/+4z9efPHFF1100bp16973vvcNzjl464UDZud///vf32q1tm7d+vjjj0c+Ofsty/0wDN/3vvfde++97PGWLVsGBTVAyaAHzakzzjjjueee27Zt20MPPbRu3bp+v7/Mi2u12sInJUmSJMmyrMEzmqYRQiil7AF7vLDDu/By3IEDB2677bZ77733kUce2blz5/A5B2+96IA3bdq0f//+T3ziE9dff/1ll10WBEG0ky80OI9lWbquL/UygEJDQHPqV7/6FSHksssuu/XWW3u93pEjRy688MIDBw6wKRm7d+/esGFDo9FYeGCr1ZqdnSWECIJwzjnnvPjiiyO+4+DATZs2HTx48MknnySEsC7E9PT0KaecMjk5SQi56667RhywaZpstIIgbNiwwXEc3/ejnZz5+te/Tgh56aWXnnrqqY0bN7InDx06tGbNmhH/HwGKRcp7ALC4559//oYbbgjDMAiCHTt2nH766YSQb3zjG9dcc43jOKtXr/7mN7+56IHXX3/9RRddpGna448/fvnll99///3nnXfeKO84fOC+ffs+/elPd7tdSulXv/rVzZs333HHHdu3b5+cnDz11FNff/31UQbc7XZvvPHGw4cPv/LKK9///vdvv/12WZZXrlwZ4eRMu91ev369ZVm7du066aSTCCEHDx78nd/5nVNPPXWkv1OAosF+0GX22muvbd++/cCBA5TSHIdxww03fOUrX0njzDt27LjkkkuuuuqqNE4OkDu0OMps9erVN91008svv5zvMM4+++w0Tuv7/hlnnIF0hhJDBQ0AwClU0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKcQ0AAAnEJAAwBwCgENAMApBDQAAKf+P5etwh9Lp94HAAAAAElFTkSuQmCC)

You can notice that we still have an outline around our chart. We can extend the theme function using the `panel.background` parameter:

```r
barp <- barp + coord_polar(theta='y')
barp <- barp + theme(
    axis.line=element_blank(),
    axis.text.x=element_blank(),
    axis.text.y=element_blank(),
    axis.ticks=element_blank(),
    axis.title.y=element_blank(),
    panel.background=element_blank())
print(barp)
```

![img](data:image/png;base64,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eXyOJWSU1neIBpBIeqD1IqHRemF8BlIg0C7zfZRmiDaKgbscixYtikQi0R9vv/32/fv3Z3Cgix5//PHsT5KXlxf3SDgcFh1oXfY3EtFoJxifkZb29nbVsbObN2/u2bPnDTfc4OTwbAJtv3Si2trayZMn19TU3HrrratXr3b35KFQSHSgteb7KA1I1tLSct9995WVlY0aNWr69On2g3/729/Ky8tLS0srKys//vhj+8G8vLxf/epXM2bMWLly5RNPPBEOhysrKydOnNjS0rJq1aqZM2dGn/bUU0+VlZVde+2127Zte+yxx0aMGDFixIgDBw4opeIO3Lp167hx48rKykaOHLllyxal1KxZs2688caysrK777775MmTiS+duOC2trYHHnjgL3/5y7333vvWW29VVlbaR2VwcvuRJ598cvTo0cOGDXvttdcuPseyLG//O2RB3wk6Vp/rb/LndYfe7MVp31441ZXzMD676Mi2dX4vIW21tbWrV6+2S/T1118XFRUdO3ZsxIgR77777pAhQ/785z+vXr36/fffV0rl5eWtW7fu/vvvtw/Mz89vbW3Nz89XSvXv37+urm7QoEH201atWjVnzpz169fPnj17w4YNU6ZMWbZs2d69e9euXRt7YENDw3e/+93a2tqbb745HA6fPn26V69eDQ0Nffv2VUotWbLk9OnTixcvjnvpxAVfuHChf//+GzZs2LRp09KlS+3lZXZy+8fly5f/7Gc/O3To0Pe+9729e/f269dP7gQdjDor/0ZpXTY6YKbS0tLdu3f/9Kc/Xb9+vV3bHTt2jB49esiQIUqpOXPm7N69+/Tp0/aToyN2rAsXLhw/frykpCT6yKxZs5RSY8aMKSwsnDJlilJq7Nix0Uk86t133x05cuTNN9+slAqFQr169VJKbdiw4ZZbbqmoqHjppZf27NkTfXL0pRMXXFBQUFtb+/vf/37lypVVVVU7d+7M+OS22bNnK6Wuueaam266yT6b3EAHDNsdsRif3aXjW4WDBw/et29fVVXVli1bysrKzp07l+LJl19+eeKD+fn59lAcfaSwsFApFQqF7G/s7xN3eBPfjqurq1u+fPnGjRu3bdu2aNGi2HNGXzrpgsePH19bW/vwww/Pmzdv2rRpkUgks5Mnss9DoHMn96M0QzTE+uKLL5RS06ZNW7Zs2dmzZxsbG8eNG1dX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)

Now we just need to change our label:

```r
barp <- barp + coord_polar(theta='y')
barp <- barp + theme(
    axis.line=element_blank(),
    axis.text.x=element_blank(),
    axis.text.y=element_blank(),
    axis.ticks=element_blank(),
    axis.title.y=element_blank(),
    panel.background=element_blank()) +
    labs(y="Carburetors")
print(barp)
```

![img](data:image/png;base64,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Wi8SGq0X6gwkQaA9FviU1nFEI2UGnnKsXr06EolE//H73//+iRMnUrihhx555JH07yQrKyvuK21tbaIDrcv5RiIa7QTzGa60traqjp197bXX+vbte8sttzi5eTqBtn90oqqqqrvvvvv555+/8847N27c6O2dZ2dniw601gKf0oBkjY2NixcvLigomDRp0oIFC+wvvvzyy0VFRRMnTiwpKTl16pT9xaysrMcee2zRokUVFRUrV65sa2srKSmZPXt2Y2Pjhg0bysrKot/2xz/+saCgYPTo0Xv37n344YcnTJgwYcKEkydPKqXibvjWW2/NmDGjoKCgsLBwz549SqklS5ZMnjy5oKBg4cKFdXV1iT868YKbm5vvu+++p59++kc/+tHrr79eUlJi3yqFO7e/smrVquLi4nHjxu3YsaP9eyzL8vd/hzTou6Bj5d88JZife+s0P+72jUfv8eR+mM8eOrt3a9CX4FpVVdXGjRvtEn3xxRf9+vU7f/78hAkT3n777bFjx/7973/fuHHjwYMHlVJZWVlbt279yU9+Yt8wJyenqakpJydHKTV48ODq6uoRI0bY37Zhw4alS5e+8MIL5eXllZWVc+bMWbdu3bFjxzZv3hx7w0uXLn33u9+tqqqaNm1aW1tbQ0ND//79L126dMMNNyilnnjiiYaGhjVr1sT96MQLbmlpGTx4cGVl5a5du9auXWtfXmp3bv/j+vXrf/3rX58+ffq22247duzYoEGD5C7ocNRZMaWBzkycOPHw4cMPPvjgCy+8YNd2//79xcXFY8eOVUotXbr08OHDDQ0N9jdHJ3aslpaWixcvDhkyJPqVJUuWKKWmTp2am5s7Z84cpdT06dOjSzzq7bffLiwsnDZtmlIqOzu7f//+SqnKyso77rhj1qxZ27dvP3r0aPSboz868YJ79OhRVVX117/+taKiorS09MCBAynfua28vFwpddNNN02ZMsW+N7mBDpnMN1rySTTzGaNGjTp+/HhpaemePXsKCgq++uqrJN983XXXJX4xJyfHHsXRr+Tm5iqlsrOz7U/szxNPeBMfjquurl6/fv2LL764d+/e1atXx95n9Ed3esG33357VVXVz372s+XLl8+bNy8SiaR254ns+yHQmZP5KS250fCQjs/l+Oyzz5RS8+bNW7du3dWrV2tqambMmFFdXW0/JWPDhg1FRUV9+vRJvGG/fv3q6+uVUllZWePGjfv4448d/sToDW+//fYjR47Y5yetra11dXW1tbVDhw7Ny8tTSj333HMOL7ixsdG+2qysrKKioubm5ra2ttTu3LZp0yal1OnTpw8dOjR9+nSlVI7Dv1uGheZ8I1HNyUNBnUoLwXyGUur9999fsWKFZVmRSGTZsmUjR45USm3ZsqWsrKy5uXnIkCHPPPNMpzdcvnz5zJkzc3Nz9+/fv2DBgtdee23SpElOfmLsDSsrKx966KEvv/wyOzv7b3/7W0lJyebNm+fOnZuXlzds2LCLFy86ueAvv/zyt7/97aVLl86ePfvSSy89+eSTPXr0yM/PT+HObVeuXCksLGxqaqqoqLDPrIU+SBjiQEdlLNPePlqY/oOEBNoPOj5OmL7z58/PnTu3uro6Ozs7wMtYsWLFn//8Zz/umSOOwGTsuEPUQQd19omOpxzpGzJkyKOPPvrJJ58Eexm33nqrH3fb1tYmcUGbMJ+jMrOjPRzRaS5oAu0fM0d0uLGgA5aZRw6FjGjqDG/94he/mDt37uzZs3fv3h30tfhC6IOEpuGRQ6RvxKwlGo3oE5cjV5rd/ef7sN7XDO/z7ZPYjh49eubMmVdeeeXTTz8tKyt75513vL7G4BFoKewd7V+maz486NNrCx1iPiPWsx+2nqh1984YC8fklN36bbLy8vK++uqrSCRSW1s7aNAgry9QBHGBNuoAOpGvUzrARlNnxLl5QPscvtRoHbmYrNSzR2TnXKOUUgN6dXgNyIgRI8aPH19cXFxbW/v888/7ebGBERdo+D2lAQlO1kYcLug3z7bZnywc0yHQb7zxxuXLl997773PP/987ty5R44c8f4qg8aDhEL59MhhII8WMp8zRqMn21lWxIq0ufuwOgS9rq5uwIABSqm+fftG37UjZAi0XD49wUPIMzpgOCsScfuhOj4n+N57762pqSktLS0tLX388ceD+ov4StYRh+EH0J3S/QkezGd0yl7QLm/SIdA9e/bcvn27pxclDgtaA55PaUY0gpf2gjYBgdaGjm8qzXxGVyzLcn3KQaAhmYdTmhEdVro8Tuj6EcJIm7J8+ZWvkhFo/ejSaOYzkmBBOyHoQUIeIXSO50pDe1ZEWe4eJGRBQyfpT2n/RjTzGd3gQUIHCLTe0j+V5jAagUjphSoEGhqS9gQP5nOwtHic0LIibj+UItDQUzpTmhGNzONBQicIdKhImNLMZzjC0+wckBJonsLhldSmNCMaGWZFWNDdkxJoeCuoRjOf4VhEWW0uP4wLtKDnQcNbmX+uNHWGc+3PnHN5G3+uRS4WdMi5mtIcdCBjeJqdEwQ6/FydSqfcaOazKBo8044XqjhAoE0h4QkeQJRlWa6fCs3zoBFiDqd0CiOa+Qy3LMv1gk484jhw4MBdd9119913/+lPfwrkb+E3HiQ0ju6/ogXhYEVc/0YV1fFBxaampocffnjXrl19+vTx8sokEbGgeRJ0hnU7pV2NaOYzUpD+gt63b1///v0feOCB+fPnh/JXeisWtMmST+maDw/m3zotk9cDo4z/n77fGdhLKXXhi68PfVKb5DvnTBjSIztLKXVDn2tjv37u3LkPPvjg2LFj58+fX7x48X/+8x9fLzgQBNpo6R93MJ+RmuOf1h37b72T79x15DP7kyW3fSf26wMGDJg8eXLv3r1Hjx7d0NDQ1taWnZ3t+XUGS8QRBwKU5LiDp0XDP+kfcUyfPv2TTz6JRCK1tbXXXntt+OqsWNCwdTWlkx90MJ+Rsm/eQdTVbTp8/8CBA5ctWzZnzpyvv/76ySef9PLixCDQaMev0UIm2a8kdHmT+KfZlZeXl5eXe3dR4nDEgQ4Sjzu6OuhgPiMt7t/NzsBXErKgEY8pjQywrDb3C5o3SwKUUh2ndOKIZj4jXZalrIi7D17qDUTFPsEjttHUGelz/RQOI484CDS6wbsswQ+83agTnEGje9FG5986jfmsixGzlpzduzXoq+haKm/YT6CBLjCl4SH77Ubd3sSnixGLQMOFmpOHeg0YopRqrD0f9LVAb/YrCd3exp9rkYtAw51eA4c2Xj5nZ1pRasFEn2+k9HajBj7NjkDDNbvR7Z9TaqTGsljQ3SLQ8AalhjvtT212dRMCDTgQO6Lj/4hSwwHL/YLmQULAqSSNbv8GSo2u2U9tdnsbf65FLgKN1HXb6PZvo9RIkMrT7Mx7qTeBRuZQakTxNDsneKk30tJr4NBUbjVgSPTD80uCHty/3WinZ9BHjx7Nzs4+fPhw5v8GGcCCRrocHnR0eXNmtZEsq82y3J5BdxLoNWvWzJw505trkodAwwNpNrr9Tii1USxLpX3E8dZbb40ZM6a1tdWzqxKGQEMcSm2CwtFDbxyap5T6/PKVd47/X5LvnH/7+B451yilBuVdH/dHa9eu3bZt29KlS327zICJCPSRTb8puP8vQV8F0uLJiI6/T0odXu9+9N/3Pvqvk+/csfeo/ckD907v8PUdO2bNmtWvXz/vL04MHiSEZ1J7wNDRPfOIYvi4fTPoSFvcEceRI0deffXV0tLSffv2LVu2rKamJqi/in9ELGjAITZ1aKT/dqOrVq2yP1m0aNHvfve7/Px8zy5ODAINL/lx0NH5D6LUmvPwedD/+Mc/PLggkQg0PJaxRrf/OEqtJyvCe3F0j0DDexludPsPpdQxhL8ZtFJKWa7fD5r34gC0R6n1wNuNOkCg4YtARnT8NVBqwTjicIJAwy8SGm2j1AJZKuL+V1gZF2gpz4M+suk3QV8Cwo83aRIkEnH9wYIGPCRnRCdiVgcr/edBm4BAw1+SG22j1MHg/aAdINDwnfxG20JTag2eY8eDhM4QaCBeaEotm/un2Zn3ICGBRiboMqLjUGr/pLCgDTzikPIsDsUTOcLOv/e6ywCe++E5y4q4/zAu0CxoZI6mOzoWm9orFi/1doBAA6kQW2otHiFUqv2Mw90tWNCAr0IwouOILbVwnEE7IegMWnEMbQatD6OT4JzaHYtXEnaPBQ14jE3tRCqvJOz4NLt33333V7/6VY8ePZRSTz/99KhRo7y8PhlkLWgYIqwjOk7mN7U2B9Df/EYVVx9xC3r48OG7du3avXv3z3/+8yeeeCKov4ivWNAIRvgOo5OIbTSzup1lpfl+0IMGDbI/ueaaa+wdHT4EGoExqtFRHIDYxo8eNWhAP6XUhZq6Q0dPJvnO0jsm5+TkKKXy8/om/ml9ff2aNWueffZZn64zWOICfWTTbwru/0vQVwH4zvBSH/vozL+PnHDyna/s+bf9yf8OHxz3R19//fUPf/jD1atX33zzzR5fnwziAg2jmDmi43hVao0OoJVS7cfKrm7S8YgjEoncd999P/7xj++55x5PL00QAo2A0egoozZ1Cs/iiDuD/uc///nKK69cvnx527ZtU6ZMCeXjhBIDzSmHaWh0HCNK7f79oOMW9KJFixYtWuTpNYkjMdAAbCEutRVx/V4c7n+HofYINERgRCfXban1OoBWyn6anXGvDHSLQEMKGu1EaDa1pdI9gzaB0FcS8qYcQHK6v/WH25cRWhET3w9aaKBhJkNeAu6tXgOG6He+ob55JaG7D+MCzREHZOGgwxiu3w9aKeMeJJS7oDnlMBY72gj2g4TuPoK+5oyTG2gATnz04rqgLwF+IdCQiBENKKWyhD8wyksKTcZhtBOaLugrX15taWl1dZPreuX2yu3p0/XIxIOEkIsHDLulaZ2VUn17Xx/0JWhA+hEHDxUCMJb0QMNwHEYnoe98hkMEGtLRaBhLg0BzygHATBoEGmBEJ+J8wwR6BJoRDRoNA+kRaEDR6BjMZ0NoE2hGNADTaBNoQDGilVLMZ5MQaGiGRsMcOgWaUw7YTG4089koOgUaAIyiWaAZ0bCZPKJhDs0CDUQZ2GjON0yjX6AZ0TATdTaQfoEGogwc0TCKloFmRCPKkEYzn82kZaAVjUYMQxoNA+kaaMAczGdjaRxoRjSiGNEIJY0DDcQKa6OZzybTO9CMaMQKa6NhLL0DDYQb89lw2geaEY1YYRrR1BnaB1rRaHQUpkbDcGEINBA+zGeo0ASaEY1Yuo9o6gxbSAKtaDQ60r3RgApToIE4mjaa+YyoUAWaEQ0gTEIVaEWj0ZF2I5r5jFhhCzQQR6NGU2fECWGgGdGIo0WjqTMShTDQikYDCIVwBlrRaHQkfEQzn9Gp0AYaiCO20dQZXQlzoBnRkI86I4kwB1rRaHQkdkQDnQp5oBWNRkeiGs18RnLhDzQQR0ijqTO6ZUSgGdGQhjrDCSMCrWg0Ogp2RFNnOGRKoBWNRkdBNZo6wzmDAq1oNDoSchgNdMWsQCsajUAxn+GKcYFWNBoxMjmiqTPcMjHQikYjRmYaTZ2RAkMDrWg0Mog6IzXmBlrRaHzD1xFNnZEyowOtaDS+4VOjqTPSYXqgFY3GNzxvNHVGmgi0UjQaPqDOSB+Bbkejobwb0dQZniDQ36LRUF40mjrDKwS6AxoNlV6jqTM8RKDj0WikjDrDW1mWZQV9DRIV3P+XoC8BAWu8fM75N5Nm+IEF3Tl2NJwfdFBn+IRAd4lGwwnqDP9wxNE9jjtMlvyggzrDVyzo7jGlTZbkoIM6w28saKfY0SaL29GkGZnBgnaKHQ0bdUbGsKBdY0qbyR7R1BmZRKBTQaMNxH9CIfM44kgF/7dqGv4XRyBY0GlhSpuAOiMoBDpdNDrESDOCRaC9QabDhzojcATaMzQ6NEgzhCDQHiPTWiPNEIVA+4JM64g6QxoC7RcarRHSDJkItL/ItHCkGZIR6Ewg0wKRZshHoDOHTMtBnaEFAp1pZDpYpBkaIdDBINOZR5qhHQIdJDKdAXQZ+iLQwSPTPiHN0B2BFoRSe4U0IxwItDhkOmV0GSFDoOWi1M6RZoQSgZaOTCdBlxFuBFoblDqKLsMQBFpLZsaaLsM0BFpvoS81UYbJCHR4hCnWdBlQBDqstIs1RQYSEWgjCOw1RQa6RaDNlbFq02IgNQQa3UjSccoL+IpAA4BQ1wR9AQCAzhFoABCKQAOAUAQaAIQi0AAgFIEGAKEINAAIRaABQCgCDQBCEWgAEIpAA4BQBBoAhCLQACAUgQYAoQg0AAhFoAFAKAINAEIRaAAQikADgFAEGgCEItAAIBSBBgChCDQACEWgAUAoAg0AQhFoABCKQAOAUAQaAIQi0AAgFIEGAKEINAAIRaABQCgCDQBCEWgAEIpAA4BQBBoAhCLQACAUgQYAoQg0AAhFoAFAKAINAEIRaAAQikADgFAEOlRaWlp+//vf33jjjTfeeOP48eMfeeSRlpYWh7fNysry8EpWr14diUQ8vEPAQAQ6VMrLy6urqw8ePHjmzJnq6uphw4ZdvXq121u1tram9uOS3NB5oFP+6UDoEejw+PjjjysrK7ds2XLDDTcopXJzcx966KH+/fsrpZYsWTJ58uSCgoKFCxfW1dXZ35+VlfXYY48tWrSooqLC/sqqVauKi4vHjRu3Y8cOpVR9fX1+fr79R62trbm5uZ3e8J133vne975XXFw8derU3bt3K6VWrlzZ1tZWUlIye/bsxsbGl19+uaioaOLEiSUlJadOnUq8k8bGxsWLFxcUFEyaNGnBggUZ+zcGSGchLLZv3z5u3LhO/+jixYv2J2vWrFm5cqX9uVJq69at0e9RSq1fv96yrFOnTg0aNOjChQt1dXUDBw60/7SlpaVnz56JN7x8+fKECRPOnTtnWdann346cuTIpqYmy7Kys7NbWlosyzp37lx+fv7Jkycty6qoqJg6dWrinezcuXP+/Pn25/X19R78uwBCISfY//eAzKisrNy2bZtlWQ0NDcOHD49+PW6ulpeXK6VuuummKVOmHDhw4I477ujqDqM33Ldv3/nz58vKyux/7Nmz59mzZ0ePHh39zv379xcXF48dO1YptXTp0l/+8pcNDQ19+vSJvZOJEycePnz4wQcfvPPOO3/wgx948lcGQoBAh0dRUdGZM2cuXbpkH3FEVVdXr1+//sCBA3l5eTt37nzqqaeif3Tdddd1dW9ZWVk5OTmWZdn/2NzcHPun0RtGIpFbbrnlzTffTOGCo3cyatSo48eP7969+9VXX125cuXRo0eTXBhgDs6gw2PMmDELFiz46U9/euHCBaXU1atXH3/88fr6+tra2qFDh+bl5SmlnnvuuST3sGnTJqXU6dOnDx06NH369N69e1977bWff/65Uuqll17q9CYzZ8784IMP/vWvf9n/uH//fvuTfv361dfXK6VmzJhRXV194sQJpdSGDRuKiors+Rzrs88+U0rNmzdv3bp1V69erampSf3fAhAiLOhQ2bJlyx/+8Idp06a1trb26tWrrKzs+uuvLykp2bx589y5c/Py8oYNG3bx4sWubn7lypXCwsKmpqaKigp7hj/11FPz588fPXp07KlFrPz8/KqqqhUrVixfvry1tbWwsHDGjBlKqeXLl8+cOTM3N3f//v1btmwpKytrbm4eMmTIM888k3gn77///ooVKyzLikQiy5YtGzlypEf/PgC9ZUX/GxYAIApHHAAgFIEGAKEINAAIRaABQCgCDQBCEWgAEIpAA4BQBBoAhCLQACAUgQYAoQg0AAhFoAFAKAINAEIRaAAQikADgFAEGgCEItAAIBSBBgChCDQACEWgAUAoAg0AQhFoABCKQAOAUAQaAIQi0AAgFIEGAKEINAAIRaABQCgCDQBCEWgAEIpAA4BQBBoAhCLQACAUgQYAoQg0AAhFoAFAKAINAEIRaAAQikADgFAEGgCEItAAIBSBBgChCDQACEWgAUAoAg0AQhFoABCKQAOAUAQaAIQi0AAgFIEGAKEINAAIRaABQKj/B7CACzoj2ISeAAAAAElFTkSuQmCC)



## Scatterplot

A  scatter plot uses points and Cartesian coordinates to display the  position of values between two or more variables. It is possible to plot  scatter plots in 2D and 3D.

Let's start importing the `ggplot2` library.

```r
if("ggplot2" %in% rownames(installed.packages()) == FALSE) {install.packages("ggplot2")}
library(ggplot2)
```

We  can create a very simple 2D scatterplot simply using qplot. Using two  variables as parameters makes a scatterplot by default.Here we are using  the mtcars dataset.

```r
qplot(mpg, wt, data=mtcars)

```

![img](data:image/png;base64,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)

We can create a similar graph using ggplot.

```r
ggplot(mtcars, aes(x = mpg, y = wt)) + geom_point(shape=1)

```

![img](data:image/png;base64,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)

You must have noticed that the shape of the circles changed. We can have solid circles modifying the `geom_point` parameter

```r
ggplot(mtcars,aes(x=mpg,y=wt)) + geom_point(shape=19)

```

![img](data:image/png;base64,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)

As  we can control the shapes, we can take advantage of this and plot three  variables in a bidimensional scatter plot. You just need to pass the `shape` parameter as a column present in your dataset.

```r
ggplot(mtcars,aes(x=mpg,y=wt,shape = cyl)) + geom_point() + scale_shape_identity()

```

![img](data:image/png;base64,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)

It  didn't work. That's because we need to have categorical data, instead  of numerical. We can fix this creating factors for the cylinders.

```r
mtcars$cylFactor<- factor(mtcars$cyl)
```

Now we just need to plot our graph again.

```r
ggplot(mtcars,aes(x=mpg,y=wt,shape = cylFactor)) + geom_point()

```

![img](data:image/png;base64,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)

We can change the colors of our circles using the `colour` parameter

```r
ggplot(mtcars,aes(x=mpg,y=wt)) + geom_point(shape=19, colour="blue")

```

![img](data:image/png;base64,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8oEHHhg+fPjAgQNTe9w2Bhp3wG1jIBaLpTaCwWB1dbVy3xho3IEmx0C2z+JQSt13331lZWW2bZeVlU2bNq1Tp07Dhg37+c9/rpQqLi7Ofj3Z16ADn3zyyZIlS7xer2mat956q+7qMq60tHTLli0VFRVvvvlmr169Jk2a5LYx0LgDbhsDO9Dv5nEAAAHUSURBVHfufPrpp03TjMViN910k1LKbWOgcQeaHAOcBw0AQulf4gAANImABgChCGgAEIqABgChCGgAEIqABgChCGgAEIqARntjGEZJSUn//v179uy5YcOG22+/vW/fvn379v3oo49qD5g9e/akSZOGDRv2wgsvpHauXLny3HPPHThw4IIFCzweDRdwAY0R0GiHCgsL33vvvYULF15++eWjRo3atm3b5MmTFy5cWHvAhRdeuHTp0tWrV8+YMeOrr77av3//jBkzXnnllc2bN/t8Po2VA/UR0GiHUs+JHzRokNfrHT16tFJq8ODBn3zySe0BqfuHderU6cILL9y0adPbb789ZMiQM844Qyk1depUTVUDDRHQaIdSd1u2LCu1kdqOx+O1B9TeqiYWi6VuywsIREDDjf7whz8opT7++OPNmzcPHjx48ODBpaWlu3fvrv0jQAK+DIEbhUKh/v37V1dXL1q0qLCwUCn10EMPXXrppX6/f+zYsR06dNBdIKAUd7ODCxlGE8M+FAoFAgGl1NKlS1euXLl27VodpQHHYQYNKKXUwoUL161bV1NT06lTp9///ve6ywGUYgYNAGLxJSEACEVAA4BQBDQACEVAA4BQBDQACPX/3zrR3Fl8cHIAAAAASUVORK5CYII=)

As we did with the shapes, we can do the same thing with colours. Again, you just pass the `colour` parameter as a column present in your dataset.

```r
ggplot(mtcars,aes(x=mpg,y=wt,color = cyl))+ geom_point(shape=19)

```

![img](data:image/png;base64,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oCgCGgAURUADgKIIaABQFAENAIoioAFAUQQ0lKBp2pw5c0aPHj1o0KC33377vvvuGzVq1KhRozZv3tyywsyZM2+55ZZJkya9/PLL8QcXLlw4bNiwc845Z9asWaYp+6orINMIaKiiV69eH3744ezZs6dOnXrJJZesX79+2rRps2fPblnhjDPOmD9//iuvvHLPPffs379/796999xzzxtvvPHee+8FAgEPOwcyhICGKm666SYhxNixY/1+/6WXXiqEGD9+/LZt21pWiM9DVlZWdsYZZ6xcufKf//znhAkT4rcS/8Y3vuFR10AGEdBQRXzyZcMw4gvx5Wg02rJCy5Q3kUgkPr0vkNsIaGSN3/72t0KIrVu3vvfee+PHjx8/fvyKFSt2797d8k9AjuF7FWSNYDA4evToUCg0b968Xr16CSF+9rOffelLX8rLy7v88suLi4u9bhBIM2azQ3bQtHZ+VoPBYH5+vhBi/vz5CxcufO2117xoDcgUjqCRxWbPnv3666/HYrGysrKnn37a63aANOMIGgAUxZeEAKAoAhoAFEVAA4CiCGgAUBQBDQCK+v81U1D6XfrRWQAAAABJRU5ErkJggg==)

As the graph before used numerical data, it created the label with a gradient from 4 to 8. If we use categorical data, like the `cylFactors`, we can assign a unique color for every category.

```r
ggplot(mtcars,aes(x=mpg,y=wt,color = cylFactor)) + geom_point(shape=19)

```

![img](data:image/png;base64,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BzYwqwugAgJaCCE+/9J+csnhe4n8nzG1I3pLuseYOlbu8L29PiCE+HS3/elu+1eXSLpfHYA2MMQhhBBLt/kbl5dt93lYiVf21RlNf0wynzigAAJaCCEM/cgtgI2cnZyhLZVlR+65PLx33GS/ABTAEIcQQkwaGFmx4/CB87mVDd4W44lTihLXnlWzcqevhz91Xrf8HwAUREALIcRJeclZF+3fX2eUhFOmLmNCDQUNPSk+9KS411UAOIKPsoeZujiph5PZdK6N6lurLMZzAXQMR9DZ8uEW/4srD89l+YsLqvL85DSA9uEIOlsa01kIsWSrv401AeCYCGgZpEwmDiAr/H5/epLykpKSk046qW/fvn379p02bdoJvvzuu+9OdTQCCOhs+edh9Y3LY0/pdle+ADnprbfe2rFjx44dO+bOnXuCLznxgE4mm1/Byxh0tkysiFSUJg426OXFyaCd+UPoupiuaSKUhXcGuolFixb97Gc/a2ho0DTtoYce+uijj7Zs2fKb3/xGCPHll1+OGDHiiy++CAaDrb38qquuWrduXSKRKC8vf/LJJwsLC1u+5+uvv+44zuTJkzVNe+211955553bb7/dcZzS0tLHHnusoqJCCKFp2s9//vN169add955N954Y9MmNNfN1rfK9u9v63Jhy7LC4fDBgwez1HozgUAgFot1+INGuxiGkZ+fX1VVlb0mXv00tGhjQAhx3sDIpaOSjuO0/NubDbquFxUVtb1lM8iyLCFEIpE47poZUVJScuDAgez9RjRlmqZhGLGYpI9WxcXF1dXVjuNIaEvXddu202MCEhQWFtbW1hYUFLT3hfv27Rs2bNhf/vKXs846y3Gc2traVCo1dOjQjRs3hsPhe+65p6qq6oEHHhBC+P3+6upqv99fUlLi8/nSu+Wvf/3rcePGlZaWCiFmz55dW1s7a9aslu9ZUFBgmmY0GjVNc8+ePcOHD//73/8+cODAxx9//Pe///2HH34ohNA07Y9//OOVV17ZskiOoLue3TVmOp2FEO+sD4wvry8JyfjFA3LJ3//+91GjRp111llCCMMw0hF/8cUXP/PMM9dff/0TTzyxcOHClq964403TjvttPTyo48++uyzz7quW1tb27dv39bes9EHH3xwxhlnDBw4UAjx3e9+96abbqqtrc3LyxNCXHrppccskoDueiKJo65Gb4hr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)

Now we need to rename our legend. Our users wouldn't understand what exactly is cylFactors.

```r
ggplot(mtcars,aes(x=mpg,y=wt,color = cylFactor)) + geom_point(shape=19) + labs(colour = "Cylinders")

```

![img](data:image/png;base64,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)

Just to finish our graph, we can rename and create the remaining labels.

```r
ggplot(mtcars,aes(x=mpg,y=wt,color = cylFactor)) + geom_point(shape=19) + xlab("Miles per Gallon ") + ylab("Weight") +
  labs(colour = "Cylinders") + ggtitle("Scatterplot")

```

![img](data:image/png;base64,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)

------



## Line Graph

Line  graphs are also representations of data in which Cartesian coordinates  are used. Much like scatterplots, the data is transformed into points -  however, in line graphs, they are connected by lines, as the name  implies.



### Simple Line Graph

For  line graphs, we are going to use the EuStockMarkets dataset. It is also  a dataset that comes included with R and it describes four European  Stock markets' historical data.

Let's start looking at their helpfile

```r
?EuStockMarkets

```

As we can see, it contains 1860 observations for each, and their filetype is `mts`, which stands for matrix. `ggplot2` doesn't work with matrices.

To get around this limitation, we should create a dataframe from this matrix. Thankfully, there's a function that does exactly what we need. It's the `as.data.frame()`.

```r
EuStockDF <- as.data.frame(EuStockMarkets)
```

Now, let's check its head, to see how the data is structured.

```r
head(EuStockDF)
      DAX    SMI    CAC   FTSE
1 1628.75 1678.1 1772.8 2443.6
2 1613.63 1688.5 1750.5 2460.2
3 1606.51 1678.6 1718.0 2448.2
4 1621.04 1684.1 1708.1 2470.4
5 1618.16 1686.6 1723.1 2484.7
6 1610.61 1671.6 1714.3 2466.8
```

Now, let's start plotting!

Let's create a line graph of the "DAX" stock price:

```r
ggplot(EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = DAX)) + geom_line()

```

![img](data:image/png;base64,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)

Let's increase the width of our line:

```r
ggplot(EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = DAX)) + geom_line(size=1.5) + labs(x = "Stocks")

```

![img](data:image/png;base64,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)

To change the colour, we can use the `colour` parameter.

```r
ggplot(EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = DAX)) + geom_line(size=1.5, colour="light blue") + labs(x = "Time", y = "Stocks")

```

![img](data:image/png;base64,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y/ryl7/8wAMP7Nu37+tf/zrFnTqczBW0crpwAhvhibcefR/QmUymUCgEtznv+4fTPYyxTCZDRLfddtuLL75IcacOJ3MFrZwunMBGeOKtR9+fi4MHD05OTiqlTp8+vWfPnl43R1+lUkkpRUSTk5PBRZjGU4eTuYJWThdOYCM88dZjEMZBnzhx4kc/+hERHTt2DNd/m5mcnPzqV79q2zbn/J577rniiiso7tThZIYefPDBF1980TTN66+//u6776bWThdOYN15wxNvPQYhoAEABlLflzgAAAYVAhoAQFMIaAAATSGgAQA0hYCGAec4zq5du3bt2rV161YhRHD7jjvuICLbtkulUq8bCNDUICyWBLACy7IuXrxIRE8//fQ73/nO4Hbg+9//vrbbpAEQetCwmb397W93HIeIGGMPPPDA9ddfv3///kcfffRP//RPr7vuuuuuu+75558P7vnEE0/cdtttN9100y233PK9732vp62GTQQBDUBEtGXLlmeeeeazn/3s7bff/uu//us/+9nP3ve+9332s58lotnZ2T/+4z/+5je/efLkyW9/+9vvf//7g1gH6DaUOACIiO68804iuuWWW2zbDraCvfXWW//93/+diB577LHLly///u//fnBPy7IuXLiwf//+HrYWNgkENAARkW3bRCSECG4Etz3PIyIp5cGDBx955JEeNg82J5Q4AFZx5MiRZ5999r//+7+DL5988snetgc2DwQ0wComJib+4z/+45Of/OShQ4euueaahx56qNctgs0CiyUBAGgKPWgAAE0hoAEANIWABgDQFAIaAEBTCGgAAE39f1wfjYs76LL5AAAAAElFTkSuQmCC)

We can also plot more than one line at a time in the same graph. Let's try plotting two stocks in the same graph.

```r
dax_smi_plot <- ggplot() +
  geom_line(data = EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = DAX), size = 1.5, colour="light blue") +
  geom_line(data = EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = SMI), size = 1.5, colour = "red") +
  labs(x = "Time", y = "Stocks")
print(dax_smi_plot)
```

![img](data:image/png;base64,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)

Now, let's plot all the stocks.

```r
all_stocks <- ggplot() +
  geom_line(data = EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = DAX), size=1, colour="light blue") +
  geom_line(data = EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = SMI), size =1, colour = "red") + 
  geom_line(data = EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = CAC), size =1, colour = "purple") + 
  geom_line(data = EuStockDF,aes(x=c(1:nrow(EuStockDF)), y = FTSE), size =1, colour = "green") +
  labs(x = "Time", y = "Stocks")
print(all_stocks)
```

![img](data:image/png;base64,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)

Let's change the labels in our graph.

```r
legend_stocks <- all_stocks + xlab("Days") + ylab("Price") + ggtitle("Eu Stocks")
print(legend_stocks)
```

![img](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAeAAAAHgCAIAAADytinCAAAgAElEQVR4nOzdeWBU1d0//ve526zZwxZAkB1BZXMF3H9qFXGpa0Wt1lqx+vj0q3Vpq8Vqq/Sxj1Wstq48LrjVvVpcQQG17DuI7AIhgeyT2e5yfn+cmZvJzCSZTCbJlXxef+idM3funEzIJyefe87nMM45CCGEOI/U3R0ghBCSHgVoQghxKArQhBDiUBSg2zZp0qRnnnmmu3tBCOlxnBigp02bxpqbO3duhq/dt2/f1VdfXVZW5vF4hg8fft1110UiEQDHH3/8448/3omdJoSQXFO6uwPpXXzxxb/97W/th4cddliGL7zooossy5o7d25ZWdmOHTveeuutaDTqcrk6p5uEENKZuPOce+65v/jFL1LbBw0a9Pbbb4tjXdcBrFu3LvGE6upqAIsWLUp64ZVXXml/vUOHDuWc19fX//SnPy0oKPD7/ZdccsmBAwfsy9599939+/d3u91jx4797LPPOOcTJ058+umnxQm33HLL6NGj9+3bxzl/9dVXR40a5XK5+vTpc+ONN+byIyCEEM6dmOLImt/v93q9H3/8sWVZie0vvfTScccdN2fOHM751q1bAdx6661Lly796KOPFi1atGPHjuuuu06c+dvf/vbll19+6qmnNm/ePHv2bFmW7Ytwzm+88cYFCxYsXLiwX79+lZWVV1111T333LNt27b58+cfe+yxXfmVEkJ6hO7+DZHGueeeyxiTE6xevZpnMILmnM+bNy8/P7+oqOjcc8997LHHqqurRbsdoDnnNTU1six//vnn4uHq1asBbN26taGhQdO0Dz74IOmaEydO/Mc//nHttdeOGzfOHmuvXr1a07SqqqpO+AAIIYRzx46gL7nkktUJRo4cmeELr7jiivLy8hdeeGHcuHGPPvromDFj9uzZk3TOtm3bTNM87rjjxMOjjz7a4/F8++233333XTQaPemkk1Ive9999y1atOjzzz8vLS0VLWPHjj3hhBOGDRs2Y8aMV155RdyKJISQHHJogC4qKhqbwO12A5Ckpt6aptnSa71e77Rp0x544IG1a9fKsvzkk0+2+Xacc/u/aZ1yyinl5eWff/653SLG4P/85z/79+9/1113TZ48WQzqCSEkVxwaoNPq1atXVVWVOP7uu+/aPN/r9fbp06ehoQGApml2TB86dKgsy9988414uGrVqnA4PHLkyBEjRmia9uWXX6Ze6tRTT503b97VV1/90Ucf2Y2SJJ122mmzZ89euXLlihUrNm7c2MEvkBBCEjk0QFdVVSWmOPbv3w/gpJNOeuGFF4LBYF1d3W9+85vUV1VUVEydOvX5559fvnz5ihUr7rzzzpUrV5577rkABg0atHjx4n379tXU1BQWFl5zzTU333zzV199tXz58uuvv/68884bOnSo3++/5ZZbZs6c+f7772/fvv2DDz5YuHChffHp06c/9dRTF1988eLFiwEsW7Zs9uzZa9eu3bt377x58zweT+ZzAQkhJCPdnQRPQ4TURL///e8559XV1eeff35RUdGIESPeeustpNwkDIVCd95551FHHeX3+wsKCo455phXXnlFPLVmzZqjjz5a07SkaXY+ny9xml0kEvn1r3/dp08ft9t95JFHLliwgDefZvfEE08UFBSsWLFi8+bNZ5xxRklJicfjmTBhwvz587vo0yGE9BiMU7lRQghxJIemOAghhFCAJoQQh6IATQghDkUBmhBCHIoCNCGEOBQFaEIIcSjH1YOur6/PYuafLMuapoVCoc7oUsdpmhaNRru7F+n5fL5gMOjM2ZZO/tzcbrdhGIZhdHdH0lAUxbKspJqODqGqqiRJzqxdwxhTFKV7azYUFBQkPnRcgNZ1PYtgwRiTJMmx1TA0TXNs38S/SMcGaMd+bl6v17IsZ3ZPkiTTNB37ywOAMz83UUTTUX2jFAchhDgUBWhCCHEoCtCEEOJQFKAJIcShKEATQohDUYAmhBCHogBNCCEORQGaEEIcigI0IYQ4FAVoQghxKArQhBDiUBSgCSHEoShAE0KIQ1GAJoQQh6IATQghDkUBmhBCHIoCNCGEdIj8/feev/+ddcKOTo7bUYUQQn5YfHfcoX36Kde08HXX5fbKNIImhJAOUdatAyBVVeX8yhSgCSGkQ0RygzU05PzKFKAJIaRjwmFQgCaEEMexLBaNAmCNjTm/NgVoQgjJHotEYgedMIuDAjQhhHRAPC7bkTqHKEATQkj2muIyjaAJIcRRmK7HDmgETQghzsGiUeXrr8Wxsnp10dSp4oZhrlCAJoSQLHkeeyzv5ptjDziXN2+WystzeH0K0IQQkiVp797kppxmoilAE0JIllh9fXILBWhCCHECedeupBZlxYocXp8C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)



### Regression

Regression  is a mathematical modelling concept in which a linear formula is  created to simulate the percepted behaviour of the data points you  create the model for. Regression is a great way to visualize trends and  to create basic predictions.

Predictions are made on  one set of variables, given another set of variables. Trends are usually  extracted from the relation between two sets of variables.  In this  example, we will be checking if there is any relation between the weight  and miles per gallon of a car.

To visualize regression,  we can trace our fit line onto our graphs. Let's use the same example  from the previous section and draw our regression line on top of it.

The first method that we will utilize is linear regression, which is  regression that utilizes what we call a linear model. To do so, we pass  the `lm` parameter to the `method` attribute of the `geom_smooth` function, like so:

```r
ggplot(mtcars,aes(x=mpg,y=wt))  + geom_point(shape=19) +
  geom_smooth(method="lm", se= FALSE, color = "red")

```

![img](data:image/png;base64,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)

You might have noticed that our code has `se = FALSE` on it. `se`  represents what we call the "confidence interval" of our model.  Confidence intervals are a lower and higher bound in which we can have  95% certainty that a data point will be in.

If you want to display this interval, you can either just ignore the `se` attribute, or set it to `TRUE`.

```r
#se = TRUE  -> confidence interval appear (default = true)
ggplot(mtcars,aes(x=mpg,y=wt,color = cylFactor)) + geom_point(shape=19) + geom_smooth(method="lm", se= TRUE, color = "red")

```

![img](data:image/png;base64,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psDZdaOcYFqjoVXctltXSVMmk/LgF+qP31cc/d7jnq/1hmFt2+ZbJxLa93++ADjX8T364osv2my2ZcuWtc2CWltbu3LlSp80LiBpldedqAxRSeh6BnczunHcuILsbEtUlKK6OnXu3NBDh9yt0cWMVh78QvG/Y7KifOW3X8tPujdddRs2SNu8cIlpxsPGP86yjJvoWSEQMGiaZtxB++Ibvesq4+LiSkpKRG5KLxGsdNw/tIXbvn2waaDek6svhONuRhsTE/NyclpuuIE2GgcvXRqdne1uja5ktDz/TNu27PJFd6tow6rUtsRke1TPF5BAwFMoFGp3cNcUiazjGDTn5MmTWVlZZrN50qRJkydPnjRpUlRUlMgtC2Dj4k2jY02EUDJaiuep3B2StkZEFLz9duzateH79/fPzlZUVZU/9xzrzru5xyFpa9pQed7P3LYN8Qp8aG1tdevi1M6X2Ymg64DesWMHIaSiouLf//73ihUrzp8/L87Fob2HjCaESPcldTejHQpF6UsvmRITB7zxRsQnn6jOny/etMmq17teAldddzFtnjSFMAxlMNijoq3Db3a9WAC/1nVAHzt27ODBgwcPHrx8+fKUKVMmT54scrPA57isdCOmKepyero5Ojpu1SrtqVOpGRnnXn3V5OaASXddaVataZ063a2iAAJA1wF9yy23jB07dsOGDRMn4lxKr+ZuV7pu8mRz376DlyxRXryY+vjjpevWNYwb51aNvrkCD0CSuj5JePTo0fvuu2/NmjVDhw6dO3fu+24uIQqBxN24bBkyJC83tyUlhTEaExcv7rtvn7s1YgI8AE7XAX3LLbcsX758z5498+fP379//0MPPSRys0BS3M1oS2RkwVtv1U+cSDkcA7OyYjdsoNycKgRzSYNPNNpbTreUmBw9/Dj2yJEjd95551133bVp0yZB29P1EMf8+fMPHjxoMpkmTZq0du1ajEEDl9Hl5eUuPp5bfzZ6587+2dmRH36ovHSpeP16e3CwW5WWlJQkJCS421QAz3zbePLe/KXc9onhuxO6mc+rtbV18eLF+/fvD3bz/eyBrnvQN95442effXb+/Pndu3f/8Y9/xDV2wImPj3fj0RR1MTOzbOVKVi4POXo07bHHVOfPu1sjrscH0Wy/8q+27a2X3uvuYd9//31oaOjs2bPvv//+U6eczevvva4Des6c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)

As with the other graphs, we can add labels to our linear regression graphs:

```r
ggplot(mtcars,aes(x=mpg,y=wt,color = cylFactor)) + geom_point(shape=19) + 
  geom_smooth(method="lm", se= TRUE, color = "red") + xlab("Miles per Gallon ") + 
  ylab("Weight") +  labs(colour = "Cylinders") + ggtitle("Linear Regression")

```

![img](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAeAAAAHgCAIAAADytinCAAAgAElEQVR4nOzdd2BT1eIH8HNHdjrSQqGlLXQPULYIwgMeKA4Q8TlRpixZoqyioMiUJQiIyB4+1J8L3KAgKAiIPCpCW+iGltGW7qTZ9/dHsJSONOPmNkm/n79u03vPOTdNvjk9OfdciuM4AgAA7odu6gYAAED9ENAAAG4KAQ0A4KaaMqD79eu3bt26JmyAm8DzAAD1EiigBw8ePGnSpFoPPvzww4mJicI0wNIGiqIoipLJZAkJCZs2bRKsausEfh4AwFOwTVh3UlKSS8vX6XQSiaTmI88+++zChQu1Wu0333wzZcqUmJiYBx98kN8qHODq5wEAPJS7DHF069ZtyZIlgwcPVqlUCQkJv/zyi+Vxg8Ewd+7c4OBgX1/fBx988NKlS5bHd+3a1alTJ4VCER4enpSUZDAYqst5++23H330UR8fn61bt9aq0d/fPz4+vlOnTgsWLAgKCvrzzz+tVFFcXPzEE0/IZLLY2Ngff/yRoqjk5OS6VTR0+KeffpqQkCCVSlu3bv3yyy9bebDm81BRUTFmzBh/f38fH59nnnmmqKjI+vMDAN6ME8Rjjz02ceLEWg/27dt37dq1lu2uXbsGBQWdPHmS47i1a9eGhITo9XqO4+bMmdOrV69Tp05lZ2cnJSVFRERUVVVxHLdly5ZDhw7l5ub+8ssvkZGRNctRqVSHDx82m80VFRX1tkGv13/55Zc0TX/33XdWqhg+fHi3bt3OnTt35syZnj17EkLOnTtXt4p6D79586ZIJPrvf/+bl5d37ty5HTt2cBxX74O1nocxY8YkJiaeOnXq3Llz3bp1GzJkiPXnBwC8mBsF9KxZsyzbOp2OoqiUlJTKykqJRJKenl59SGRk5I8//lirnO3bt/fp06e6nMmTJzfUBoqiGIahKIqm6U2bNnEc11AVxcXFDMP88ccflgePHDlSM6Crq2jo8OTkZLFYfOvWrZoNqPfBms9DSUkJwzBHjhyp3p8QkpGR0dDzU+9pAoDXcKNpdtHR0ZYNsVjs6+tbWFiYnp6u0+liYmKof2RlZWVnZxNCUlJSnn322YSEhODg4JkzZ169erW6nISEhIaqePrpp5OTkw8fPty5c+fvvvuOENJQFZmZmRzHde7c2XJg165da5ZTXUVDh3fo0KFnz57R0dEvvvjixx9/rNPpCCH1PlhTZmamyWTq0aOH5ceOHTvKZLLqMZO6z48DTzIAeBA3CmiGYWr+aDabTSYTIaS0tLTmR8qkSZMMBsNDDz0UFBT0ySefnD17dvXq1dVj0IQQqVTaUBUqlapDhw79+/f/5JNPfvzxx4MHDzZUhfWmVlfR0OGWjvDnn3/epk2bpKSkBx54wGAw1Pug9Yq4Ghfi131+rB8LAJ7OjQK6rri4OLFY/MMPP9R6PCsrKz8/f9WqVR07dgwJCcnPz7e35Ojo6CeffPLdd99tqIqoqCiKos6dO2f58ezZs3a1kBBC0/S///3vFStW/O9//zt79mxKSkpDD9aslGGYU6dOWX48d+6cVquNi4uz9+wAwDsIN83u1q1blkFVi6ioqEYPUSqVM2fOnD59OkVR3bt3v3Hjxscffzx79uzg4GCZTHb48OHHHnvs/PnzH3zwQa3epS2mTJnSv3//vLy8eqsIDw9/9tlnJ0+evHXrVqPROH/+fEIIRVE2tvDmzZtHjhx55JFHAgMDv/zyS5lMFh4efubMmboP1izN399/1KhRU6dO3bZtm1gsnjhx4pAhQ2x5ogDAKwkX0J9//vnnn39e/WO9vc66Fi1aJBaL58yZc+PGjdatWw8cONDf39/X13f37t3Tpk2bNGlSRETErFmz1q5da297+vbt26FDhw0bNrz33nt1qyCErF+/fuzYsffff39YWNjKlSuffPLJeqc819vCqqqqn3/+edWqVRqNJiEh4auvvlKpVL6+vnUfrFXaunXrpk+f/uijjxqNxkcffdR9rqYBAOFRHJYbtcGpU6f69OlTVlYml8ubui0A0Fw05ZWEbu748eOVlZUdO3bMzc2dPHnyk08+iXQGACEhoBuk1WpnzJiRk5MTGBj42GOPrVmzpqlbBADNC4Y4AADclFtPswMAaM4Q0AAAbgoBDQDgphDQAABuCgENAOCmENAAAG5KiHnQ1bcFqZe/v79arW50XTdeSKVSvV4vzDpwCoWC4ziNRiNAXSzLMgxTd/1SV5BIJFKptKysTIC6CCEKhUKtVgtQEU3TAQEB1l+rPBLsvAghKpWqoqLCaDQKUJdMJtNqtcJM3lUqlSaTSaFQCFBXU0EPGgDATSGgAQDcFAIaAMBNIaABANwUAhoAwE0hoAEA3BQCGgDATSGgAQDcFAIaAMBNIaABANwUAhoAwE0JccurqqoqK7+VSCQGg0GY9TFYljWZTMIsFCASiQghwqwxQtM0RVEmk0mAuhiGYVlWmHU/CCEikUiY55CiKKlUav21yiPBzosIuwSNkG8xsVhsNpstbzRvJcRiSdYXhRGJRFqtFoslOUPgxZIoihJsoR8hF0uSSqXed16EELFYXFVV5X2LJVk6Jd4d0BjiAABwUwhoAAA35XYBfb2cPXNFer1ciLEXAAB35l45eOG6eM8fvpbtkfeVdwjWN217AACakHv1oP+8Iq13GwCgGXKvgBYxd778ZWkhvggGAHBb7hXQ/46tqncbAKAZcq8x6GBf47IhRRVa2kdqZt3rswMAQGjuFdCEEJYmKrkQF5IAALg5twtoD2Uyk4NpiqJKRsKaH07U+EnxGQMAzkJA8+NEluxousyyrTdRI7pXNG17AMALYKCXHzWvrPn7mqQJWwIAXgMBzY/IFncWe+oerm3ClgCA18AQBz+6hWu1Bupygail0vRQvBAr2AGA10NA84MipE9UVZ8ozN0GAN5giAMAwE0hoAEA3JR7DXFo9PSXfynOX5PcG6Ib1lGtEGM2MQA0X+7Vg/4hVX7+moQQcv6a5MdUeVM3BwCgKblXQJdV0fVuAwA0Q+4Vgu0CjfVuAwA0Q+41Bt0vWqMQm3NuidoFGrqH4XIPAGjW3CugaYr0aKvt0RbRDADgZkMcAABQDQENAOCmENAAAG4KAQ0A4KYQ0AAAbgoBDQDgphDQAABuCgENAOCmENAAAG4KAQ0A4KYQ0AAAbgoBDQDgphDQAABuCgENAOCmeFhuVKvVjh49OjIykhDyzDPPdOrUyfkyAQCAn/WgIyMjly1bxktRAABgwU9A5+bmJiUltW7dety4cUqlkhBSXFx89OhRQkhcXFzbtm2tHEvTtFgsZhiGl5ZYJxKJKIriOE6AuliW5ThOKpUKUBdN0zRNUxQlQF0sy9I0Lcx5WaoTpi7Ls+d950UIoShKIpGwrBB357CclzBvMYZhaNrLB2l5+JtJJJIPP/xQqVR+/fXXe/fuffnllwkharX6jz/+IITI5fLo6Ggrh1MUZXnPO9+SRjEMI1hAW85IJBIJUxdFUcIEtKUuYc7LUp0wdVmePe87L+LVbzFhKmpCfD6VZWVlixcvXr16da3Hi4qKrBzl7++vVqsNBgNfzbBCKpXq9Xqz2SxAXQqFguM4jUYjQF0syzIMo9PpBKhLIpFIpdKysjIB6iKEKBQKtVotQEU0TQcEBFh/rfJIsPMihKhUqoqKCqNRiLswy2QyrVYrTG4qlUqTyaRQKASoq6nw8KFa/fe4cOFCcHCw8wUCAADhZYgjIyNj586dUqmUpulp06Y5XyAAABBeArpDhw5r1qxxvhwAAKjJy78DBQDwXAhoAAA35aYBnZ2d3dRNAABoYm4a0AQZDQDNnvsGNEFGA0Dz5tYBTZDRANCMuXtAE2Q0ADRXHhDQBBkNAM2SZwQ0QUYDQPPjMQFNkNEA0Mx4UkATZDQANCceFtAEGQ0AzYbnBTRBRgNA8+CRAU2Q0QDQDHhqQBNkNAB4Ow8OaIKMBgCv5tkBTZDRAOC9PD6gCTIaALyUNwQ0QUYDgDfykoAmyGgA8DreE9AEGQ0A3sWrApogowHAi3hbQBNkNAB4Cy8MaIKMBgCv4J0BTQjJzs5GTAOAR/PagLZARgOA5/LygCbIaADwWN4f0AQZDQCeqVkENEFGA4AHcseAZjIywjZsoEwmfotFRgOAZ3G7gKb0et+RI1vv3Rs3dSpbUsJv4RkZGfwWCADgOm4X0JxYrJk71yyT+Zw92+HFF5UXLvBbflZWFr8FAgC4iNsFNCFEN3Ro2gcf6IOCRIWFcZMnBxw6xG/5GOsAAI/gjgFNCFEnJqbs3l3ZsSOt1UYtWBC6cSMxm3ksHxkNAO7PTQOaEGIIDEzbtKlw2DDCccF79sTMnMlUVvJYPjIaANyc+wY0IYQTiXLmzctatMgskfifONF+xAhZZiaP5SOjAcCdURzHuboOtVpt5bcymUyv15vunlSXnp5e80fF+fPtZs4UFRWZ5fLcRYvKBgxwrCUMw5jN5lqnHBMT41hp1onFYkKIXq93ReG10DRN07TRaBSgLpZlWZbVarUC1EUIEYvFwjyHFEXJ5XLrr1UeCXZehBCZTKbT6cy8DhI2RCQSGY1GAVKFECKRSMxms+WN5q2ECOhbt25Z+a2fn59GozEYDDUfrNu3FRUWRs+Zo7hwgVDUjZEj8yZPJrTd3X+WZU0mU91TjoiIsLeoRikUCo7jNBoN7yXXxTAMy7I6nU6AusRisVQqLS8vF6AuQohcLhfmOaRpWqVSWX+t8kiw8yKE+Pv7V1ZWCvP5LZPJtFqtMAGtVCpNJpNcLhegrqbCClBHo38tjuNq7VP3EH2LFqmbN7d7550W337bevduaWZm1uLFJoXCgcbULTwrK4v3jOb+wW+x1qsTpi5iw9/U4+qy1OJ951Vdl2BPo8B1CVBRE3LrMehaOLE4e8GC/EmTCE37Hz8eN3myuKCAr8IxHg0A7saTApoQQijq2tix6StWmORyRWpq4siRyuRkvspGRgOAW/G0gCaEEFLat2/qjh26sDBRcXH8lClBX37JV8nIaABwHx4Z0ISQqsjIC3v3lvTvTxkMbd95J3L+fJqneQW4FQsAuAlPDWhCiFkuz1y+/PqIEYSiAg8dips2TVRczFfhyGgAaHIeHNCEEI6m86ZNy1y82CyVKv/6K3H0aPnly3wVjowGgKbl2QFtUfzQQyk7d+ratBHfuJE4dmyLb7/lq2RkNAA0IW8IaEJIVVRU6rZtlffeS+n1EYsXt9myhfA0QRIZDQBNxUsCmvyzuFLR4MGE40K2bYuZM4fh6UotZDQANAnvCWhiuZLlzTevzJjBMYz/sWMJY8ZIr17lpWRkNAAIz6sC2uLm8OFpmzcbAgNl2dntR4xQ/fILL8UiowFAYF4Y0ISQyo4dU7dv10RH0xpN1Lx5rffu5aVYZDQACMk7A5oQogsJSd2+vXjAAMpsDtuwIXLhQpqP1R2R0QAgGK8NaEKIWSbLXL48Z948jmUDv/8+YcwY8bVrzheLjAYAYXhzQFsUDhuWsWqVSamUp6fHjBmjSElxvkxkNAAIwPsDmhBS+sADKbt2adu1ExUUxI0f3+L7750vExkNAK7WLAKaEKIND0/ZubO8Tx9ar49YuDB87Vrq7ptsOQAZDQAu1VwCmhBiUiiy3nsvb+pUQtOtPv44fuJEkdP3N0JGA4DrNKOAJoQQiroxalTWwoVmsVh5/nzCSy/J7747rQOwPCkAuEgzC2hCCCG3Hn447cMPDS1bSq5dSxg3LuDnn50vExkNALxz04B2xW22a1K3b39h377y7t3pqqqo119vt3w55fQ9j5HRAMAvNw1oQkhERIRLY9ro53d57drCoUMJIS2/+ipm1iymosLJMpHRAMAj9w1oC5dmNCcW57zxRu6cORzL+v3+e+LYsdKcHCfLREYDAF/cPaCJ67vSBU89den9940qlTQ3N3HsWL8TJ5wsEBkNALzwgIC2cGlGV3TufOGjj9QdOjCVlbGvvRa6cSMxm50pEBkNAM7zmIAmLu5KG1q2TN28uWjIEMJxwXv2xMycyajVzhSY7vQEPgBo5jwpoC1cl9GcWJy9YIFlcSX/EycSxo+X5Oc7UyAyGgCc4XkBTVzclS4cNix97Vqjj48sIyNx1CjfP/5wpjSMdQCAwzwyoC1cl9FlPXqkbdumDQtjy8tjX3215f79zpSGjAYAx3hwQBNXdqWrIiJSd+0q69GDMhjaLVvWdsUKZ65kQUYDgAM8O6AtXJTRRh+f9Pfeu/HCC4SQoC++iJs8WVRS4nBpWLIDAOzlDQFNXNaV5mj66iuvpK9ZY1IofJKTOzz3nM/Zs84UaEtGVxmony7JD5xXXC1hnakLADydlwS0hYu60qV9+lz64AN9q1ZsSUnsjBkBBw86U1qjGf3ZOZ+f0uQnsmUbfvUvqGCcqQsAPJpXBTRxWUar4+NT9uyp6NyZ1umi3nwz9P33nbmSxUpGVxmoC9fF1T9eKhA3tCcAeD1vC2jisuEOg0p16YMPro8cSTguePfuuFdeYZ1YXKmhjJayXM0fWyqdve0LAHguLwxoCxcNSedNnZo7ezbHML6nT8ePHy/Jy3O4tHozmqLIy73LLNsD4jTxrfQOlw8Ano63gM7JyRk6dGhWVhZfBTrPRV3pgqefvrxhg9HPT5aVlTh6tN/p0w4XVW9GRwQaVg4tWjm0aFC8xolmAoDH4y2gP/vss8TERL5K45ErMrq8W7eUnTuroqLY8vKYV15p/dFHDheFuXcA0BB+JnJdvHgxJCTEVOM+2SaTSa1WE0IkEglFUdYPpyiq0X2cERkZSf6JQr4q0oeFpe7ZE758eYtvvw1bv97nf//LXrzYpFTW3MfG88rJyXHyU4T6hzOF2FujYBUJU5elFu87L4GrE/K8BH4OmwTFcVzjezVm0aJFs2bNWr9+/TPPPGNJw4sXL44aNYoQMnr06KlTpzpfBS9SU1N5LpHjWnz4YcuNG4nZrE1MzNuwwRAc7FhJCQkJ/DYNADwdDz3oU6dOJSYmyuXymg+2b9/+zz//tGwXFRVZOdzf31+tVhsMBudb0qiwsDC9Xp+ZmcljmZUvvljatm3km29KU1LaPfVUxvLlFV26EEIkEgnHcXq9rd/ynTlzxuF+NMuyDMPodDrHDreLRCKRSqVlZWUC1EUIUSgUaufWfbURTdMBAQHWX6s8Euy8CCEqlaqiosLo9F03bSGTybRaLS/dvkYplUqTyaRQKASoq6nwMAadnZ197ty5hQsXpqSkbN68uby83PkyXYr3UenSPn0u7t1bFR3NlpTETZ4cvGcPcegFisvBAaAmHnrQzz//vGXjnXfeeeaZZ3x9fZ0v09UsGc1jGupCQ1O3bIlcsMD/xInQjRulV65cX7CAE4kcKCo7O9vVNzUHAI/A5zzopKQkywC0p+A3B01KZfqaNdfHjCEU1eLrryPHj2dv3XKsKPSjAYB48YUqNuJ5rjRN5738cubSpWapVJGcHPPCC/JLlxwrCRkNAM09oC347UoXDxx4ce9eXbt24hs3El96qcW33zpWDjIaoJlDQN/Gb1da27Zt5o4d6o4dKb0+YvHiNps3O7a4EjIaoDlDQN+Fx4w2BgZmbt1quU14yI4dMbNmMZWVDpSDjAZothDQtfHYlbbcJjxr4UKzWOx//Hj7ESNkGRkOlIOMBmieEND147ErfevRRy+/955RpZLk5ydMmOB/4oQDhSCjAZohBPRdLhWIj2XI8kpZwmtXuqJr14u7dmni4pjKypiZM4N37XLgShZXX8ZiNpOv/1bMOdDiozM+pVV4YQA0PbwP7ziWIdt+0ve7i4r1x/zTC29fY8JXRuuDg1O3bi1+6CFiNodu2hS1YAGt1TpQjusy+vcc2fEsGSHk/DXJNxe8+fJZAE+BgL4js+jOhX9nr0qrt/nqSpul0swlS3LmzeNYNuDQofYjRkhzcx0ox0UZfb3szv0P/74mcUUVAGAXBPQdNVculIlqz4rjqytdOGzYpfffN6pU0tzchJde8v3jDwcKcUVGRwTeWa+qa5gQ6y4BgHUI6Dv+HVNl2YgNMvT7Z7sm3oakO3dO2b7dst5/7PTpwXv2OFAI7xndNVz3n06VnUJ1A+I0Q+9xZEYgAPCLn/WgrXOf5UalUqlerzc3fM2ImSOVOtpX2shFJbaEo2W50XK1Ia+MFTEkzN9A3722OK3RRC5cqDp6lBBya9CgnPnzzRK7BxYsnxlYbtR5WG6UF1hulF/oQd+Fpkij6Uxs7kprDdR3KYq/8iV/XpH8kSut9VuzXJ75zjs3XnyREBJ48GDsK6+wJSX2NhjT7wC8GALaQbZ8c3it7E6fOb+M1Rpr356Ho+mr06dnvf22WSz2+d//2o8e7cDiSshoAG+FgHaK9YwWM3f9yDbwZN965JG0LVv0QUHi69cTxo8POHjQ3mZkZmZmOHSNIgC4MwS0s6x0pdv4m9uqbg/8dW6jY+kGB+bUiYkpe/ZUdupEa7VRCxaEbdhA2bC4UrmWLlIzZu52xxxdaQAvg4DmR70ZTVGkW7h2cHv1E/eqI1s08i2oISAg7f33C598khDSeu/emFdfZSoqrOz/9zXJT5fkxzJkx7OkehMyGsALIaB501BXWsJyDGXTl9qcSJSTlJQzbx4nEvmdPJk4dqz0ypV69zSZqcv/XOtYWMnkldy5dRkyGsBrIKB55vxc6cJhw1J27NAHB0tzc9uPHKk6dqzuPlStrxvv/gBARgN4BwQ0/5zPaE1cXOrWrerERFqjiZo7t9W+fbV2oCkusbXesh2kNIWrTLV2QEYDeAEEtEtERETExMQ4U4I+KChty5aixx6jzObwdesiFy6k9fqaOyS00j8Yp+kbXfVApLberx+R0QCeDgHtQk5mtFkszn7rrSszZnA0Hfj99/Hjx4tv3qy5g6/U3EJhohse4Hb1CqUA4FIIaNdyfiW8m8OHp69bZ/LxUaSmJo4a5ZOcbG8JyGgAD4WAFoKTGV12//0pO3dq27YVFRfHTZ4c9MUX9paAjAbwRAhogTjZldaGh6fs2FHWqxdlNLZdsaLdsmWUnctLIaMBPA4CWlDOZLTJx+fy2rV5U6cSmm65f3/imDGS69ftKgEZDeBZENBCc2q4g6KujxyZuXixWSqVX74cP26c4uJFuwpARgN4EAR0E3ByuKP4wQdTt23TBQeLCwvjJ05s8f33dh2OqR0AngIB3WScyWhNbGzK7t0VXbvSen3EwoWh69bZsrhSTchoAPeHgHbQj6mKOQdazDnQIuWGuO5vj2fJpuyTTf1Y/ueV2uv01+RMV9ro73/p/fevjxxJCGn10UfR48aJiovtKgEZDeDmENCOuFwgPnJZZtneddrXeHfn9UY58/Xft2/D83/nlGXaRp5khzOao+m8qVMzlywxS6XK5OTEkSMVaWl2lYCMBnBnCGhHlGjuet40+rt+LK26a6H+sqrGn2SnhqQfeujS9u361q3FBQXxEyeqDh+263BkNIDbQkA7IrrlnTnIcUH6WrcxDFfdNUM52K/2Skb1cma4QxMXd+m//63o0oWuqop+/fXQjRuJPUPSyGgA98QsXLjQ1XVoNBorv5VKpQaDwcqdtnnEsqzJZHL+lsNyMdc+WM9QXGwrw2Pt1aK7b20lYkiXMJ1ULIpqaXq+S5lcfLu6ggrmy/PKM1ekZo4K8av/Fssqlaq0tNTe9lAUxcnlRQMGSPLz5ZmZPn/9JcvJKevVixOJbCyhtLS0tLRUpVI1uifLsizLCnMHcUKIWCwW5o7vFEXJZDLrr1UeCXZehBCZTGb9ZvY8EolEwtw+nBAiFos5jhOL6/kSyGuwje8C9QnxMw69t8EXYqDC9GQXA8dxGs2dd8XqI7fj73KBuIXS1C6g/venpR/tQK/WLJFkLV5cFRsbumlTwM8/S3NzM1av1gUH215Cdna282ulAgBfMMQhELX+rjX2r5Q08tHoYFBS1PWRIy+vWWPy8ZGnpyeOGuX75592FYDhDgD3IUQPmmEYK7+lKIqmaev78MVSEVX7fiSuqovjuOrz8pWRqBbGzKLbT3i7QHOjpxwdHZ2VlWVjXZan0fJjRZ8+abt3R82cKc3Ojp02Le+VVwqGD7e95bm5uZGRkdbrEubvRQgRrC7Ls+d952XBMIzzI3u2sLzFhKmr5mveW1ECPJWVlZVWfiuXy3U6nclk0zdpTrIMkAnz6pFIJBzH6Wussl9QQf94UazRU93aGrq1tWOcLiMjw/oOFEVRFFVrkJFRq8PfeMPv2DFCSPHjj1994w3OntG66Ojoeh9nWVYkElVVVdlelDPEYrH+7jsVuAhFUQqFwvprlUeCnRcR9i1mGVsX8i3m2Bi0wWBYvHjxRx99RAiRy+WDBw9evHixqIHvbKRSaWlpqVQqrd5otHyWZXkZixeiB63Vaq38ViqV6vV6wb4wEezbEks/oua5+4rIM51ufwdl9SmpLTQ01PrIA03TNE3XekEYxOKdb74Ytc08+JPjAV9/Lc7JyVixwhAYaGOlqamppL6RFolEwjCM9b8pjwSri6ZphULhfedFCJHJZDqdTpjv7iiK0mq1wgS05Tt/xwJ6zJgxxcXFp0+fbtmypVar3bJli1qt9vf3t37Ur7/+KpFIHGps/YxGI8taC2Ev/wfBa9g+Cc/ImUuMFWbOnKrN+bL0+KqnIue+PqBKIVGeP99h+HCfc+csu5k5SqOnar2PzBxXYqwwcHfeyRiSBu+Tnp7+xRdf7N69u2XLloQQqVQ6ffp0f3//VatWTZkyxbLPzZs3W7VqVWtWz7/+9S/L/CWKolasWPHCCy907979wIEDlt9++eWXCQkJXbt2XbRoUfUhv//+e9++fbt27XrfffcdOXLE8iBFUW+88cZTTz314YcfVlVVPfvssx07duzSpcsTTzxRq6mYxeFaaTfFJ3OkvlJz/5iqALmz/2NGRERYT8xc3c31BZ8TQmIkocGiAMuDp7q0mfr2Q0/C/x8AACAASURBVJtWn5HcuBH7yivZCxZkPDDol3Q5ISRIaeoarpWLOEKI2qz9qOjgZV0eIeTllkOjpaGWwzG1A7zMuXPnIiMjLelc00svvZSYmLhixQqlUrlly5bhw4fL5fKGComPj587d252dna/fv2GDh1648aNiRMnnj59OjIycsWKFZZ9iouLJ02adOjQodatW1+9erV3796XL1+29MHbt2+/dOlSQsg333yj0+n++usvQkhZWVmtWtCDdqFrZfSOU76pN8Snc6RfJCt5+bfPelYerrg9ZyNdl1douvPHpuM7pu7aVdmxI63VRs2fH7h2E202EUIKKplLN2//h3isPNmSzoSQX8rP1SwW/WhoDgICAh5//PG9e/cajcatW7dOnjzZys6PPPIIISQiIqKoqMhgMPz+++89e/a0fLs+fvx4yz7Hjx+/cePGc889169fvxEjRkgkkqtXr1p+Vd1Zvvfee5OTkydPnvzZZ5/VHe5AD9qFsgrvfP6lF4rKtLS/jIfhbysTpU3cnfKllPhpVb+/NVk+jHyQ330G1idt06a2q1a13L+/24EdPpnpn4xfXSX30Ztuz2nRcHeGRNN0V2qVjH40eI3OnTtnZWUVFhbW7URPmzbthRdeCAoKSkhIsH7T5+qxb4qiLF/AVj9S/WWj2WyOj48/evRo3cOr++Zt27a9cOHCkSNHDh06NG/evPPnz9fstqMH7UJt/O+KY18Jn19O1huXcdLw6u1uivj7le3HBw15LnCAivUhhHAiUc7rr+fOnWtm2bgLv01Z+kzQtcx2AbdHnLvJ46qPHeR3X93CsZA0eIeYmJgnnnhi1KhRN2/eJISo1eqlS5daruC95557AgMDZ8yYUT0YbaNevXqdOXPGUsjXX39tebB3794pKSkHDx60/Hjy5Mm6B+bn5xNCHn/88TVr1qjV6qKiopq/RQ/ahSJamJ+4tzLlhoSmuAGxGt6nbNYdkv6XT8dwcaubxpJ24lat/hmDrqXgP/+pioqKnJPUoiD3lRXPZsnfLu3blxDSThKcFPxCtu56C9YvUhLSUKUZGRkdOnTg90QABLZ79+633367R48eRqNRJpM999xzCsXtFSjHjRv3+uuvDx482K4CW7du/e677w4ZMiQyMrL6MoIWLVp88803s2fPfvXVV41GY6dOnXr27FnrwIsXL86ePZvjOLPZPGXKlPDw8Jq/FWIedK3PhFr8/f3VarUw0+wsU/qEmWanUCg4jhNmbYfc3Ny60+ysE9+8GT17tiItjVBU/rhx18aNI7Zdv2OZB926dWtHG2sfhUKhVqsFqIim6YCAAOuvVR4Jdl6EEJVKVVFRIcw0O5lMJtg0O6VSaTKZqoOVL+PGjYuLi5s9eza/xToGQxzeICoqyt5D9K1apW7fXvjEE4Tj2mzdGjtjBltRYfvhGOsA73Pt2rW4uLj09HR7xzdcBwHtJRq68M8Ky5D01RkzOIbxO3kyfvx4SV6e7YdjSBq8TEhIyKVLl44dO2Zldp3AENDew7EVpW8MH375vfeMfn6yrKzE0aN9z5yx63BkNIDr1B/QtVZaEGzhBXCeAxldft99Kbt2VUVGsuXlsdOnB/3f/9l1ODIaPIvRaKyyh2Crn9dVf0Bb5mBXq/vNI7gzBzJa16ZN6o4dpX36UCZT29Wr2y1bRtnztS0yGjyI2Ww22kOYdabqVTugLU3nOK66cUVFRehBexwHhjtMcnn6qlXXR48mFNVy//74KVPsuk04hqQBeFc7oJcsWSKVSn/99VfpP+Li4kaMGNEkjQMn2d2Vpum8yZMzFy0ySyS3bxOemmpXAchoAB7VDug333zTaDQmJSVV96Bv3bo1f/78JmkcOM+B4Y7iQYMufvSRtl07cUFBwtixrT791K7DkdEAfKl/DHr58uWEEIPBoP2HsK0CPjkw3KFt2zb1ww8runShTKbwNWvC162j7BmGQ0aDFzt//jzDMMnJyQLUVX9A79+/v23btn5+fi3+IUBTwKXszWijSnVp48aCZ54hhLTaty92xgy2vNz2wzEkDZ6E45hfj7D7drHffEnUjdxVZ9myZb179xamXfUH9MyZM/fv36/RaCr/IUxrwKXszWiOZXNnzcqZP58Ti31Pn04cM0Zm2z0SqyGjwSPQyX8yvx6ms9Lpv86yh76zsuevv/4aExNTdxk8VzWs3keVSmXnzp2FaQEIyYHhjsLHH0/ZsUMfHCy5ejVx5MiA76y9fOtCRoP7o6/duYaWvnjeyp4rVqyYNWuW61v0T2PqfXT48OFbtmzB0LO3sjejNbGxF3fvrujShdbr2775Zqu1a4k9C05VZ/Q5Tfp/b/2UrrXjgnIAAZhDQu9sJ97T0G779+/v06ePn5+fII0ipO5qdlQDS5o5szwVVrNzNZZlGYax93one/u2lMHQduXKlgcOEELKevXKXLLEpFTafvgf6tSphg8s219FL+3tc68tR2E1O+dhNbta9Hp97TcLxzGnjlP5V4nSx9inP1Hc9cJmGMayOsfbb7997NgxsVicnJwcFRV14MABV38/V7sHzTXApY2AJmH3kLRIlPPGG1fnz+dY1u/33xNHj5bm5Nh++HlNZp+K2/cE2HvroF1V84UyGpi8XLpYoBQGj0FRpp59jE8NNz48pFY61/TWW28dOXLkxx9/7N279/vvvy/A7Aks2N+sWbl7VkOKnnzS3KZN6Jw50itXEiZOzFi2rKJrV1sOpCmKENKnIu43n0tSWuxYg51BadTK99dYtnU9++h79xe+DeAdPv/8c2Eqqn8Mmr1bYGDgkCFDcuzpLoF1Zo6cuSL96rzydI5UkBEXa+ztSlf07p2yY4e2XTu2pCRu2jQbF1fq63P7a+c+FXEv6P5ldyudJkr5u3pbcvI30nQLLADYqP4e9MqVKymKGjt2LCFk69atFRUVUVFREyZMOHTokLDN81q/Zcq+u3h77KxcRz8YJ8RQtRV1755lnbZt25QdOyIXLPA/caLt6tWKS5dy5s7lxNb6xVGSkHdCJ94ylgWxKpqim+AutLXuOWbbHWQAmlD9PeiPP/741Vdf9fPz8/PzmzVr1tdffz1y5EjBvj9pDjKLRNXbV0vcYqDJ3hl4JqUyfc2aa2PGEIpq8c03CZMmiQoLrR8iotjWokCauv2qs/0jgTIaZN/v91m1SPbFx0zhTdsbWZMh4R5T+O0T1PUdUDuvAdxP/dFQWVl59erVsLAwQkhubq5lNTsaL2j+BCjujGv48Hq3byfZ15Wm6fyXX9bExkYuXqy4cKH96NHpK1eq27e3vTob+9GiP0+zF88TQtisdMJxVU8Nt72KapxMVvWf5+kb+ZxcaQ4IdKAE8A4sy9qVZg3NbRNA/a186623unXrNmzYsGHDht13332LFi1Sq9UPP/ywwI3zYg/Fqe8N0RFC7gnRPZLYxOMbtdg78lAyYEDKtm26kBBRYWH8xImBP/xg1+G2XBROl5dVb7PZGXaVXxPHsqbQtkhnaGi6mrtNY2vwrt7Xr18/efIkIaRnz57BwcHO1IF50K7m2Dxo6xoKTctdvesuEc5oNJELFvj/9hshpHDYsNzZsznWvqGbej8YLPOF2awM2Rf7LI8YOnfXDnyk7p5OwjxoXnjqPGirqudBC49ZuHBhzZ+1Wq3lrS6TyWJiYmJiYmQymdFoZO18s9VkPaSkUqnBYBAmNFmWNZlMwrx6xGIxIUSYDx6apmma5ve+DyqVSqVSlZaW1q2LYZi673ZOJCoZMIAtKVGkpirS0uRpaWW9e1v/2rCW0tJSlUpV60GxWGwwGMyqAHPrYCKVGRPv0fXs44rhY4qiZDKZMB+o5J/zEqYumUwmWL9EJBIJ80lACBGLxRzHie15jVmYTCa73iw0TYtEosb3c4HaL3R/f/8zZ87419EkjYMmZ9dwB8eyuUlJuXPncizrf+JE4pgxdl3JQqwOdxijYrUDH9F37UEYxq4yATxX7YDWarX33Xefto4maRy4A3uHpAv+859LGzcaVSppbm7imDGWQQ+7YH0lAIsG/1XU6XQZGY5/GwPexO4rWbp0ubhrlyYujlGrY2bPDtmxg9g5rISMBvd06tSpgQMHPvjggytXrhSguvoD+ueff46NjX300UcJISdPnnzuuecEaAq4M3tnSeuDg1O3br01aBAxm9ts3hw9bx5t5/AulvwHIZ2suLD46q6Pi342cw0O1mu12pkzZ3711Vc//fTTnDlzBGhV/QE9b968EydOhISEEEJ69uz5119/CdAUcH92ZbRZKs1avPjqtGkcTauOHEl86SVJnt0Ljaanp9t7CIC9jpWdG3TxtVX5+yZmrFxwZVtDux0/ftzf33/cuHFDhw4VJhXrD2iz2RwaemeB1Cacpw3uJjo62q79b4wYkbZ5syEgQJaZ2f7FF1VHj9pbI/rR4GpfFf9avb3heoMLIV2/fj0lJWX79u1r1qyxrIThavUHtFwuv3nz9gW133//fWCgtYn9xcXFc+bMmT9/flJS0pUrV/hvI7iZuLg4u/av7NQpdevWqqgoRqOJSkpqvW+fvTViuANcqpUooHr7If/7GtotICCgW7duSqUyOjq6oqKC34mt9Wrwrt4DBw5MSUn517/+NXLkyFWrVlkpwt/ff8WKFUuWLHnhhRc+/fRT17QT3Iu9Q9K6sLCU7dtL+venzOawdesiFi2i9Hp7K0VGg4tMCX5ycEAvy/bc0Bca2u3+++/Pzs42m83FxcVisZhx/YzP2pefbN++vX///r179z569OiJEyfMZnPv3r2tr0tdfVV7VVWVj4+Pq1oK7seuhTvMcnnGihWtPvkkbN26Ft9+K798OX3VKr2dF6k2wRp40Az4Mop9sQurzDoZLbGyW2Bg4JQpUwYNGqTT6d577z0BGlb7Uu/BgwcfP37c19e3f//+/fr169+/f7t27RotJS8v74MPPrh27drSpUstXy3m5uauWLGCEDJo0CDLbJCGCHl1H03TwlxPRQixfLoK8E8QIYSiKIqihDk1y1WLNa8Wu3Tpkl0l+B46FDp/Pl1VZWjd+sr69VUJCdarq/e87B1msYVIJBLs6j6GYYR5bRCvfotxHOdAN9aDLvWuZy0Ok8l07ty5o0ePHj161PKtZb9+/Xbt2tVoWVlZWdu2bVu2bBkhpLy8/I8//iCEtGvXrlWrVlaOksvlOp1OmBer5TpUYV6pEomEEMLv+hgNqRuarsOyrFgsrnVJtL1T5mWXLkW++qr4xg2zRHLlzTdLHmlwbQ2WZRs6L3u/rrSOoiilUllRUcFjmVZIJBJhXhuEEIVCodVqhXmLicVivf2DV46RSqVms9nyRrOLZwd0tYsXLx4+fHjjxo35+flWFnYxGAyWC9ULCgpWrFixZs2aWjtgsSRXc8ViSQ2RSCRSqbSsrKzur+waIxaVlETPnatMTiaE3HjxxbypU7n6VthoNMj4GvHAYkm8wGJJ/Ko9Bn3x4kVL3zk5OTkmJuZf//rXrl27unfvbqWIy5cv79u3j6Zpg8Ewfvx4V7YW3JpdQ9IGlSpt8+Y2mzYF79nT+qOPlBcuZCxfbrA6X6heGJUGL1a7B01RVI8ePRYsWPDwww/z9R0letCu5iY9aAt751q03L+/7apVlMGgCw1NX7WqKiqqVnW2nJfzGY0eNC88ogdtNBrtGoehaVoqldpbCy9qLzfarVs3s9m8e/fu9evXnz9/vqKiIjAw0Mm5GVhu1NVcsdxoQyz3EbYSmvUuUmqFJj6+vHt3/99/F9+4EfjDD9qICG2N76Utf7JGCyktLa13tVLbYblRXnjEcqM0TVuWNbcRy7JNdbFeg2PQZWVlv/3229GjR/fv309RlDNX3KIH7Wpu1YO2sLcfzZaWRs+b53P2LKGo6yNG5E+ebBmStvfLNIe70uhB88IjetAeNAZd/4UqBQUFhw4d+vHHHw8ePJifn9+mTRuBmwWezt4rWYz+/pc2brz5zDOE44L37Il59VXGoQkVuJgFvEntgH755ZcTExPDw8M3bNgQEBCwfv36kpKSo/avnwBACGkZ3pojtnamOIa5MmtWzrx5HMv6nTyZOHq0zM71/i1wXTh4jdqzOAIDAzds2NCrVy+ZTNYkDQLvUG5ST8pZ81P5GULIZ7LX20pa23hg4bBhVRER0UlJ0qtXE8aMubp8eeH99zvQAMzuAC9Quwe9ZMmSAQMGIJ3BSZsLDljSmRDyoeiQXcdWduqUsmePOj6eUavbzpgRvGePY21AVxo8Hf833wQghBQYS6q3fy7/097OrD4o6NIHH5T27k2ZzaEbN7ZbutSBxZUskNFgC4OJ5JfSal0jszWmTp36yCOP9OvX78iRIwK0CgENLjHUv3f19uSgYcT++RUmhSJ99eqCl14iFNXywIH4yZNFjk6xQEaDdbfU9KwvfFYeUrx+QHn2SoM38D5//nxWVtYPP/ywZ8+e+fPnC9AwBDS4RB+fjj/HrZ0TPHxn5Ly3QkZbHrR3ageh6RvTp19+912TUqk8f77D8OG+f/7pWHsw3AFW/JZ+J5RPZzcY0CqVSqPRWJYbDQoKEqBhCGhwlY7y6Nmtnx/s14um7nqZ2duVLnvggbQPP9QFB7OlpbEzZrT45huHm4SMhnqZa0w1unSzwSuow8LCOnTo0LVr16FDh86bN0+AhiGgoQnYm9GamJiU3bvLu3Wj9PqIxYvD166lHL3aCF1pqOuBqDsXyj3TVdvQbocPH75169a5c+dOnjw5YcIEARqGgAbhUCYTVVZKzGZif0Yb/f0vb9hw87nnCCGtPv445pVXWCeWBkVGQ02tfM2LH6986YGquYPUNcO6lpKSkoCAAEKIr6+vMCvTIqChEVpOf7Dsj2SNs3fXZm5cU767VLllvfyz/1LlZcT+jOYY5sprr2UuW2aWyfxOn27//PPytDSH24OMhpp8pdy9bYwhftb+MxsyZEhRUdHDDz/88MMPL126VIBW1b5QBaAmtVk7ImvJbxV/EUJGt3hkVdhkh4sSn/zNssFcyZacOq596DFi5wqlFsUDB+pCQqLnzBEXFMRPnpy5eHHZAw841iRL1bieBWwkkUgEvu0qetBgzcGyPyzpTAjZVfTDLWO542WZayxKp7szzGf31A5C1ImJKXv2VHbqxFRWxs6cGbxrF3FidR50pcFtIaDBGpa66xttmji+6KIxKrZ629ChU63f2pvRhoCAtM2br48cSczm0E2bYl97zbHFlSyys7OzsrIcPhzARRDQYM0gv/se8rt9P53prZ5SsY6vDG7o1E39wljtw0PUYyaZIqLq7mD3kDRN502demXmTI5h/E6ciJ84UXLtmsPNI4SkpqY6czgA76zdk5AvWA/a1Vy6HrSZM5+vyvRjlBGSYGLzetAOqzXgYMt60L5//BE1bx5bUWH088tctqzc6h3aGkJRlEKhqKysJIKMSmM9aOc5vB40x3F2tZCiqKZasB89aGgETdGd5DGWdBaAA+FYft99qbt2VUVEsGVlsdOnt9q3z8k2YFTau1EURdujqdKZIKDBDTmQ0dqwsJS9e4sefZQymcLXrYuaN4+uqnKmDchocAcIaHBHDkztMIvF2W+9dW38eEJRAYcPx7/8srigwJk24JpDaHIIaHBfdnelKSp//PiMlStNcrkiJSVx1Cjl+fNOtgEZDU0IAQ1uLSYmxt5DSvr2vbh3b1VEhOjWrfiJEx1e778autLQVBDQ4O4cGJLWhYWl7txZ0rcvZTLdXu/f6WlCyGgQHgIaPIADGW2SyzNWrrQMSbc8cCD+5ZdFt2452Qx0pUFgCGhwCSNnWnp9zzMZb07NXZuvL3S+QEfmJlNU/vjxmUuXmqVS5fnziSNHKlJSnG8JMhoEg4AGl9hV9MO6G5/9UnHu0+Ijb+Rv5aVMx64fKR44MHX7dl1wsLiwMH7ChBbff+98S9CVBmEgoMElLlbdya/vSk/yVawD0+8IIZqYmNRt29Tt29N6fcTbb7fZutWZxZWqIaPB1RDQ4BI9le2rt58J+De/hTuQ0YaWLdM+/LDo0UcJx4Vs3RozZw7Dx1X4yGhwKWbhwoWursP6ehRSqdRgMAizPgbLsiaTSZiFAsRiMSFEmDVGLBekmkymxnd1GsuyLMs2uj5Ge1mEivXhOG6gX7e32oyR0mLHqhOLxfU+hyqVqrS01K6iOIYp7dfP0KKF3+nTsqysgMOHy7t1MwYEWH5LUZRYLNbr9fa2sLS0tLS0VKVS2XVUQ+flCjKZTLAlaEQikTCLfhBCxGIxx3GWN5q3Qg8aXGV8yyGfRr+9LHSCH2P3cja2cGxIunDYsMvr1hn9/CRXryZMmOD3+++8NAZdaXAFBDR4MMcyurx795TduzXR0UxFRcxrrwXv3ctLY/DNIfAOAQ2ezbGM1oWEpG7fXjxgAGU2h27YELlgAc3TYq3IaOARAho8nmMZbZbJMpcvz5k3j2OYwIMHE0aPFuXl8dIedKWBLwho8AYOL7FfOGxY+rp1Rh8fWUZGxDPP+J45w1eTkNHgPAQ0eAmHM7qsR4+UXbuqIiOZ0tLY6dOdX1ypGrrS4CQENHgPxy5jIYTowsLSdu6sGDDAsrhS5Ftv0fbPt2sIMhocJsQ9Caus3ttCIpF45TxokUhEBJwHTVGUMPOgGYaxZR40X0QikQPPYXp6ugN1iWm6xcqVLfbuJYRUdu9+ZfVqo7+/A+U0pObSqY6dl2OEvBWnwJcamM1myxvNW+Gmsa7iNTeNrcXJm8aK/zwl+eWQMSpW36W7qV099/auxeGbq9rbb62+aWyL775ru3w5rdfrQkIyVq3S2L8gtRXVHXzcNNZ5Dt801oNgiAOEw+RflfxyiBDCZl6Wf/ZfyuTCyHB4SLroscfSNm82tGwpuXYtYdy4gJ9/5rFVGJUGuyCgQTh08V0rMlOVlS6tzuGMVnfocGHfvvLu3emqqqjXX2+3fDnFa/cTGQ02QkCDcExh4Xe220Waff1cXaPDGW3087u8dm3h0KGEkJZffRUzezbD68eJY6Pk0NwgoEE4Zv8AzfAxxvb3Gjp3rxo0hFCUAJU6nNGcWJzzxhu5c+ZwLOt34kTC2LHSq1d5bBiGO6BRCGgQlKlNWNWjT2gHPsK5vvtczeGMJoQUPPVU2pYthsBAWU5O+xEjVMeO8dgwguEOsAoBDc2CMxld2aFD6vbtVdHRtEYTlZTU6pNPeGwYQVcaGoaAhubCmYzWhYSkbNtmuU14+LvvRixaxOOVLBbIaKgLAQ3NiMOXGhJCzHJ5xooV18aOJRTV4ttv4ydOFBfycDPcmtCVhloQ0NDsON6Vpun8SZMur11r8vFRXLzYfvhwHhdXqoaMhmoIaGiOnBnuKOvVK3XLFl1oKFtWFjtjRssDB3hsmAW60mCBgIZmypmMroqKStm1q7xHD8pgaLd0adtVqygXLISCjAYENHgCs1n82xHZgf+TfX+AKndwGZC6nMloo6/vpfXr86ZOJTQd9Nln8RMmiG7davwwO6Er3cwhoMEDiJL/lJw6zl5OYy/+JT1ykMeSncloQlHXR47MXLrULJMp//47ceRIxcWL/DXtDmR0s4WABg/AFBZUb7PpafwW7lRGE1I8YEDq9u264GBxYWHCxIktvvuOr4bVhK5084SABg9grLGIh7H9vbyX72RGa6KjU/bsKe/WjdLrI95+O3zNGso1S9oio5sbBDR4AGPivboBjxgjovRdumv/PcgVVURGRjpzuNHP7/KGDTeffZYQ0urTT2NmzGArKnhq2l3QlW5WENDgGfRdulc99YJuwCOcVOaiKhISEpw5nGOYKzNnXpkxg2MYv1On4idMkPB0m/C6kNHNBAIa4A4nxzoIITeHD7+8bp3R11eWmZk4erTf6dO8NKwudKWbAwQ0wF2cuRzcorxHj4v79qkTE9ny8tjp00M3biQuu8saMtq7IaAB6uFkRuuDgtI2bSrp359wXPCePZFvvUW77I6R6Ep7MQQ0QP2czGizXJ7xzjv5EycSmg48eDB+wgTeF1eqCRntlRDQAA1ydkiaoq699FL6qlUmhUKRmpo4apTywgWemlaPJuxKU+Vlsu8PyA78H33koOvGc5ohBDSANc5/bVjap8/FvXuroqNFRUXx48e3+r//46VhDWmSjJb+cpC9+Bd7OY0+flR07k/hG+CtENAAjXA+o3WhoalbtpQ+8ABlMoWvXh22bp2LrmSxEL4rzV6+c3knU3hDyKq9GwIaoHHOZ7RJqUxfs+b6mDGEolrv2xcxeTJbXs5L2xoiZEYb23e8sx3WTrB6vR4CGsAmzmc0oem8l1++/O67JqVSefJk++efd9HiStUE60pr/z1I36W7MSLK/PAQV1yL32whoAFsZclo+lqe6Nyfor/O0qUlDhRS9sADaZs2GVq1EhcWxk+Zojp8mO9m1paWxvPyUnVxUqluwCNVT71gvq+Xq+tqVhDQAHaIVsjEF5KZwhvMzeviP044NpSsiY9P37ev8p57aI0m+vXX23zwgatnPmRmZmIenidCQAPYgSq4GVteo+OsrXKsHGOLFmkffFA0ZAjhuJCdO2NmzWIqK/lpYsOQ0R4HAQ1gB3ObUEJIdUY7s3ITJxZnL1iQ9fbbZonE//jx9iNGyDIy+Gllw3DZoWdBQAPYwawK1Dz1gjEqNqJNG90D/Qjt7Dvo1iOPXF63zqhSSfLzEyZM8Dtxgpd2WoeM9hQIaAD7mCKiqp58Tjv4yXYd7uFhagchFV27Xty1SxMXx1RWxsyc2fqjj5wvs1HoSnsEBDSAU3jJaH1wcMr27UWDB1Nmc9j69VHz5tFVDo5u2wUZ7eYQ0ADO4iWjLUPS+RMmEIoKOHw4bsoUUVGR88U2Cl1pd4aABuABLxlNKOrauHEZ77xjlsuVFy60d/HiSjUho90TAhqAH/xkNCEl/funbtumCwkRFRbGT5rU4uuveSm2UehKacEtngAAF+9JREFUuyEENABv+MpoTXT0xX37Svv2pfT6iCVLXLrefy3IaLfCOl9EZmbm1q1bGYYhhLzyyitBQUHOlwngoSIiInjJOJNcnvHOO2Hr17f6+OPAH34Q37yZsXy5UaVyvuRGWdrP14cNOINZuHChs0UwzMCBAwcNGiSRSH755Zfu3bvX2kGj0Vg5XCqVGgwGsyCLfLMsazKZOI4ToC6xWEwIMRgMAtRF0zRN0yaTSYC6WJZlWVYnVIdOLBYL8xxSFCWTyay/Vm2kUqlKS0ut72N5KTZSEE2X9eypa9PG7/ffpXl5gT//XNG5s6FFC3vbIxKJjEajvS/70tLS0tJSlZ0fCZa67DrEYWKxmOM4yxvNW/HQg/bz87NsUBRl6UcTQoqKir777jtCyD333BMXF2flcJqmJRIJy/LQkkaJRCKapoUJaMsZyWSOX2lmO/ofAtTFsixN08Kcl6U6YeqiKIrw9/dKTExMT0+3sgNN0yKRyJaiyocOTU9MjHjtNXFeXuK4cXlJSbeGDbOrMRRFiUQix/pAeXl5MTExtu8vEokoihLsLSbMa74J8RaLarX6s88+mz17tuVHvV6fn59PCAkPD69O7YYI9ixbPkKEefVYPgkaPXe+6qr56eg1dZG7P/VdXREhhMe64uPjL1++bKU621/2uri4jD172s6cqTh3LmzRImlu7o0ZMzh73jV2VVdLZmYmISQ2NtaWnQXrKBDnTspT8PNZZzAYFi1a9Pjjj9cd3yCEFFmdzunv769Wq4X5N1Yqler1emGGUxQKBcdxvPzL3CiWZRmGEWbYQSKRSKXSsrIyAeoihCgUCrVaLUBFNE0HBARYf606oKHxaIlEYu/fizIYwtesCfryS0JIWa9emUuWmJRKWw6Uy+Vardb5l70to9IymUyr1QrTB1IqlSaTSaFQCFBXU+Hh84fjuLVr1/bt27fedAZoznj8qo0TiXKTknKSkjiW9fv998SxY6VXr/JVuC0wD094PAT077//fvbs2WPHji1YsGDPnj3OFwjgTW5nNMexuVmi/50WpV6gnPhfp/DJJ9O2bDG0aCHNyWk/YoTq2DHeGmobZLSQhBjOxxCHq2GIw3kuGuKoduXEb6ILyZZtU6tg+r5ezvy9JNevR8+cKc/I4Bjm6rRpN4cPt7IzX0MctdT7zwGGOPjl5UPsAG4iVlNRvc3cvO5kabrg4NRt20r69aNMpvB164S8kqUautICQEADCMEU3KZ6mX9TqxDnCzTL5RkrV1557TWOpgN/+CFxzBhJfr7zxdoFo9KuhoAGEIKh/b363v0jAwJMIWHG+PZ8FXvzuecyVqwwyeWyjIyEl17ySU7mq2TbIaNdBwENIAiK0vXsU/X0C6FDnmgXH89jwaV9+6bu3KkNCxMVF8dNnhz0xRc8Fm4jdKVdBAEN0ATsujyvUVURESm7dpX17EkZjW1XrGi3bBml1/NYvo2Q0bxDQAM0DX5XIzL5+Fxety5v6lRC0y33708cO1Zy3dmvIh2Qnp6OmOYRAhqgyfC8YhxFXR85MnPxYrNMJr98OX7cOEVKCp/l28yBjKaMRlHaRVHq35ShCfr+bgsBDdCUeF/Vs/jBB1O3bdMFB4sLC+MnTgw8eJDf8m1k36i0yST76hPpN19Iv/1K9uUnlFGIqyI8AgIaoInxntGamJiUjz4q79GD1ukiFywIefttSqglQGuxMaOZwptMTtbt7Ss59LU8VzbKkyCgAZoe7xlt9PG5/O67hcOGEUJUn30WNWcOI8gFmXXZ0pXmxJK7fpZIXdggj4KABnALvGc0JxLlzJuXO2sWxzB+v/6aMGaM9MoVfquwnfWMNgcE6u7vbdnWd+1hahUsSKM8ANbicBWsxcELr1mLo5aGzssVUyBa/v136MyZbGmpyccnc9Gisgce4L2Kao3evcXK5xBVpSEcx8ltXVsDa3EAgKBccSdAdY8eKfv2qTt0YCoqYl97LXTjRiJIH6VeVj6BOJnc9nRuJhDQAO7FFRltCApKe//94oEDCccF79kTtWABrdXyXouNcNmh7RDQAG7HFRltlskyly7NmzKF0HTATz8ljB8vvnGD91psh5i2BQIawB25IqMJRV0fNSrtgw8MKpX80qX2L77oe/o0/7XYAxltHQIawE25JKMJqejcOXXHjqqoKLa8PPaVV4Kb+i5I6EpbgYAGcF8uymhdmzYp27eX9O9Pmc2hGzdGLlgg/Hr/tSCj64WABnBrLspos1ye8c47lsWVAg8eTBg/Xnzzpisqsh0yui4ENIC7c1FGWxZXSl+92qRQyNPSEseOVVy44JKKwFEIaAAP4KqMJqS0d+9Lmzbpg4JEhYXxkycH/PSTiyoCByCgATyD6zJanZCQsnt35b330lpt1Pz5oRs3Uk13JQvUhIAG8BgREREuimlDYGDahx9eHznSciVL3KRJouJiV1QEdkFAA3gYF2U0xzB5U6fmzp3LsaxPcnL8+PEyfGvX1BDQAJ7HyYy2sjx0wX/+c2nTJkNAgPTq1YSxY/1/+82ZisBJCGgAj+RYRtMV5dJD30qO/Cj+8xTVwFKLFZ06pezerY6PZ9TqmNmzQ3buJK5f8xLqhYAG8FQOZDSTddmyQRcXsVnpDe2mb9Uqddu2wscfJ2Zzmw8+iH3tNaay0vGGgqMQ0AAezO6MNtXoC5usLcLOicU58+fnzJvHsazfiROJo0dLc3IcaSI4AQEN4NnsymhzUKvbWxwxtW7T6P6Fw4Zdev99g0olvXIlYdy4Jl9cqblBQAN4PNsz2hQaru92vzE2UdfjAbNtd5Zyt8WVmhUENIA3sD2jzQEtjO0iOX+V7YXr2rRJ3bKlrFcvy+JK7d55hxLkHnWAgAbwEq671JAQYvLxSX/33esjRhBCWn75ZfyUKbiSRQAIaADv4dKM5mg6b9q0rMWLzRKJMjk5ceRIRWqq66oDgoAG8DKNZDTHMflXRakXmOv5js1uvjVoUOrWrfrWrcUFBfHjxwd+/72DDQUbIKABvI2VjGazM0UX/2Ku5oj+PsfkX3WsfE18/MXduyu6dKH1+siFC8Peew+LK7kIAhrACzWU0VRpSfU2XVjgcPlGlerSxo0FTz9NCGn93//GvPoqU1HhcGnQEIpz/UWcVVVVVn4rkUgMBoNZkE9glmVNJpMAp0wIEYlEhBCDIF920zRNUZTJZBKgLoZhWJbVCXWHJJFIJMxzSFGUVCq1/lrlkTDnlZ6eTmq97M/+QV273XHm2kWRezo5WYX/jz+GvvkmrdPpQ0Nz3ntPHxvrzHs5JibG9p3FYrHZbLa80byVEAFdVFRk5bf+/v5qtVqYN6FUKtXr9cJ8GCgUCo7jNA0sd8AvlmUZhhEmNCUSiVQqLSsrE6AuQohCoVCr1QJURNN0QECA9dcqjwQ7r+zsbLlcrtVqLS97qkrDpqUwhTdMrYKNCR04scT5KnzOnYtOSmJLSkw+PjnvvFNy330Op4pdX3IqlUqTyaRQKByryyNgiAPAm9WKPE4mN3Tupn1osKFjV17SmRBS0blzyq5dmuhopqIictq01nv2YHElviCgAbxcfHy8q6vQBQenbttWMmAAZTaHbtgQuWABrdW6utLmAAEN4P2ioqJcXYVZLs9Ytuz6lCmEpgMPHUoYP158/bqrK/V6CGiAZsGl17DcRlE3x41LX73apFTKL11qP3q0z//+5/JKvRoCGqC5ECKjCSnr0ydl505t27ZsSUnc1KlBX3whQKXeCgEN0IwIk9Hatm0v7t5d8u9/U0Zj2xUrIufPp4Wal+llENAAzYswGW2WyzOWL8+bOvX2kPS4ceIbNwSo18sgoAGaHWEymlDU9ZEj09esMSkU8kuXEseOVV64IES9XgQBDdAcRURECBPTpQ88kLp1q65NG1FRUfykSS2+/lqASr0GAhqg+RImo6uio1O3b6/s2JHS6yOWLg3dtIlgcSXbIKABmjVhMtoQEJC2aVPh0KGE44J37YqZORO3CbcFAhqguRMmozmRKOeNN3Jnz+ZY1v/EicQxY3Cb8EYhoAFAqK8NCSl4+umUHTv0rVtLc3PbjxoVcPiwMPV6KAQ0ABAiYEZr4uNTt2zRxMfTVVVRb7wRsmMHFldqCAIaAG4TLKP1rVunbt16a9AgYja32bw56o03sLhSvRDQAHCHYBltlkiyFi++On06R9MBP/+cMGGC+OZNYar2IAhoALiLYBlNCLnx4ovp771n9PWVp6Uljh4tOnNGsKo9AgIaAGoTMqPLevS4uG+fOjGRrajA/Oha2KZuAAC4o4iIiOzsbGHq0gcFpW3a5JOcHNCjhzA1egr0oAGgfkL2o81yeVmvXoJV5ykQ0ADQICEzGupCQAOANcjoJoSABoBGIKObCgIaABqHjG4SCGgAsAkyWngIaACwFTJaYAhoALADMlpICGgAsA8yWjAIaACwGzJaGAhoAHAEMloACGgAcBAy2tUQ0ADgOGS0SyGgAcApyGjXQUADgLOQ0S6CgAYAHiCjXQEBDQD8QEbzDgENALyJiYlp6iZ4FR4C2mQyzZkz5/nnnz98+LDzpQGAR4uIiEBXmi88BDRN00lJSU888YTzRQGAd0BG84KHm8ZSFBUQEFDrQb1eX1hYSAjx8fFhGMb64TRNW9+HLzRN0zRNUZQwdXEcJ+R5CVYXRVHC1EUIEawumqYJId53XhYMw3AcJ0BFlvOy1BUdHZ2VlWXX4XY9J5bosK99nsZVd/XOysqaPHkyIeT5558fN26clT0pilIqlS5qRl0ymUyYiiiK4jhOIpEIUx0hRC6XC1MRRVH+/v7C1EUIEfI59MrzasK3WJcuXVJTU20/1q7n3/IWs6NlHshVAR0fH3/kyBHLdlFRkZU9/f391Wq1wWBwUUtqkkqler3ebDYLUJdCoeA4TqPRCFAXy7IMw+h0OgHqkkgkUqm0rKxMgLoIIQqFQq1WC1ARTdMBAQG3bt0SoC4i4HkRQlQqVUVFhdFoFKAumUym1Wpr5mZQUFB2draNh9v1/CuV/9/evYc09f5xAP8cb7NaF3N2NVNzUVJNK6VClFj9YZRdsAwWZnSBjIj+GGVWlJBoFEZ2QTJUtDCkMAOhC2Y3i1qgssSmk65YNpdhNm2X8/vjfNnXn5t+09Y5p8P79dfxuD3P5/Ejb45n7pncbrePGTNmeCX+VST+BwIACA73o0fMM1fQubm5RqPR19fXaDTu2rXLI2MCgGSEhYX9+nU0OHkmoA8cOOCRcQBAqpDRI4BbHADAE9zrGC4ENADwBxk9LAhoAOAVMvrXIaABgG/I6F+EgAYAASCjfwUCGgCEgYz+TwhoABAMMnpoCGgAEBIyeggIaAAQGDJ6MAhoABAeMtotBDQAiAIy2hUCGgBApBDQAAAihYAGABApBDQAgEghoAEARAoBDQAgUghoAACRQkADAIgUAhoAQKQQ0AAAIoWABgAQKQQ0AIBIIaABAEQKAQ0AIFIIaAAAkUJAAwCIFAIaAECkENAAACIlfEDfvXu3o6ODn7nsdjvLsvzM1dDQ0NTUxM9cDofDbrfzM9fHjx9ra2v5mYuIrFYrPxP19fVVVFTwMxfxuC4iqq6uNpvN/MzF2+8hEel0utevX/M2nSB8eJhDoVAM8d2ysrJ9+/YplUoeKuFTcXHxuHHjFi9eLHQhHtbQ0HDjxo2VK1cKXYiHmc3m06dPb9y4UehCPK+oqOj48ePh4eFCF+Jh9+/fnzlz5sKFC4Uu5A8S/goaAADc8j527JiwFQQHByuVylGjRglbhscpFIqIiIiAgAChC/EwuVyuVCqnTp0qdCEe5u3trVQqJfnB0jNmzFAqlf7+/kIX4mFBQUFKpXLChAlCF/IHMbzdkwUAgGHBLQ4AAJHi40XCAex2e0ZGxvv373fs2KFWq7mTVVVVL1++ZFl29+7df+mfz67r6u3tTUtL416c2bRpU1RUlNA1joTRaLx06ZK3tzcR7du3b9KkSSSJfrmuSxr9IiKz2ZyTk+Pn52ez2dLT00NCQkgSLXNdl2RaNiiWdw6Ho7Ozs7y8/N69e9wZk8mk1WodDofBYMjOzua/JI9wXZfFYsnIyBC2qt/X1dVlsVhYln306NH58+dZqfTLdV3S6BfLsna73eFwsCzb2Nh48uRJViotc12XZFo2GAFucTAMM3HixP5nmpub582bxzCMUql8+/Yt/yV5hOu6iOjt27cHDx48c+bM9+/fBanq940fP557fYlhGO56Uxr9cl0XSaJfROTl5cUwDBFZLJaxY8eSVFrmui6SSssGI4p70N+/fx89ejR37HA4hC3Gg2QyWUFBQU5OTnh4eGlpqdDl/Jaenp6KiorVq1eTtPrVf11S6teHDx8yMzMvXryYlJREEmrZgHVJqWVuiSKg5XL5jx8/uGMvL1GU5BEMw8jlciJKSEgwGo1ClzNyVqs1JydHo9FMnz6dJNSvAeuSTL+IKDg4+MSJE0eOHDl37hxJqGUD1iWllrklilbNmTNHr9ezLGswGEJDQ4Uux2N6e3tZliUivV7/l74sQ0Qsy+bl5SUkJMTExHBnpNEv13VJo1/U733kcrm8r6+PpNIy13VJpmWDEeC/OIgoNzfXaDT6+voajcZdu3YFBgbGxcUdPXqUiNLT0wUpySMGrKu1tbWoqMjf39/Ly2vv3r1CVzdCdXV1L1++7O7ufvDggVKpTE1NlUa/XNcljX4RkcFguHr1qpeXl9Vq3blzJxFJo2Wu65JMywaDN6oAAIiUKG5xAACAKwQ0AIBIIaABAEQKAQ0AIFIIaCAiUigUM2fOdL6FobCwkGEY7l9N/f39e3t7+x8I5efPn0ePHp01a1ZoaGhkZOSWLVtaW1uHeLx4KgcYGQQ0/EOhUNTU1HDHxcXFzg+qePjwoUwm478em8024MzWrVt1Ol1dXd2bN28aGxtXrFhRX1/Pf2EAvEFAwz+2bdtWXFxMRC0tLTabbe7cudz5+Ph47k0BTnV1dQkJCYsWLYqNjeUy3WKxpKSkqFSqhQsXrlu3znVwhmG0Wm1qampcXFxlZeVg43CPzMzMTE5OLigo6D+CwWCorKwsKSmZPHkyEfn4+KSlpSUnJ3Pf1Wg0ixcvVqlU69ev//r162BrrK6ujo6OXrBggVqtdl59MwyTm5ur0WhiYmJu3rw53J8bwB8k2DZNICaBgYEtLS3h4eHfvn07dOjQhQsXNBpNfn4+y7IymYzb9Y076OzsnD9/fnt7O8uy796947Z8rKqqWrt2LTdUV1eX6/hEdOXKFZZlTSbTjBkzPn/+7Hac/o8c4Nq1a5GRkYPV39HRwR1kZ2c7tzcbUHl7e7tCoXj9+jXLsgUFBbGxsc7aKisrWZZta2sLCQkZwU8P4A8R5p2EIEI+Pj4bNmwoLy+vqKh4/vz5kydP3D7s8ePHnz592rx5M/elTCZ7//79ggUL6uvr09PTly9fvmrVKrdP5Ha3CQwMjI6OfvbsGRG5jhMREUFEbq/B+2toaEhJSbFYLElJSfn5+UR0/fr1q1evsizb3d0dHBzs9llPnz5dtGjR7NmziWj79u179+7t7u7mNkVLTEwkorCwMJPJZLVafX19hy4AgB8IaPjXtm3b4uPj1Wr1EJ/z5nA45syZU1tbO+C8Xq+vqam5c+dORkZGY2Ojc+80J+dGClarlWEYu93udhwicn0uEUVFRbW1tX358iUoKEilUjU3N586dUqv1xORTqfLy8t79uxZQEBAVVXV2bNnh7FmIiLy8/PjDrjCENAgErgHDf+KjIzMysrKzMwc4jFxcXFNTU23b9/mvnz69CkRffz4kYiSkpJOnz7d09NjMplcn3j58mUiamlpefHixZIlS9yOM4TZs2evWbNm69at7e3t3Bmz2ew8mDp1Kvf5vOXl5YONsHTpUp1O19zcTESFhYXR0dHOPYUBxAlX0PB//nMnHYVCcevWLa1Wu3//fpvNFhUVtXTp0levXmm1WpZlHQ7Hnj17uM9YGqCnp0elUvX19V26dCkoKIiIXMcZeurS0tKsrKxly5ZZrdaJEyfOnz//8OHDRKRWq4uLixMTEwMCAqZNm9bR0eH26VOmTCkpKdm8efPPnz+nTJlSVlb2Sz8RAOFgsyTgA8PgNw1g2HCLAwBApHBdAwAgUriCBgAQKQQ0AIBIIaABAEQKAQ0AIFIIaAAAkfofIbO1EOE0ZBsAAAAASUVORK5CYII=)

Another  type of regression utilizes the Gaussian model. Instead of a straight  line, the Gaussian model fits a (possibly not straight) curve. To use  the Gaussian model, we pass the `auto` parameter to the `method` attribute

```r
ggplot(mtcars,aes(x=mpg,y=wt,color = cylFactor)) + geom_point(shape=19) + 
  geom_smooth(method="auto", se= TRUE, color = "red") + xlab("Miles per Gallon ") + 
  ylab("Weight") +  labs(colour = "Cylinders") + ggtitle("Gaussian Regression")
`geom_smooth()` using method = 'loess'

```

![img](data:image/png;base64,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)

#### Box Plots

### geom_bloxplot()

We create a plot with the ggplot function and specify the x and  y-axis of the plot. Then we add the boxplot to our plot, which results  in creating one boxplot for each value of x.

```r
ggplot(df, aes(x=label, y=value)) + geom_boxplot()

ggplotly()

```

![img](data:image/png;base64,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)

# Basic Concepts in Big Data



Big data refers to large volume of unstructured data, too large for traditional processing.

Big data enables organizations to store, manage, and manipulate vast amounts of disparate data at the right speed and at the right time.

Big data can be described by the following characteristics:

**Volume**
    The quantity of generated and stored data. The size of the data determines the value and potential insight, and whether it can be considered big data or not.

**Variety**
    The type and nature of the data. This helps people who analyze it to effectively use the resulting insight. Big data draws from text, images, audio, video; plus it completes missing pieces through data fusion.

**Velocity**
    In this context, the speed at which the data is generated and processed to meet the demands and challenges that lie in the path of growth and development. Big data is often available in real-time. Compared to small data, big data are produced more continually. Two kinds of velocity related to big data are the frequency of generation and the frequency of handling, recording, and publishing.

**Veracity**
    It is the extended definition for big data, which refers to the data quality and the data value. The data quality of captured data can vary greatly, affecting the accurate analysis.

Data must be processed with advanced tools (analytics and algorithms) to reveal meaningful information. For example, to manage a factory one must consider both visible and invisible issues with various components. Information generation algorithms must detect and address invisible issues such as machine degradation, component wear, etc. on the factory floor.

![https://cdn.intellipaat.com/mediaFiles/2018/12/Big-Data-Cheat-Sheet-1.png](https://cdn.intellipaat.com/mediaFiles/2018/12/Big-Data-Cheat-Sheet-1.png)

# Basic Concepts in Cloud Deployment

Cloud computing is a model for enabling convenient, on‐demand network access to a shared pool
of configurable computing resources (e.g., networks,servers, storage, applications, and services) that can be rapidly provisioned and released with minimal effort or service provider interaction.

Containers: Containers offer a logical packaging mechanism in which applications can
be abstracted from the environment in which they actually run. This decoupling allows
container-based applications to be deployed easily and consistently, regardless of whether
the target environment is a private data center, the public cloud, or even a developer’s
personal laptop. Containerization provides a clean separation of concerns, as developers
focus on their application logic and dependencies, while IT operations teams can focus on
deployment and management without bothering with application details such as specific
software versions and configurations specific to the app.

![img](https://cloud.google.com/images/containers-landing/containers-101.png)

Docker: **Docker** is a **tool** designed to make it easier to create, deploy, and run applications by 
using containers. Containers allow a developer to package up an application with all of the parts it needs, such as libraries and other dependencies, and ship it all out as one package.

Kubernetes: Kubernetes is an open-source container-orchestration system for automating application deployment, scaling, and management.