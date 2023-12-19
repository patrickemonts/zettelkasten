#stabilizer #simulation 

Stabilizer circuits are those composed only by the gates $H$, $S$, $CNOT$ and single-qubit measurements in the eigenbases of $X$, $Y$ or $Z$. Pauli gates can also be used and re-absorbed in the specified gates. Stabilizer circuits are efficiently simulatable in a classical computer, via [[Gottesman-Knill theorem]]. 

The key for simulation of stabilizer circuits is to keep track of the stabilizer group of the quantum state. For stabilizer circuits, the stabilizer group uniquely characterizes the quantum state (see [[Stabilizer states]]). 

An interesting result is that any stabilizer circuit can be expressed with at most $\mathcal O(n^2 \log n)$ gates. 
# Links
- [[Clifford group]]
- [[Gottesman-Knill theorem]]
- [[stabilizer states]]
# References
-  Scott Aaronson, Daniel Gottesman,; Improved simulation of stabilizer circuits; (2004); [10.1103/PhysRevA.70.052328](https://www.doi.org/10.1103/PhysRevA.70.052328);  @aaronson_improved_2004