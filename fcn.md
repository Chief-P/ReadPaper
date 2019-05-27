# Fully Convolutional Networks for Semantic Segmentation 

CVPR2015, Long et al.

## Background

The trend of recognition is from whole-image classification to pixelwise prediction (growth of precesion).

1. Patchwise training is common, but lacks the **efficiency** of fully convolutional training.
Pre- and post-processing are used in former methods.

1. Inherent tension between semantics and location: **what** (global) and **where** (local). Deep feature hierarchies encode location and semantics in a nonlinear local-to-global pyramid.

## Related Work

Success of deep nets for image classification and transfer learning.

1. Fully convolutional networks (Matan et al. [26])

1. Dense prediction with convnets

## Solution

Transform fully connected layers into convolution layers.

Upsampling: transposed convolution.

Optimization: SGD with momentum.

Code: http://fcn.berkeleyvision.org

Fine-tuning

## Result

Datasets: PASCAL VOC 2011-2, NYUDv2, and SIFT Flow

## TODO
* AlexNet, VGG nets, and GoogLeNet
* Learn some applications of FCN.
* Learn more about transfer learning [3, 38] and fine-tuning [3].