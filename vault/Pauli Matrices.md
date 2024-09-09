#physics #quantum-information #quantum #condensed-matter 

The Pauli matrices are given by the three matrices

$$\sigma_x=\begin{pmatrix}0&1\\1&0\end{pmatrix}$$
$$\sigma_y=\begin{pmatrix}0&-i\\i&0\end{pmatrix}$$
$$\sigma_z=\begin{pmatrix}1&0\\0&-1\end{pmatrix}$$

In quantum information, the Pauli matrices are commonly referred to as simply $X$, $Y$, $Z$. 

All Pauli matrices are [[Hermitian Matrix| Hermitian]] and together with the $2\times 2$ identity, they form a basis for the real vector space of Hermitian matrices.
Furthermore, they fulfill the following commutation relations
$$[\sigma_i,\sigma_j]=2i\epsilon_{ijk}\sigma_k,$$
where $i,j,k\in\{x,y,z\}$ and $\epsilon_{ijk}$ is the fully anti-symmetric Levi-Civitas symbol.

Any Hermitian matrix can be written as
$$
H = \vec a \cdot \vec\sigma = a_x \sigma_x + a_y \sigma_y + a_z \sigma_z
$$
Pauli operators satisfy the properties
$$
\begin{matrix}
\operatorname{tr}(\sigma) & = 0 \\
\operatorname{det}(\sigma) & = -1 \\
\sigma^2 & = I \\
-i \sigma_X \sigma_Y \sigma_Z & = I \\
[\sigma_i, \sigma_j] & = 2 i \epsilon_{ijk} \sigma_k \\
\{\sigma_i, \sigma_j\} & = 2 \delta_{ij} I  
\end{matrix}
$$
The eigenvalues of the Pauli operators are
$$
\begin{matrix}
\ket{+_X} = \ket{+} = \frac{1}{\sqrt 2}\begin{pmatrix}1 \\ 1 \end{pmatrix} & 
\ket{-_X} = \ket{-} = \frac{1}{\sqrt 2}\begin{pmatrix}1 \\ -1 \end{pmatrix} \\
\ket{+_Y} = \ket{+i} = \frac{1}{\sqrt 2}\begin{pmatrix}1 \\ i \end{pmatrix} & 
\ket{-_Y} = \ket{-i} = \frac{1}{\sqrt 2}\begin{pmatrix}1 \\ -i \end{pmatrix} \\
\ket{+_Z} = \ket{0} = \begin{pmatrix}1 \\ 0 \end{pmatrix} & 
\ket{-_Z} = \ket{1} = \begin{pmatrix}0 \\ 1 \end{pmatrix} \\
\end{matrix}
$$

# Links
- [[Clifford group]]

# References
-  Michael A Nielsen, Isaac L Chuang,; Quantum computation and quantum information (cambridge series on information and the natural sciences); (2004);  @nielsen_quantum_2004 
