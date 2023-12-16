
#quantum #quantum-information

If we only care about the final probability distribution of the $m$ outcomes, 
not about the resulting post-measurement state, then the most general type of measurement we can use a positive-operator-valued measure(POVM).  

A Positive Operator Valued Measure is a generalization of [[Projective Measurements]].
It  is described by a set of matrices  $m$ positive semidefinite matrices $E=(E_i)_{i=1}^m$ where all operators sum to identity  $\sum_{i=1}^m E_i = \mathbb{1}$. 

When measuring a state $\ket{\phi}$, the probability of outcome $i$ is given by $\mathrm{Tr}(E_i\ketbra{\phi}{\phi})$.
A projective measurement is the special case of a POVM where the measurement elements $E_i$ are projectors.
In the special case of a projective measurement, $E_i$ is a projector, then $\mathrm{Tr}(E_i\ketbra{\phi}{\phi})=\mathrm{Tr}(E_i^2\ketbra{\phi}{\phi})=\mathrm{Tr}(E_i\ketbra{\phi}{\phi}E_i)=||E_i\ket{\phi}||^2$, using the fact that $E_i=E_i^2$ and the cyclic property of the trace.

Even though POVMs strictly generalize projective measurements, one can show that every POVM can be "simulated'' by a projective measurement on a slightly larger space that yields the exact same probability distribution over measurement outcomes (this follows from [[Neumark's Theorem|Neumark's theorem]])

## Example
For example, suppose you have a state in a 2-dimensional space, and you know it is either in state $\ket{0}$ or in state $\ket{+}=\frac{1}{\sqrt{2}}(\ket{0}+\ket{1})$. 
Since the two states are not orthogonal , there is no measurement that distinguishes them perfectly. However, we can construct a POVM measurement that never makes a mistake, but sometimes gives another outcome 2, meaning "I don't know.'' 
In total the measurement has two outcomes:

-  If the state is $\ket{0}$, then you get correct outcome 0 with probability 1/4, and outcome 2 with probability 3/4, but never get incorrect outcome 1.
-  If the state is $\ket{+}$, then you get correct outcome 1 with probability 1/4, and outcome 2 with probability 3/4, but never get incorrect outcome 0.

There is no projective measurement to achieve this, but a 3-outcome POVM with the following operators $E_i$ does the job:

- $E_0=\frac{1}{2}\ketbra{-}{-}$ (where $\ket{-}=\frac{1}{\sqrt{2}}(\ket{0}-\ket{1})$, which is orthogonal to the $\ket{+}$ state)
- $E_1=\frac{1}{2}\ketbra{1}{1}$ (note that this is orthogonal to the $\ket{0}$ state)
- $E_2=I-E_0-E_1.$

You can check that $E_0,E_1,E_2$ are positive semi-definite matrices and add up to identity, so they form a valid POVM. None of the 3 matrices is a projector.
# Links
- [[Projective Measurements]]

# References
-  Michael A Nielsen, Isaac L Chuang,; Quantum computation and quantum information (cambridge series on information and the natural sciences); (2004);  @nielsen_quantum_2004 
-  Ronald de Wolf,; Quantum Computing: Lecture Notes; (2023); [10.48550/arXiv.1907.09415](https://www.doi.org/10.48550/arXiv.1907.09415);  @de_wolf_quantum_2023 

