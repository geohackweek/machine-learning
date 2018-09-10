---
title: "Land Classification with Supervised Machine Learning"
teaching: 0
exercises: 11
questions: 10
- "
1. What type of information can you discern from the streaming cloud imagery?
2. One image is satellite imagery and one is aerial imagery. Can you tell which is which? Why? What other observations can you make about these images?
3. Why are there two different training data sets?
4. What do you notice about the training and image data shapes? Do they make sense?
5. What about the distribution of class types? 
6. What could the distribution of the training data indicate? What changes could be useful?
7. What are some of the major problems with the predicted result? How could we improve them?
8. How can we define accuracy? Precision? What is recall?
9. What kind of differences do you expect between the aerial and satellite image predictions?
"
objectives:
- "Gain insight into setting up a geospatial machine learning model, understand differences in imagery types,
create testing and training data for supervised modelling,
evalaute performance against multiple model types,
gain knowledge of streaming pixels from the cloud."
keypoints:
- "run a support vector machine simple model on aerial and satellite imagery streaming frmo the cloud."
---

# Perform Land Classification using Supervised Machine Learning

## Goal:

In this tutorial, you will work with nadir-looking imagery to run supervised machine learning models to perform land classification. From this excersize, you will:
* gain insight into setting up a geospatial machine learning model,
* understand differences in imagery types,
* create testing and training data for supervised modelling,
* evalaute performance against multiple model types,
* gain knowledge of streaming pixels from the cloud.

## Background

Land classification is the technique of labelling each individual pixel in an image with its relevant class (e.g. water, road, tree, etc). In remote sensing, there is a long history of this process, largely driven by manual labor. With the rise of increased acquisition from digital sensor platforms, at high resolution, manual classification is unscalabile and can have inherent human biases. Machine learning is ideal for land classification in its ability to scale the pixel-wise labelling exponentially. A Support Vector Machine implementation is very straightfoward, and is discusssed here. However, for large-scale processing workflows, Convolutional Neural Networks (CNN) have become ideal.

![alt-text](../assets/img/lc.png "Logo Title Text 1")

<i> Figure 1. RGB overhead imagery (left) is used in combination with truth data to perform a pixel-size land classification (far right), where each pixel is translated from an RGB value to a label class. In this case, the classes are pool (cyan), impervious surface (grey), tree/shrub (dark green), irrigated lawn (light green), shadows (dark grey), natural/non-irrirgated lawn (brown). This land classification map was produced using a deep learning Convolutional Neural Network. </i>

For this tutorial, you will be using [this jupyter notebook](../code/demo_landclassification.ipynb).

