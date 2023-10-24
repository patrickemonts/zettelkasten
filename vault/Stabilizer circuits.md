#stabilizer #simulation 

Stabilizer circuits are those composed only by the gates $P$, $S$, $CNOT$. Pauli gates can also be used and re-absorbed in the specified gates. Stabilizer circuits are efficiently simulatable in a classical computer, via [[Gottesman-Knill theorem]]. 

The key for simulation of stabilizer circuits is to keep track of the _tableau_, a collection of binary variables that represents Pauli strings, updated accordingly to the rules specified by the circuit. 

An interesting result is that any stabilizer circuit can be expressed with at most $\mathcal O(n^2 \log n)$ gates. 
# Links
- [[Clifford group]]
- [[Gottesman-Knill theorem]]
# References
-  Scott Aaronson, Daniel Gottesman,; Improved simulation of stabilizer circuits; (2004); [10.1103/PhysRevA.70.052328](https://www.doi.org/10.1103/PhysRevA.70.052328);  @aaronson_improved_2004