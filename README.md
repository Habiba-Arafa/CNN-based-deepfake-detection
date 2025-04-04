# DeepFake Detection using CNNs

## Overview

Using deep learning model to detect deepfake images by using Convolutional Neural Networks (CNNs). it integrates 3 datasets for training and testing to make model learn robust features achieving high accuracy to distinguish between  real and fake images.
---


##  Datasets  Used

- **DeepFake and Real Images (https://www.kaggle.com/datasets/manjilkarki/deepfake-and-real-images)**
- **FaceForensics (https://www.kaggle.com/datasets/greatgamedota/faceforensics)**
- **DFDC Faces of the Train Sample (https://www.kaggle.com/datasets/itamargr/dfdc-faces-of-the-train-sample)**

---

### Model Architecture

- **TThe model consists of the following layers:**T
- **Three blocks of Conv2D + Conv2D + MaxPooling2D**
- **Flatten layer**
- **Dropout layer (0.5)**
- **Two Dense layers with ReLU activation**
- **Final Dense layer with sigmoid activation for binary classification



---
###Training
the dataset was normalized , the model trained on 20 epochs using Adam optimizer also using EarlyStopping and ReduceLROnPlateau callbacks for optimization.



---

## Results 

- The model was evaluated on the three 3 datasets :
- FaceForensics achieved 98.94% , Loss 0.034
- DFDC Faces achieved 81.87% , Loss 1.30
- DeepFake and Real Images achieved 71.12% , Loss 1.76


