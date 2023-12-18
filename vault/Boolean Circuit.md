#computer-science #math

A *Boolean circuit* is a finite [[Directed Acyclic Graph]] with [[Logic Gates]] AND, OR, and NOT.
It has $n$ input nodes, which contain the $n$ input bits ($n\geq 0$). The internal nodes are AND, OR, and NOT gates, and there are one or more designated output nodes.  
The initial input bits are fed into AND, OR, and NOT gates according to the circuit, and eventually the output nodes assume some value.

A circuit *computes* some Boolean function $$f: \{0,1\}^n\rightarrow\{0,1\}^m$$ if the output nodes get the right value $f(x)$ for every input $x\in\{0,1\}^n$.

# Links
- [[Quantum Computing Gates]]
- [[Logic Gates]]
- [[Directed Acyclic Graph]]

# References
-  Ronald de Wolf,; Quantum Computing: Lecture Notes; (2023); [10.48550/arXiv.1907.09415](https://www.doi.org/10.48550/arXiv.1907.09415);  @de_wolf_quantum_2023 
