# LIME: Low-light Image Enhancement via Illumination Map Estimation

Xiaojie Guo et al. [Image Processing, 2017]

## Related

DeHz, Retinex

## Methodology

Retinex explains the formation of a low-light image:

$L = R \circ T$, 

where $T$ represents illumination map.

Optimization problem:

$\min_{T}{{\lVert \hat{T} - T \rVert}_{F}^{2} + \alpha \lVert W \circ \nabla T \rVert_{1}}$,

to preserve the overall structure and to smooth the textural details simultaneously.

Solved with ALM.

## TODO

Read Retinex and DeHz