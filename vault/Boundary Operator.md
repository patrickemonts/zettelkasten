#math #homology
Given a p-simplex $σ(p) = [x0 · · · xp]$, the action of the boundary operator is, by definition,
$$\partial_p[x_0\dots x_p] = \sum_{i=1}^p(-1)^i[x_0\dots \hat{x}_i\dots x_p]$$
The boundary operator returns a sum of $p-1$ simplices (with alternating sign). Note that the boundary of a boundary is 0
$$\partial_{p-1}\partial_p \sigma{p}=0.$$
By linearity, the boundary operator can be extended to act on [[Chain Groups| chain groups]] as $\partial_p\colon C_p(K) \rightarrow C_{p-1}(K)$, where $K$ is a simplicial complex and $C_p(K)$ is the chain group with $p$-simplices defined on $K$.
Given the boundary opeator, multiple [[Chain Groups|chain group]]  from a [[Chain Complex| chain complex]].
The co-boundary operator is defined as $$\partial^\dagger_p\colon C_p \rightarrow C_{p+1}.$$
# Links
- [[SUSY and Cohomology]]
- [[Homology]]
- [[Reduced Homology]]
# References
- Crichigno, M. & Kohler, T. Clique Homology is QMA1-hard. Preprint at https://doi.org/10.48550/arXiv.2209.11793 (2022).