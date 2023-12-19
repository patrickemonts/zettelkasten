#Pauli #stabilizer

The Clifford group is the set of operations that stabilizes the Pauli group for $n$ qubits $\mathcal P_n$.  As usual for gates, we say that two Cliffords are equivalent if they are the same up to a global phase (complex number of modulus one). In math, we write
$$
\mathcal C_n = \{g \in \mathcal{SU}(2^n) : g\ \mathcal P_n\ g^\dagger = \mathcal P_n\} / U(1)
$$
where
$$ U(1) = \{e^{i\cdot \phi} \mid \phi \in [0, 2\pi)\}$$ is the group of all phases.

The Clifford group on any number of qubits is generated with the gates $\{H, S, {\rm CNOT}\}$

Clifford representation of quantum states is related to efficient simulation of some particular states, see [[Gottesman-Knill theorem]]

# Links
- [[Stabilizer states]]
- [[Gottesman-Knill theorem]]

# References
-  Michael A. Nielsen, Isaac L. Chuang,; Quantum Computation and Quantum Information: 10th Anniversary Edition; (2010); [https://www.cambridge.org/core/books/quantum-computation-and-quantum-information/01E10196D0A682A6AEFFEA52D53BE9AE](https://www.cambridge.org/core/books/quantum-computation-and-quantum-information/01E10196D0A682A6AEFFEA52D53BE9AE);  @nielsen_quantum_2010
- Maris Ozols; Clifford group; (2008); http://home.lu.lv/~sd20008/papers/essays/Clifford%20group%20[paper].pdf