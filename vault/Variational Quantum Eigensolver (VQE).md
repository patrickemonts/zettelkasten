#physics #quantum-information #method #todo #refs-needed 

The Variational Quantum Eigensolver is a generic variational method to find an approximation to the ground state of a Hamiltonian $H$. The elements of a VQE are
- Hamiltonian $H$
- Parameterizable Ansatz $U(\theta)$
- Optimization process

The goal is to obtain the set of parameters $\theta^*$ minimizing the energy of the Hamiltonian with respect to the parameterized state $U(\theta)\ket{\psi_0}$, where $\ket{\psi_0}$ is the initial state. 
$$
\theta^* = \operatorname{argmin}_\theta \bra{\psi_0}U^\dagger(\theta) H U(\theta)\ket{\psi_0}
$$

Due to the variational principle, we know
$$\operatorname{min}_\theta \bra{\psi_0}U^\dagger(\theta) H U(\theta)\ket{\psi_0} \geq \operatorname{min}_{\ket\psi} \bra{\psi} H \ket{\psi},$$
and thus we can only obtain an approximation to the ground state.

The optimizer is a classical method allowing to find good instances of $\theta^*$.

# Links
- [[Barren Plateaus]]
- 

# References
-  Alberto Peruzzo, Jarrod McClean, Peter Shadbolt, Man-Hong Yung, Xiao-Qi Zhou, Peter J. Love, Alán Aspuru-Guzik, Jeremy L. O’Brien,; A variational eigenvalue solver on a photonic quantum processor; (2014); [10.1038/ncomms5213](https://www.doi.org/10.1038/ncomms5213);  @peruzzo_variational_2014