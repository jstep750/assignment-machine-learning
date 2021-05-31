## Principal Component Analysis (PCA)

### 1. Problem definition

#### (1). Data

- the given data consists of $`\{ (x_i, y_i) \}_{i=1}^n`$ where $`z_i = (x_i, y_i) \in \mathbb{R}^2`$ represent a point in 2-dimensional coordinate.

#### (2). Normalization

- the data should be normalized in such a way that features $x$ and $y$ have mean = 0 and standard deviation = 1

```math
    x = \frac{x - \mu_x}{\sigma_x}, \quad 
    y = \frac{y - \mu_y}{\sigma_y}
```

- $`\mu_x`$ denotes the mean of $`x`$
- $`\sigma_x`$ denotes the standard deviation of $`x`$
- $`\mu_y`$ denotes the mean of $`y`$
- $`\sigma_y`$ denotes the standard deviation of $`y`$

#### (3). Covariance Matrix

- compute the co-variance matrix 

```math
    \Sigma = \frac{1}{n} \sum_{i = 1}^n z_i z_i^T = \frac{1}{n} Z^T Z
```
    
- $`n`$ denotes the number of data
- $`Z = \begin{bmatrix} z_1^T \\ \vdots \\ z_n^T \end{bmatrix}`$

#### (4). Principal Components

- compute the eigenvector and the eigenvalues of the covariance matrix

```math
\Sigma u = \lambda u
```

- $`u`$ denotes an eigenvector and $`\lambda`$ denotes an eigenvalue of matrix $`\Sigma`$

### 2. Complete the notebook 

- download the notebook file [assignment_12.ipynb](https://gitlab.com/cau-class/machine-learning/2021-1/assignment/-/blob/master/12/assignment_12.ipynb) 
- download the data files [assignment_12_data.txt](https://gitlab.com/cau-class/machine-learning/2021-1/assignment/-/blob/master/12/assignment_12_data.txt) 
- complete the `codes section` in the notebook so that the results in the `results section` in the notebook can be produced as expected
 
### 3. list of submission

- completed notebook file in PDF format
- github history in the course of completiing the notebook file in PDF format
- it is required to make `git commit` and `git push` at least once in every 10 minutes