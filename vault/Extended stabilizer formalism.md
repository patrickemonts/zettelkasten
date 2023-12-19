Classical simulation method for simulating arbitrary quantum circuits on the usual input state $|0\rangle^ {\otimes n}$ . In the vanilla way, this is achieved by:
- writing the circuit to only consist of Clifford gates and T gates. Denote the number of T gates by $k$
- add $k$ ancillas, replace all T gates by some adaptive Clifford gates, and replace the input state by a $|0\rangle^{\otimes n} \otimes |T\rangle^{\otimes k}$ where $|T\rangle = (|0\rangle + e^{i\pi/4}|1\rangle)/\sqrt{2}$ is the magic state
- write the input state as linear combination of $m$ stabilizer states
- perform $O(m^2)$ simulations of the vanilla stabilizer formalism

$m$ is an exponential function of $k$. It is ongoing effort to reduce the base of the exponent. 

Various optimizations are possible.

[[Stabilizer states]]
# References
- Sergey Bravyi and David Gosset; Improved Classical Simulation of Quantum Circuits Dominated by Clifford Gates; (2016); https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.116.250501
-  Sergey Bravyi, Graeme Smith, and John A. Smolin; Trading Classical and Quantum Computational Resources; (2016); https://journals.aps.org/prx/abstract/10.1103/PhysRevX.6.021043
