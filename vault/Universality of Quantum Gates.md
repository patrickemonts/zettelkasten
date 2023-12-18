#physics #computer-science 

A *universal set* of gates means that any other unitary transformation can be built from these gates. 

There are several choices:
1.  The set of all 1-qubit operations together with the 2-qubit $CNOT$ gate is universal.

Since there are infinitely many 1-qubit gates, this statement is not very useful in practice. A finite set would be more useful.

2. The set consisting of $CNOT$, Hadamard, and the phase-gate $T=R_{\pi/4}$ is universal in the sense of approximation.
   Any other unitary can be arbitrarily well approximated using circuits of only these gates.

The [[Solovay-Kitaev theorem]] states that this approximation is quite efficient:
Any 1- or 2-qubit gate can be approximated up to error $\epsilon$ using a number of gates (from our small set) that is only $\mathrm{polylog}(1/\epsilon)$. in particular, simulating arbitrary gates up to exponentially small error costs only a polynomial overhead.

It is possible to restrict to gates with real numbers and an even smaller set

3. The set of Hadamard and Toffoli (CCNOT) is universal for all unitaries with real entries in the sense of approximation, meaning that any unitary with only real entries can be arbitrarily well approximated using circuits of only these gates.

# Links
- [[Quantum Gates]]
- [[Quantum Circuit]]

# References
- Solovay-Kitaev Theorem
	-  C.M. Dawson, M.A. Nielsen,; The Solovay-Kitaev algorithm; (2006); [10.26421/QIC6.1-6](https://www.doi.org/10.26421/QIC6.1-6);  @dawson_solovay-kitaev_2006 
	- A. Yu Kitaev,; Quantum computations: algorithms and error correction; (1997); [10.1070/RM1997v052n06ABEH002155](https://www.doi.org/10.1070/RM1997v052n06ABEH002155);  @kitaev_quantum_1997 
	-  Michael A Nielsen, Isaac L Chuang,; Quantum computation and quantum information (cambridge series on information and the natural sciences); (2004);  @nielsen_quantum_2004, Appendix 3
-  Ronald de Wolf,; Quantum Computing: Lecture Notes; (2023); [10.48550/arXiv.1907.09415](https://www.doi.org/10.48550/arXiv.1907.09415);  @de_wolf_quantum_2023 
