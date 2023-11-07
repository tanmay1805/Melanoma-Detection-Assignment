# Melanoma Detection Assignment
In this assignment, we build a multiclass classification model using a custom convolutional neural network in TensorFlow.

***Problem statement***: To build a CNN based model which can accurately detect melanoma.

## General Information
Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths.
A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

* Actinic keratosis
* Basal cell carcinoma
* Dermatofibroma
* Melanoma
* Nevus
* Pigmented benign keratosis
* Seborrheic keratosis
* Squamous cell carcinoma
* Vascular lesion

## Conclusions
- Basic model of custom CNN shows ***training accuracy of 89%*** and ***validation accuracy of 51%***. This is clearly evident that the model is Overfitting.
- After we use a dropout layer, the model of custom CNN shows ***training accuracy of 48%*** and ***validation accuracy of 46%***. Although training and validation accuracy came closer, model accuracy overall has dropped significantly.
- After class rebalancing and augmentation ***Model accuracy is ~95% in training*** and ***~77% in validation dataset***. *Overfitting is addressed and rebalancing helped*. Model accuracy is well within acceptance range.

## Technologies Used
- tensorflow - version 2.14.0
- keras - version 2.14.0