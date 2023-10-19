#physics #many-body #method
Matrix product states are one-dimensional [[Tensor Networks]]. The states can be written as
$$\ket{\psi }=\sum_{\{i\}} \sum_{\{\alpha\}}A^{i_1}_{1,\alpha_1}A^{i_2}_{\alpha_1,\alpha_2}\cdots  A^{i_N}_{\alpha_{N-1},1}\ket{ i_1,\cdots,i_N }$$
Here, $A^i_{\alpha_1,\alpha_2}$ are $d\times D\times D$ tensors of rank 3 with a physical index $i$ and two virtual indices $\alpha_1$ and $\alpha_2$. The virtual indices are called virtual since they are only used for the construction of the state.
In analogy to the names of the indices, $d$ is called the physical bond dimension and $D$ is the virtual bond dimension.

Following the [[Graphical Notation Tensor Networks|graphical notation]] for tensor networks, the state can be written equivalently as
![[mps.svg]]
Due to their one-dimensional structure, they are numerically efficient to contract.

# Links
- [[Tensor Networks]]
- [[Graphical Notation Tensor Networks]]
- [[Projected Entangled Pair States (PEPS)]]
- [[Gauge Freedom of Tensor Networks]]
- [[Matrix Product Operators]]
- [[Construction of MPS]]
- [[Canonical Form]]
# References
- Review
	- J. Ignacio Cirac, David Pérez-García, Norbert Schuch, Frank Verstraete,; Matrix product states and projected entangled pair states: Concepts, symmetries, theorems; (2021); [10.1103/RevModPhys.93.045003](https://www.doi.org/10.1103/RevModPhys.93.045003);  @cirac_matrix_2021 
- Early papers
	- M. Fannes, B. Nachtergaele, R. F. Werner,; Finitely correlated states on quantum spin chains; (1992); [10.1007/BF02099178](https://www.doi.org/10.1007/BF02099178);  @fannes_finitely_1992 
- Introduction
	- Jacob C. Bridgeman, Christopher T. Chubb,; Hand-waving and Interpretive Dance: An Introductory Course on Tensor Networks; (2017); [10.1088/1751-8121/aa6dc3](https://www.doi.org/10.1088/1751-8121/aa6dc3);  @bridgeman_hand-waving_2017 
