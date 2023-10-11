# Melanoma Cancer Detection using CNN
> <strong>Problem statement:</strong> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

> The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


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

## Project Pipeline
* <strong>Data Reading/Data Understanding </strong> → Defining the path for train and test images
* <strong>Dataset Creation</strong> → Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
* <strong>Model Building & training </strong> <br/>
    * Creating a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1). <br/>
    * Choosing an appropriate optimiser and loss function for model training <br/>
    * Training the model for ~20 epochs <br/>
    * Findings after the model fit. Checking if there is any evidence of model overfit or underfit. <br/>
* <strong>Class distribution:</strong> Examine the current class distribution in the training dataset <br/>
    → Which class has the least number of samples? <br/>
    → Which classes dominate the data in terms of the proportionate number of samples? <br/>
* <strong>Chosing an appropriate data augmentation strategy to resolve underfitting/overfitting </strong>
* <strong>Handling class imbalances:</strong> Rectifying class imbalances present in the training dataset with [Augmentor](https://augmentor.readthedocs.io/en/master/) library.
* <strong>Model Building & training on the rectified class imbalance data </strong> <br/>
    * Creating a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1). <br/>
    * Choosing an appropriate optimiser and loss function for model training <br/>
    * Training the model for ~30 epochs <br/>
    * Findings after the model fit. Checking if there is any evidence of model overfit or underfit. <br/>
* <strong>Class distribution:</strong> Examine the current class distribution in the training dataset <br/>
    → Which class has the least number of samples? <br/>
    → Which classes dominate the data in terms of the proportionate number of samples? <br/>
* <strong>Prediction with test images </strong>

## Technologies Used
- Python
- Google Colab
- T4 GPU by Google Colab

## Python Libraries Used
- pathlib - Version: 1.0.1
- tensorflow - Version: 2.13.0
- matplotlib - Version: 3.7.1
- numpy - Version: 1.23.5
- pandas - Version: 1.5.3
- os
- PIL
- google-colab - Version: 1.0.0
- seaborn - Version: 0.12.2
- glob

## Contact
Created by [@janardanchavan] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->