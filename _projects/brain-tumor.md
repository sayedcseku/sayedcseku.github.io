---
title: "Brain Tumour auto-segmentation from 3D MRI images using 3D U-Net"
excerpt: "Building a neural auto-segmentation model for MRI images with UNets with Dice Loss function. In this project, I build a multi-class segmentation model. We'll identify 3 different abnormalities in each image: edemas, non-enhancing tumors, and enhancing tumors. This project is to be continued. <br/>"
collection: portfolio
---


<img src='/images/u-net-architecture.png'>

# Standard data preparation techniques for MRI datasets

While our dataset is provided to us post-registration and in the NIfTI format, we still have to do some minor pre-processing before feeding the data to our model.

# Metrics and loss functions for segmentation

- Dice Similarity Coefficient

Aside from the architecture, one of the most important elements of any deep learning method is the choice of our loss function.

A natural choice that you may be familiar with is the cross-entropy loss function.

However, this loss function is not ideal for segmentation tasks due to heavy class imbalance (there are typically not many positive regions).
A much more common loss for segmentation tasks is the Dice similarity coefficient, which is a measure of how well two contours overlap.

The Dice index ranges from 0 (complete mismatch)
To 1 (perfect match).

# Visualizing and evaluating segmentation models
