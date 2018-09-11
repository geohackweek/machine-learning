---
title: "Land Classification with Supervised Machine Learning"
teaching: 25
exercises: 0
questions:
- "
How can I create a simple image pixel classifier using python?
"
objectives:
- "Gain insight into setting up a geospatial machine learning model, understand differences in imagery types,
create testing and training data for supervised modelling,
evalaute performance against multiple model types,
gain knowledge of streaming pixels from the cloud."
keypoints:
- "run a support vector machine simple model on aerial and satellite imagery streaming from the cloud."
---

# Perform Land Classification using Supervised Machine Learning

## Goal:

In this tutorial, you will work with nadir-looking imagery to run supervised machine learning models to perform land classification. From this exercise, you will:
* gain insight into setting up a geospatial machine learning model,
* understand differences in imagery types,
* create testing and training data for supervised modeling,
* evaluate performance against multiple model types,
* gain knowledge of streaming pixels from the cloud.

## Background

Land classification is the technique of labelling each individual pixel in an image with its relevant class (e.g. water, road, tree, etc). In remote sensing, there is a long history of this process, largely driven by manual labor. With the rise of increased acquisition from digital sensor platforms, at high resolution, manual classification is unscalable and can have inherent human biases. Machine learning is ideal for land classification in its ability to scale the pixel-wise labelling exponentially. A Support Vector Machine implementation is very straightforward, and is discussed here. However, for large-scale processing workflows, Convolutional Neural Networks (CNN) have become ideal.

![alt-text](../assets/img/lc.png "Logo Title Text 1")

<i> Figure 1. RGB overhead imagery (left) is used in combination with truth data to perform a pixel-size land classification (far right), where each pixel is translated from an RGB value to a label class. In this case, the classes are pool (cyan), impervious surface (grey), tree/shrub (dark green), irrigated lawn (light green), shadows (dark grey), natural/non-irrirgated lawn (brown). This land classification map was produced using a deep learning Convolutional Neural Network. </i>

For this tutorial, you will be using [this jupyter notebook](../code/demo_landclassification.ipynb).
