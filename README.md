Project Name: Melanoma-CNN-Prediction

Problem statement: 
  To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin   cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

Objective:
  To build a multiclass classification model using a custom convolutional neural network in TensorFlow.

  The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


The data set contains the following diseases:

  Actinic keratosis
  Basal cell carcinoma
  Dermatofibroma
  Melanoma
  Nevus
  Pigmented benign keratosis
  Seborrheic keratosis
  Squamous cell carcinoma
  Vascular lesion


Project Pipeline:
    1.	Data Reading/Data Understanding →  The path for train and test images 
    2.	Dataset Creation→ Created train & validation dataset from the train directory with a batch size of 32. Resized  images to 180*180.
    3.	Dataset visualisation → Created a code to visualize one instance of all the nine classes present in the dataset 
    4.	Model Building & training→
          --- Created a CNN model, which can accurately detect 9 classes present in the dataset.
          --- While building the model, rescaled the images to normalize pixel values between (0,1).
          ---Chosen an appropriate optimiser and loss function for model training
          ----Trained the model for ~20 
    5.	Chosen an appropriate data augmentation strategy to resolve underfitting/overfitting 
    6.	Model Building & training on the augmented data→ 
          --- Created a CNN model, which can accurately detect 9 classes present in the dataset.
          --- While building the model, rescaled the images to normalize pixel values between (0,1).
          ---Chosen an appropriate optimiser and loss function for model training
          ----Trained the model for ~20 
    7.	Class distribution →Examined the presence of class imbalance in the training dataset 
    8.	Handling class imbalances→ Rectified class imbalances present in the training dataset with Augmentor library.
    9.	Model Building & training on the rectified class imbalance data→
          --- Created a CNN model, which can accurately detect 9 classes present in the dataset.
          --- While building the model, rescaled the images to normalize pixel values between (0,1).
          ---Chosen an appropriate optimiser and loss function for model training
          ----Trained the model for ~50

Project Findings:
  1.	Outcome of general model before augmentation and class imbalance:
    --- In Model-1 Model accuracy on training data accuracy: 95% and Val accuracy: 78%.So highly over fitting .
    --- In Model-2 Model accuracy on training data accuracy: 96% and Val accuracy: 81%. So over fitting is present, but lesser than Model-1

  2.	Outcome of model after augmentation:

        There is no overfitting present  but model accuracy is low

  3.	Findings of class distribution:
    ----Class-6 has the least number of samples
    ----Class-5,Class-3,Class-1 and Class-4 dominate the data in terms proportionate number of samples

  4.	Outcome of  model after rectifying the class imbalance:
    ---There is no over fitting  present now and the accuracy of train data and val_accuracy increases.

Technology Used:
      Tensorflow Library Version: 2.9.2

Acknowledgement:
      We would like to thank UpGrad and IIIT Bangalore for all the support and learnings. It has been an incredible experience learning the right concepts and methodologies to execute ML and DL based projects of any level of complexities. 

Contact:
    Created by;
                1.  Gaurav Kumar --> https://github.com/Gktwinkle,
                2.  Dipshikha Mudoi --> https://github.com/dipsikhamudoi,
                3.  Rohit Mishra --> https://github.com/rohitmishra6300

                                                                               - feel free to contact us!
