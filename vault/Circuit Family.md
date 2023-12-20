#math #computer-science 

A *circuit family* is a set $\mathcal{C}={C_n}$ of circuits, where $n$ is the number of input bits.
Each of the circuits has one output bit.
A circuit family *recognizes*/*decides* a [[Language]] $L\subseteq \{0,1\}^*=\cup_{n\leq 0}\{0,1\}^n$  if for every $n$ and every input $x\in \{0,1\}^n$, the circuit $C_n$ outputs 1 if $x\in L$ and 0 otherwise.

A circuit family is called *uniformly polynomial* if there exists a [[Deterministic Turing Machine]] that outputs *$C_n$* given $n$ as input, using space logarithmic in $n$. That means that the number of gates (size of the circuit) can grow at most polynomially with $n$.

Uniformly polynomial circuit families are equal in power to polynomial-time [[Deterministic Turing Machine|Deterministic Turing Machines]]: a language $L$ can be decided by a uniformly polynomial circuit family if and only if $L\in \textbf{P}$ , where $\textbf{P}$ is the [[Complexity Class]] of languages decidable by polynomial-time Turing machines.
# Links
- [[Boolean Circuit]]
- [[Logic Gates]]
- [[Deterministic Turing Machine]]
- [[Turing Machine]]
- [[Complexity Class -- P]]

# References
-  Ronald de Wolf,; Quantum Computing: Lecture Notes; (2023); [10.48550/arXiv.1907.09415](https://www.doi.org/10.48550/arXiv.1907.09415);  @de_wolf_quantum_2023 
- Proof for uniformly polynomial circuits <=> poly-time Det. Turing Machines
	-  Christos H. Papadimitriou,; Computational Complexity; (1994);  @papadimitriou_computational_1994, Theorem 11.5