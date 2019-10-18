# Spatial Transformer Networks

Jaderberg et al., Google DeepMind, 2016

## Background

Spatially invariant CNN

## Methodology

### 1. Localisation Network

$\theta=f_{loc}(U)$, where $\theta$ is the parameters of the transformation, $U$ is the input feature map, and $f_{loc}()$ can take any form of networks.

### 2. Parameterised Sampling Grid

Transformation $T_\theta(G)$, where G is the sampling grid.

### 3. Differentiable Image Sampling

$V_i^c = \sum_n^H \sum_m^WU_{nm}^c k(x_i^s-m;\Phi_x) k(y_i^s-n;\Phi_y)$,

where $k()$ defines the image interpolation with parameters $\Phi_x$, $\Phi_y$.

Define the gradients with respect to $U$ and $G$ to allow backpropagation.

## Limitation

Parallel spatial transformers limits the number of objects that the network can model.