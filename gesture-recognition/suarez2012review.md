# Hand Gesture Recognition with Depth Images: A Review

2012 IEEE RO-MAN: Jesus Suarez et al.

## Background

Problems: occlusions, lighting changes, rapid motion, or other skin-colored objects in a scene

## Pipeline & Methods

### 1. Depth Sensors

### 2. Hand Localization

Segmentation
* Depth Threshold/Skin-color Map
* Clustering/Region Growing

Tracking
* NITE
* Kalman filter
* CAMSHIFT/mean shift

### 3. Gesture Recognition

Static
* k-NN/NN/SVM
* Template Matching

Dynamic
* HMM
* FSM classifier (to codify hand motion)

## TODO
* Find SOTA in GR based on RGB
* Build input data