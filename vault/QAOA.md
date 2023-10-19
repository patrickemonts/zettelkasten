#quantum-information #method

Double acronym: quantum approximate optimization ansatz, or quantum alternating operator ansatz. 

## Quantum Approximate Optimization Ansatz
The first indicates an ansatz derived by the discretization (through Trotter-Suzuki expansion) of the adiabatic state preparation algorithm. 
To mitigate the error due to trotter expansion and non-adiabaticity, the evolution time within each trotter step is turned into a variational parameter. 
Key property: this ansatz is problem-dependent, as the description of the problem Hamiltonian is used in the definition of the ansatz.

## Quantum Alternating Operator Approach
The second acronym indicates a variational algorithm which uses this ansatz, typically applied to solving classical optimization problems (classical Ising, MAXCUT).
# Links
- [[Variational Quantum Eigensolver (VQE)]]

# References
-  Edward Farhi, Jeffrey Goldstone, Sam Gutmann,; A Quantum Approximate Optimization Algorithm; (2014); [10.48550/arXiv.1411.4028](https://www.doi.org/10.48550/arXiv.1411.4028);  @farhi_quantum_2014

