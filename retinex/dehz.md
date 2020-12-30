# Fast Efficient Algorithm for Enhancement of Low Lighting Video

Xuan Dong et al. [ICME, 2011]

## Enhancement

Hazy image model (with the LIME notation):

$1-L = (1-R) \circ \tilde{T} + a(1-\tilde{T})$.

When the atmosphere is homogeneous,

$\tilde{T}(x)=e^{-\beta d(x)}$,

where d is the depth of the object.

Estimation:

$\tilde{T}(x)=1-\omega \min_{c \in {r, g, b}}{\min_{y \in \Omega(x)}\frac{(1-L)^c(y)}{a^c}}$

## Acceleration

### Motion Estimation



### Fast SAD Algorithm



## Remark

Intuitive! Maybe the authors observed the inverted images and found they look hazy.