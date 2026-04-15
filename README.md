# CUSTOM-DEEP-LEARNING-ON-FISH
This is a project built to build a custom Convolutional Neural Network for multiclass 


This notebook implements a 31-class fish image classification experiment using 8,829 images split 80/20 into training and validation sets. Two approaches were compared: a custom CNN and a transfer-learning model based on VGG16. The workflow includes basic data augmentation, normalisation, caching, shuffling, and early stopping callbacks to reduce overfitting.
Scientifically, the custom CNN showed weak generalisation: training accuracy rose to about 41%, but validation accuracy remained low and unstable, with final validation performance around 56.6% accuracy. In contrast, the VGG16 model performed much better. After freezing the backbone and then fine-tuning the last layers with a low learning rate, validation accuracy reached about 88.1%, with a final evaluation near 87.9% accuracy and substantially lower loss.

The low dataset clearly impacted the accuracy of the custom model. 
