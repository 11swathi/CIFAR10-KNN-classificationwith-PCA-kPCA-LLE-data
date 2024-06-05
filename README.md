# CIFAR10-KNN-classificationwith-PCA-kPCA-LLE-data

## Objective:
This project investigates how different ways of representing data affect image classification on 
the CIFAR-10 dataset. We will compare four methods: using the raw images directly, Principal 
Component Analysis (PCA), kernel PCA (kPCA), Locally Linear Embedding (LLE). For each 
representation, I will train a K-Nearest Neighbors (KNN) classifier and measure its performance 
in terms of classification accuracy and computational efficiency (training time). The main goal is 
to understand how these representation methods influence the KNN classifier's ability to 
accurately classify images, while also considering the computational cost.



## Dataset Description:
The CIFAR-10 dataset consists of 60,000 32x32 color images in 10 classes, with 6000 images 
per class. The originally provided dataset included a separate training set with 50,000 images and 
test set with 10,000 images. Interestingly, the training set was further divided into five batches of 
10,000 images each and the test batch contains exactly 1000 randomly-selected images from 
each class. To improve the training process, I combined all the batches into a single dataset of 
60,000 images. I normalized and reshaped the data after combining it, so dimension of the data is 
now 3072 (32x32x3). This larger dataset was then split into training, validation, and test sets for 
the classification task. 



- Name: CIFAR-10 (Canadian Institute for Advanced Research)
- Dataset Link: [https://www.cs.toronto.edu/~kriz/cifar.html]
- Size: 60,000 images (50,000 training + 10,000 testing)
- Image format: 32x32 pixels, RGB color
- Number of classes: 10 (6000 images per class)
- Class Labels: The CIFAR-10 dataset consists of images belonging to 10 mutually exclusive 
classes, representing everyday objects.
