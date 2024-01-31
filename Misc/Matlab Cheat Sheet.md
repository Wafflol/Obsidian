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
- det(diag(v)) = product of the entries in v

### Linear Algebra things
##### Shortest distance between lines
$L_{1} : \begin{bmatrix}5\\2\\1\end{bmatrix}+t\begin{bmatrix}-1\\1\\2\end{bmatrix}$, $L_{2}: \begin{bmatrix}0\\-1\\2\end{bmatrix}+s\begin{bmatrix}4\\2\\-1\end{bmatrix}$
```
P = [5 2 1]; Q = [0 -1 2];
n = cross([-1 1 2], [4 2 -1]);
PQ = Q - P;
distance = abs(dot(PQ, n)/norm(n))
```

##### Surface Area of a tetrahedron
###### Area of a triangle
- ```areaABC = norm(cross(AB,AC))/2;```

