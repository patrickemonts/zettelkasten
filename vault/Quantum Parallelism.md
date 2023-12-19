#quantum-information #quantum 

One uniquely quantum-mechanical effect that we can use for building quantum algorithms is *quantum parallelism*.

Suppose we have a classical algorithm that computes some function $f:\{0,1\}^n\rightarrow\{0,1\}^m$. Then we can build a quantum circuit $U$ (consisting only of Toffoli gates) that maps $\ket{z}\ket{0}\rightarrow\ket{z}\ket{f(z)}$ for every $z\in\{0,1\}^n$.
Using $n$ [[Quantum Gates#^efb8de|Hadamard]] gates, we can generate a superposition of all inputs $z$. If we apply $U$ to this superposition, we obtain
$$
U\left(\frac{1}{\sqrt{2^n}}\sum_{z\in\01^n}\ket{z}\ket{0}\right)=
\frac{1}{\sqrt{2^n}}\sum_{z\in\01^n}\ket{z}\ket{f(z)}.
$$
One application of $U$ yields the final superposition that contains $f(z)$ for *all* $2^n$ input values $z$!  
However, by itself this is not very useful and does not give more than classical randomization, since observing the final superposition will give just one uniformly random $\ket{z}\ket{f(z)}$ and all other information will be lost.

The idea of *quantum parallelism* needs to be combined with 
the effects of interference and [[Entanglement]] in order to get something 
that is better than classical.

# Links
- [[Quantum Circuit]]

# References
-  Ronald de Wolf,; Quantum Computing: Lecture Notes; (2023); [10.48550/arXiv.1907.09415](https://www.doi.org/10.48550/arXiv.1907.09415);  @de_wolf_quantum_2023 
