# Deep Residual Learning for Image Recognition

Kaiming He et al., MSR. [CVPR, 2016]

## Background

*Vanishing/exploding gradients* has been largely addressed
by normalized initialization and intermediate normalization layers.

*Degradation* of training accuracy on deeper networks:
a stacked model is not even better than a solution by construction.

## Methodology

$H(x)=F(x)+x$

A building block is defined as:

$y = F(x, \{W_i\}) + W_s x$,

where the function $F(x, \{W_i\})$ represents the residual
mapping to be learned, and $W_s$ is a linear projection to
match dimensions.

If the function $F$ has only a single layer, the block is reduced to a linear layer.

## Comment

Analogous to Taylor expansion and remainder.