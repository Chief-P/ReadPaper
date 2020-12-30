# Moving Object Detection on RGB-D Videos Using Graph Regularized Spatiotemporal RPCA

Javed et al. [ICIAP, 2017]

## Background

RPCA methods work under batch processing.

Spatial information is lost when restructuring.

## Methodology

Model reformulation:

$\min_{B,F}\|B\|^2_{max} + \lambda \|F\|_1 + \gamma_1 tr(B^T\Phi_sB) + \gamma_2 tr(B^T\Phi_tB) \;s.t.\; D=B+F$,

where $\Phi_t \in \R^{c\times c}$ and $\Phi_s \in \R^{p\times p}$ are Laplacian matrix of the temporal graph and spatial graph.
The last two terms are for spatialtemporal graph regularization of background model.

### 1. Removing motionless frames

Compute the dense optical flow between two consecutive frames. Derive $D \in \R^{p\times c}.$

### 2. Spatiotemporal graph Laplacians

Temporal graph is built built using s-NN strategy:

$G_t=(V_t, E_t, A_t)$,

where $V_t$ is the columns of matrix $D$, $A_t(i,j) = \exp(-\frac{\Delta_{i,j}-\Delta_{min}}{\sigma^2})$.

$\Phi_t = I - W^{-1/2}AW^{-1/2}$,

where $W = diag(\sum_j A_t(i,j))$.

### 3. Solution for Objective Function

Approximation.

## References

Detailed: Spatiotemporal Low-Rank Modeling for Complex Scene Background Initialization