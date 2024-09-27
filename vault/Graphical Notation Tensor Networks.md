#tensornetworks

The graphical notation in tensor networks is a way to represent (possibly high-dimensional) tensors and their contractions.
A tensor of rank $d$ is given by a bubble and $d$ legs. Connected legs are contracted (i.e. matrix multiplication along that axis)

# Example
- Vector: A vector $\vec{v}$ has one index that is needed to address an element. Thus, one leg (in black) ![[mpsnotation_vector.excalidraw|200]]
- Matrix: A matrix $A$ needs two indices $A_{i,j}$ to address an element. Thus, two legs![[mpsnotation_matrix.excalidraw|200]]
- Tensor (rank 3): As an example, we use the 3-leg tensor $T_{i,j,k}$. One leg is marked in orange which is reminiscent to the convention used for [[Matrix Product States (MPS)|MPS]] here![[mpsnotation_tensor.exaclidraw|200]]
- Matrix-Matrix product: Not only the objects themselves, but also arithmetic operations between different tensors can be expressed with the graphical notation. Here, the middle indes $k$ is contracted, i.e. the matrix multiplication over this index is execute. ![[mpsnotation_matrix_matrix_product.excalidraw]]
# Links
- [[Matrix Product States (MPS)]]
- [[Projected Entangled Pair States (PEPS)]]
- [[Tensor Networks]]
- [[Variational Methods]]

# References
-  Román Orús,; A practical introduction to tensor networks: Matrix product states and projected entangled pair states; (2014); [10.1016/j.aop.2014.06.013](https://www.doi.org/10.1016/j.aop.2014.06.013);  @orus_practical_2014 
-  Jacob C. Bridgeman, Christopher T. Chubb,; Hand-waving and Interpretive Dance: An Introductory Course on Tensor Networks; (2017); [10.1088/1751-8121/aa6dc3](https://www.doi.org/10.1088/1751-8121/aa6dc3);  @bridgeman_hand-waving_2017 
