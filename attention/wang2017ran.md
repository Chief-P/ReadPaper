# Residual Attention Network for Image Classification

Fei Wang et al., SenseTime. [CVPR, 2017]

## Background

Previous works focus on sequential process. No attention mechanism has been applied to feed-forward network. Recent feed-forward networks are very deep.

Soft attention.

## Structure

The output of Attention Modules $H$ is:

$H_{i,c}(x) = M_{i,c}(x) * T_{i,c}(x)$,

where $i$ ranges over all spatial positions and $c$ ranges over all channels.

### A. Mask Branch

$M(x,\theta)$

Bottom-up top-down structure.

Feature selector during forward inference & gradient update filter during back propagation, which makes the trunk branch robust to noisy labels.

### B. Trunk Branch

$T(x,\phi)$

## Methodology

### 1. Attention Residual Learning

$H_{i,c}(x) = (1 + M_{i,c}(x)) * F_{i,c}(x)$,

where $F(x)$ is the original features.

Compared to residual learning:

$H_{i,c}(x) = x + F_{i,c}(x)$,

where $F_{i,c}(x)$ approximates the residual function.

### 2.Soft Mask Branch

## TODO

Residual Learning