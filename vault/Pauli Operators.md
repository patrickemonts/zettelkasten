#Pauli 

Pauli operators are the basis of complex Hermitian matrices. They are
$$
\sigma_X = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} \qquad
\sigma_Y = \begin{pmatrix} 0 & -i \\ i & 0 \end{pmatrix} \qquad
\sigma_Z = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix} 
$$
Occasionally, Pauli operators are referred to as simply X, Y, Z. 

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

The Pauli group is defined as 
$$
\mathcal P = \{ \pm I , \pm i I, \pm X , \pm i X, \pm Y , \pm i Y, \pm Z , \pm i Z\}
$$

# Links
- [[Clifford group]]

# References
- 