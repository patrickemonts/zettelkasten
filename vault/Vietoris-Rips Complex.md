#math #homology #todo #refs-needed 

> [!definition]
> Let $X$ be a collection of points in $\mathbb{R}^n$. The Vietoris-Rips complex of $X$ and $\epsilon$ is 
> $$ \mathcal{R}_\epsilon(X) = {S \subset X : B_\epsilon(x_i) \cap B_\epsilon(x_j) \neq \emptyset \forall x_i, x_j \in S}$$

To compute a Vietoris-Rips complex, we only need to compute $\mathcal{O}(n^2)$ distances, where $n$ is the number of data points. That is considerably quicker than computing a [[Cech Complex]].

However, Vietoris-Rips complex is not equivalent to a [[Cech Complex]] and only for a [[Cech Complex]], the [[Nerve Theorem]] holds. Thus, we cannot expect that the [[Betti Numbers | Betti numbers]] of the two complexes are equivalent.
If we are interested in the persistence and not in the exact Betti number of a given filtration, the following proposition helps

> [!proposition]
> For any $\epsilon > 0$, there is a chain of inclusion maps 
> $$R_\epsilon \hookrightarrow C_{\epsilon\sqrt{2}} \hookrightarrow R_{\epsilon\sqrt{2}}, $$
> where the simplicial complex is left implicit in the notation.

TODO: Write some comment about this
# Links
- [[Cech Complex]]
- [[Nerve Theorem]]
- 

# References
- TODO