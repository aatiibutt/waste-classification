# Waste Classification Using Convolutional Neural Network

## Pre-Requisites
1. Anaconda (https://www.anaconda.com/products/individual)
2. Pytorch (https://pytorch.org/get-started/locally/)
3. Waste Classification Binary Class Dataset (https://www.kaggle.com/techsash/waste-classification-data)
4. Thung and Wang's Dataset (https://github.com/garythung/trashnet/blob/master/data/dataset-resized.zip)

## Data Augmentation

To add more diversity in dataset, we have performed four types of data augmentations including,

- Gaussian Blur
- Horizontal Flip
- Contrast

You can use the **Augmentation.ipynb** in **Train_Notebooks** to perform augmentation on the provided dataset.

## Training

To this end, three state-of-the-art CNNs i.e. **GoogleNet** , **Resnet-152**, **VGG**, **ResNext** and the proposed architecture **ResNext-Plus** are employed to perform classification. It is important to mention here that, pre-trained CNNs are downloaded, and trained through transfer learning to achieve effective results. All the networks are available in above-folder named **Trained Notebooks**. All the trained models are available in above-folder **models**.

## Results
The experiments are performed on both i.e. the augmented and non augmented datasets to analyse the difference through adaptive and static learning rate. The experiments showed that Resnext-plus achieved better accuracy on augmented dataset with adaptive learning rate.

#### GoogleNet
- With Adaptive Learning Rate on non-Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/google-non.PNG?raw=true)

- With Adaptive Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/google-aug.PNG?raw=true)

#### Resnet

- With Adaptive Learning Rate on non-Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/res-non.PNG?raw=true)

- With Adaptive Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/res-aug.PNG?raw=true)

#### VGG

- With Adaptive Learning Rate on non-Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/vgg-non.PNG?raw=true)

- With Adaptive Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/vgg-aug.PNG?raw=true)

#### ResNext

- With Adaptive Learning Rate on non-Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/resnxt-non.PNG?raw=true)

- With Adaptive Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/resnxt-aug.PNG?raw=true)

#### ResNext-Plus

- With Adaptive Learning Rate on non-Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/resnxt-non.PNG?raw=true)

- With Adaptive Learning Rate on Augmented Dataset

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/respls-aug.PNG?raw=true)

#### ResNext-Plus on Sencond Dataset (Thung and Yang’s)

![alt text](https://github.com/aatiibutt/waste-classification/blob/main/graph/resnxtpls-seconddata.PNG?raw=true)

