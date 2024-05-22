Grover’s search algorithms, including various Partial Grover Searches (PGS),
experience scaling problems for unknown multiple solutions as the number of
iterations rises with an increase in the number of solutions or marked states
making implementation more computationally expensive. Inspired by recent PGS
algorithms for multiple searchers, this article proposes a fast Grover quantum
search algorithm: Bi-directional Multi-solution Grover Search (BMGS), to tackle
an arbitrary number of solutions from an unstructured database. We introduced a
multi-segment bi-directional search tactic with PGS on multiple equal segments
of each state, starting from an initial state and multiple marked states in parallel.
We have shown in this article that for each solution our novel approach requires
at most √N(1 − d√(1/(b^(r/dk)) iterations over Partial Grover Search (PGS), which
take π/4√N*√(1 − 1/b) (here, N = 2r elements, b is the branching factor of PGS, 
d is the number of equal segments on r and k = ⌈log2 b⌉) and the number of arbitrary 
solutions is s). Our proposed BMGS algorithm is benchmarked against state-of-the-art 
DFGS, PGS, and standard GS implementations for an arbitrary number of solutions 
with 2 to 20 qubits. We also show our BMGS requires fewer iterations for large b and d 
and archives an O(s√N) average complexity. In this repository is our implementation
of BMGS.
