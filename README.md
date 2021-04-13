# Keras3D Image Classifcation with TensorBoard Logging 

![3D Brain Scan Segments](https://keras.io/img/examples/vision/3D_image_classification/3D_image_classification_19_0.png)


This demo is a slighly modifed version of the [Keras 3D Image Classification from CT Scans
](https://keras.io/examples/vision/3D_image_classification/) by  Hasib Zunair with the addtion of argparse and tensorboard logging. 

The example show the steps needed to build a 3D convolutional neural network (CNN) to predict the presence of viral pneumonia in computer tomography (CT) scans. 2D CNNs are commonly used to process RGB images (3 channels). A 3D CNN is simply the 3D equivalent: it takes as input a 3D volume or a sequence of 2D frames (e.g. slices in a CT scan), 3D CNNs are a powerful model for learning representations for volumetric data. It uses a subset of the [MosMedData: Chest CT Scans with COVID-19 Related Findings](https://arxiv.org/abs/2005.06465). This dataset consists of lung CT scans with COVID-19 related findings, as well as without such findings.

For more information please read the [original tutorial here](https://keras.io/examples/vision/3D_image_classification/)


## Running the Code

```
python train.py --max_epochs 3
```
