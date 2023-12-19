For an $n$-qubit quantum state $|\phi\rangle$, its stabilizer group is the subgroup $G$ of the $n$-qubit Pauli group such that $g\ket{\phi} = \ket{\phi}$ for all $g\in G$.  See also [[Stabilizer group]].

For stabilizer states, the stabilizer group:
- is maximal, i.e. one cannot add elements from the Pauli group such that the group still is a stabilizer group
- uniquely characterizes the state. That is, there is only a single quantum state $\ket{\phi}$  (modulo global factor) such that $g \ket{\phi} = \ket{\phi}$ for all elements $g$ of the stabilizer group.

For an $n$-qubit stabilizer state, its stabilizer group is of size $2^n$ but has merely $n$ generators, making a succinct representation possible.

Typically, the generators are not stored as Pauli strings but instead as a _tableau_, a collection of binary variables that represents Pauli strings.

# References
-  Scott Aaronson, Daniel Gottesman,; Improved simulation of stabilizer circuits; (2004); [10.1103/PhysRevA.70.052328](https://www.doi.org/10.1103/PhysRevA.70.052328);  @aaronson_improved_2004
-  Michael A. Nielsen, Isaac L. Chuang,; Quantum Computation and Quantum Information: 10th Anniversary Edition; (2010); [https://www.cambridge.org/core/books/quantum-computation-and-quantum-information/01E10196D0A682A6AEFFEA52D53BE9AE](https://www.cambridge.org/core/books/quantum-computation-and-quantum-information/01E10196D0A682A6AEFFEA52D53BE9AE);  @nielsen_quantum_2010