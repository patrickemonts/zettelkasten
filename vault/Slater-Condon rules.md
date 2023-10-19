#chemistry #physics

Slater-Condon rules can help you to express matrix elements of one- and two-body fermionic operators in terms of one- and two-body integrals. More specifically,  suppose you have $N$ electrons and $M$ spin-orbitals. A if you have a single slater determinant where $N$ spin-orbitals are occupied, including two with indices $m$ and $n$. 
$$
\ket{\Phi(\mathbf{r}_1, \mathbf{r}_2, \dots, \mathbf{r}_N)} = \frac{1}{\sqrt{N!}}\begin{vmatrix}
\phi_1(\mathbf{r}_1)& \phi_2(\mathbf{r}_1)& \cdots & \phi_N(\mathbf{r}_1)\\
\phi_1(\mathbf{r}_2)& \phi_2(\mathbf{r}_2)& \cdots & \phi_N(\mathbf{r}_2)\\
\vdots & \vdots & \ddots & \vdots\\
\phi_1(\mathbf{r}_N)& \phi_2(\mathbf{r}_N)& \cdots & \phi_N(\mathbf{r}_N)
\end{vmatrix} \equiv \ket{\phi_1 \phi_2 \dots \phi_m \phi_n \dots \phi_N}
$$
where $\mathbf{r}$ is a composite spatial and spin variable. This determinant could be for example a Hartree-Fock determinant. We define a singly excited determinant by
$$
\ket{\Phi_m^p} = \ket{\phi_1(\mathbf{r}_1) \phi_2(\mathbf{r}_2) \dots \phi_p(\mathbf{r}_m) \phi_n(\mathbf{r}_n) \dots \phi_N(\mathbf{r}_N)}
$$
And a doubly excited determinant
$$
\ket{\Phi_{mn}^{pq}} = \ket{\phi_1(\mathbf{r}_1) \phi_2(\mathbf{r}_2) \dots \phi_p(\mathbf{r}_m) \phi_q(\mathbf{r}_n) \dots \phi_N(\mathbf{r}_N)}
$$
Then if you have a one-body operator on an $N$-particle system
$$
\hat{F} = \sum_{i=1}^{N} \hat{f}(i)
$$

The Slater-Condon rules are:
$$
\begin{aligned}
\langle\Phi|\hat{F}| \Phi\rangle & =\sum_{i=1}^N\left\langle\phi_i|\hat{f}| \phi_i\right\rangle \\
\left\langle\Phi|\hat{F}| \Phi_m^p\right\rangle & =\left\langle\phi_m|\hat{f}| \phi_p\right\rangle \\
\left\langle\Phi|\hat{F}| \Phi_{m n}^{p q}\right\rangle & =0
\end{aligned}
$$
For a two-body operator (like the coulomb repulsion)
$$
\hat{G}=\frac{1}{2} \sum_{i=1}^N \sum_{\substack{j=1 \\ j \neq i}}^N \hat{g}(i, j)
$$
The Slater-Condon rules are:
$$
\begin{aligned}
\langle\Psi|\hat{G}| \Psi\rangle & =\frac{1}{2} \sum_{i=1}^N \sum_{\substack{j=1 \\
j \neq i}}^N\left(\left\langle\phi_i \phi_j|\hat{g}| \phi_i \phi_j\right\rangle-\left\langle\phi_i \phi_j|\hat{g}| \phi_j \phi_i\right\rangle\right), \\
\left\langle\Psi|\hat{G}| \Psi_m^p\right\rangle & =\sum_{i=1}^N\left(\left\langle\phi_m \phi_i|\hat{g}| \phi_p \phi_i\right\rangle-\left\langle\phi_m \phi_i|\hat{g}| \phi_i \phi_p\right\rangle\right), \\
\left\langle\Psi|\hat{G}| \Psi_{m n}^{p q}\right\rangle & =\left\langle\phi_m \phi_n|\hat{g}| \phi_p \phi_q\right\rangle-\left\langle\phi_m \phi_n|\hat{g}| \phi_q \phi_p\right\rangle.
\end{aligned}
$$
# Links
- [[Slater Determinant]]
-  [[Fermion]]

# References
- [Szabo, Attila; Ostlund, Neil S. (1996). "Ch. 2.3.3". Modern Quantum Chemistry : Introduction to Advanced Electronic Structure Theory.](https://books.google.nl/books/about/Modern_Quantum_Chemistry.html?id=6mV9gYzEkgIC&redir_esc=y)
- [Wikipedia](https://en.wikipedia.org/wiki/Slater%E2%80%93Condon_rules)