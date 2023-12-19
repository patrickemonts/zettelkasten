#quantum #quantum-information 

In analogy to [[Logic Gates]], unitary matrices that act on only few qubits are called *quantum gates*. These quantum gates are used as building blocks of [[Quantum Circuit|quantum circuits]]. 

## Single qubit gates
Typical gates are 
- $X$ $$X=\begin{pmatrix}0 & 1\\ 1 & 0\end{pmatrix}$$
- $Z$ $$Z=\begin{pmatrix}
1 & 0\\ 
0 & -1
\end{pmatrix}$$
- The $Z$ gate is a special case of the *phase* gate which rotates the $\ket{1}$ state by an angle $\phi$ $$R_\phi=\begin{pmatrix}1 & 0\\ 
0 & e^{i\phi}\end{pmatrix}$$
- $T$, a special case of $R_\phi$ with $\phi=\pi/4$.
- Hadamard gate $H$ $$H=\frac{1}{\sqrt{2}}\begin{pmatrix}1 & 1\\ 1 & -1\end{pmatrix}$$
## Two Qubit Gates
- Controlled NOT gate, flip the *target* qubit depending on the *control* qubit $$CNOT=\begin{pmatrix}1 & 0 & 0 & 0\\0 & 1 & 0 & 0\\0 & 0 & 0 & 1\\0 & 0 & 1 & 0\end{pmatrix}$$
# Links
- [[Logic Gates]]
- [[Pauli Matrices]]

# References
-  Ronald de Wolf,; Quantum Computing: Lecture Notes; (2023); [10.48550/arXiv.1907.09415](https://www.doi.org/10.48550/arXiv.1907.09415);  @de_wolf_quantum_2023 
- Michael A Nielsen, Isaac L Chuang,; Quantum computation and quantum information (cambridge series on information and the natural sciences); (2004);  @nielsen_quantum_2004 
