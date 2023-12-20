#quantum-information #quantum #physics 

A projective [[Measurement|measurement]] on some space, with $m$ possible outcomes, is a set of projectors $P_1,\dots , P_m$  acting on the same space  $V$ and that sum to identity, $\sum_{j=1}^m P_j = I$.
For a projective measurement these projectors are pairwise orthogonal, meaning that $P_iP_j = 0$ if $i != j$. 
The projector $P_j$ projects on some subspace $V_j$ of the total Hilbert space V , and every state $\ket{\phi}\in V$ can be decomposed in a unique way as $$\ket{\phi}=\sum_{j=1}^m \ket{\phi_j}$$, with $\ket{\phi_j}=P_j\ket{\phi}\in V_j$. 
Because the projectors are orthogonal, the both subspaces $V_j$ and the states $\ket{\phi_j}$ are orthogonal.
When we apply the measurement to a pure state $\ket{\phi}$, then we will get outcome $j$ with probability $$||\ket{\phi_j}||=\mathrm{Tr}(P_j\ket{\phi}\bra{\phi}=\bra{\phi}P_j\ket{\phi}$$ and the measured state will then "collapse" to the new state $$\ket{\phi_j}/||\ket{\phi_j}|| = P_j\ket{\phi}/||P_j\ket{\phi}||$$
## Example
The measurement in the computational basis is given by the two projectors $$P_0 = \ket{0}\bra{0} = \begin{pmatrix}1&0\\0&0\end{pmatrix}$$
and
$$P_1 = \ket{1}\bra{1} = \begin{pmatrix}0&0\\0&1\end{pmatrix}.$$
The two projectors sum to identity as expected.
# Links
- [[Measurement]]
- [[Positive Operator Valued Measure (POVM)]]
- 

# References
-  Ronald de Wolf,; Quantum Computing: Lecture Notes; (2023); [10.48550/arXiv.1907.09415](https://www.doi.org/10.48550/arXiv.1907.09415);  @de_wolf_quantum_2023 
