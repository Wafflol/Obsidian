### Normal Functions
- norm(w) = magnitude
	- sqrt(dot(w, w)) also works
- dot(u, v) = dot prod
- cross(u, v) = cross prod

### Matrix syntax
- Separate columns with a space ( ), and rows with a semicolon (;)
- Creating a matrix:
	- A = [1 2 3; 4 5 6; 7 8 9]
	- Will create $\begin{bmatrix}1&2&3\\4&5&6\\7&8&9\end{bmatrix}$
- Accessing contents:
	- A(2,3) gets 2, 3 indexing at 1
	- end gets last row/column
		- ex. A(1, end) gets 1st row last column
		- can do math
			- ex. A(end-1, 1)
	- colon (:) gets entire row/column
		- ex. A(1, :)
### Matrix functions
- eye(n) creates an identity matrix of size n
- diag(v) creates a matrix with entries of v along the diagonal
	- ex. diag([1 2 3]) makes $\begin{bmatrix}1&0&0\\0&2&0\\0&0&3\end{bmatrix}$
- ones(n) creates a matrix of ones of size n
- zeroes(n) creates a matrix of zeroes of size n
- det(A) = determinant

### Function Combinations
- det(diag(v)) = product of the entries in v

##### Shortest distance between lines
$L_{1} : \begin{bmatrix}2 & 3 & &2\end{bmatrix}$