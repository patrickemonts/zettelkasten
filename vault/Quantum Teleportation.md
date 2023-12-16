#quantum #quantum-information

Quantum teleportation is a quantum protocol to transfer a quantum state from one party to another one.
This protocol does *not* act instantaneously (otherwise it would conflict with relativity) and it does *not* copy the state, but transfer it (otherwise it would be in contradiction to the [[No Cloning Theorem]]).

The protocol of quantum teleportation acts between to parties, Alice and Bob.
In total, the protocol involves three qubits, two qubits $\ket{A_1}$, $\ket{A_2}$ on Alice's side an one qubit $\ket{B}$ on Bob's side. Additionally, Alice and Bob have a classical communication channel connecting them.

The aim is to teleport Alice's first qubit $\ket{A_1}=\alpha_0\ket{0}+\alpha_1\ket{1}$ to Bobs qubit $\ket{B}$.
Without further resources this would be impossible, because the amplitudes $\alpha_0,\alpha_1$ may require an infinite number of bits of precision to write them down exactly.
However, suppose Alice's second qubit $\ket{A_2}$ and Bob's qubit $\ket{B}$ are in an entangled state
$$
\ket{\phi}=\frac{1}{\sqrt{2}}(\ket{0_A0_B}+\ket{1_A1_B})
$$ 
with Bob . 
Initially, the full state of the system is
$$
\ket{A_1}\otimes\ket{\phi}=(\alpha_0\ket{0}+\alpha_1\ket{1})\otimes\frac{1}{\sqrt{2}}(\ket{00}+\ket{11}).
$$
Alice performs a CNOT on her two qubits and then a Hadamard transform
on her first qubit. Now, the joint three-qubit state can be written as
$$
\begin{array}{l}
\frac{1}{2} \ \ket{00}(\alpha_0\ket{0}+\alpha_1\ket{1}) \ +\\
\frac{1}{2} \ \ket{01}(\alpha_0\ket{1}+\alpha_1\ket{0}) \ +\\
\frac{1}{2} \ \ket{10}(\alpha_0\ket{0}-\alpha_1\ket{1}) \ +\\
\frac{1}{2}\underbrace{\ket{11}}_{Alice}\underbrace{(\alpha_0\ket{1}-\alpha_1\ket{0})}_{Bob}.
\end{array}
$$
Alice now measures her two qubits in the computational basis 
and sends the result in the form of 2 random classical bits $ab$ to Bob over the classical channel. 

Depending on the bits $ab$, Bob  knows which transformation he must perform qubit in order to regain Alice's original quantum state $\alpha_0\ket{0}+\alpha_1\ket{1}$.
First, if $b=1$ then he applies a bitflip ($X$-gate) on his qubit; second if $a=1$ then he applies a phaseflip ($Z$-gate). For instance, if Alice sent $ab=11$, then Bob knows that his qubit is in the state $\alpha_0\ket{1}-\alpha_1\ket{0}$. 
An $X$ gate followed by a $Z$ gate will give him Alice's original quantum state $\alpha_0\ket{0}+\alpha_1\ket{1}$.  
In fact, if Alice's qubit had been *entangled* with some other qubits,
then teleportation preserves this entanglement: Bob then receives
a qubit that is entangled in the same way as Alice's original qubit was.

Note that the qubit on Alice's side has been destroyed: teleporting moves a qubit from Alice to Bob, rather than copying it. Copying an unknown quantum is impossible according to the [[No Cloning Theorem]].

# Links
- [[Entanglement]]
- [[No Cloning Theorem]]

# References
-  Charles H. Bennett, Gilles Brassard, Claude Crépeau, Richard Jozsa, Asher Peres, William K. Wootters,; Teleporting an unknown quantum state via dual classical and Einstein-Podolsky-Rosen channels; (1993); [10.1103/PhysRevLett.70.1895](https://www.doi.org/10.1103/PhysRevLet.70.1895);  @bennett_teleporting_1993 
-  Ronald de Wolf,; Quantum Computing: Lecture Notes; (2023); [10.48550/arXiv.1907.09415](https://www.doi.org/10.48550/arXiv.1907.09415);  @de_wolf_quantum_2023 

