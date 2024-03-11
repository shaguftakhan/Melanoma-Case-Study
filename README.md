# Project Name
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)



## General Information
- What is the background of your project?
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

- What is the business problem that your project is trying to solve?
A model needs to be built to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

- What is the dataset that is being used?
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

    Actinic keratosis
    Basal cell carcinoma
    Dermatofibroma
    Melanoma
    Nevus
    Pigmented benign keratosis
    Seborrheic keratosis
    Squamous cell carcinoma
    Vascular lesion


## Conclusions
- Findings:
- In the first iteration, the model is found to be slightly overfitting. The training accuracy is in 60s, while the validation accuracy is stuck in 50. If the training would continue the model will overfit even more.

- Utilising Tensorflow's inbuild layer for performing data augmentation. This layer can be included as part of the model, and runs on only training data

- So, in the next iteration, the model's overfitting has decreased considerably, and now the validation accuracy is seen to be following the training accuracy closely. The validation accuracy and validation loss, though exhibit significant fluctuation.

- To Rectify the class imbalance installing the python package known as `Augmentor` (https://augmentor.readthedocs.io/en/master/) to add more samples across all classes so that none of the classes have very few samples.

- So, now we have added 500 images to all the classes to maintain some class balance. We can add more images as we want to improve training process.

- In final iteration, class rebalancing helped reduce the overfitting, but it also reduced the model accuracy both on training and validation sets. This suggests a bigger model may be used to further improve accuracy. 

- Regularising with the help of droupout layers and batch normalisation helped improve the model performance.


## Technologies Used

Google colab - Version: 0.0.1a2
Python - Version: 3.10.12
tensorflow - Version: 2.15.0



## Contact
Created by [@shaguftakhan] and [@KarthikMishra] - feel free to contact!

