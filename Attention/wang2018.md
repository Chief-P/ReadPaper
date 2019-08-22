# Non-local Neural Networks

Xiaolong Wang et al. [CVPR, 2018]

## Background

Currently, long-range dependencies can only be captured when convolutional or recurrent oprations are applied repeatedly.

Generalization of the classical non-local mean operation.

More accurate and economical than the 3D convolutional counterparts.

## Methodology

### Formulation

Non-local operation:

$y_i = \frac{1}{C(x)}\sum_{\forall j} f(x_i,x_j)g(x_j)$,

where the pairwise function $f$ computes a scalar between $i$ and all $j$, the unary function $g$ computes a representation of the input signal at the position j, and $C(x)$ is for normalization.

### Instantiations

Embedded Gaussain: $f(x_i,x_j)=e^{\theta(x_i)^T\phi(x_j)}$.

Dot product: $f(x_i,x_j)=\theta(x_i)^T\phi(x_j)$

### Non-local Block

$z_i = W_z y_i + x_i$,

where $W_z$ is initialized as zero to fit into pretrained model.

## Comment

The structure of the paper reminds me of ResNet (formulation, instantiation, and block), afterall it is supervised by Kaiming.