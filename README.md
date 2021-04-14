# Keras 3D Image Classification with TensorBoard Logging 


## Run with Grid

[![Grid](https://img.shields.io/badge/rid_AI-run-78FF96.svg?labelColor=black&logo=data:image/svg%2bxml;base64,PHN2ZyB3aWR0aD0iNDgiIGhlaWdodD0iNDgiIGZpbGw9Im5vbmUiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggZD0iTTEgMTR2MjBhMTQgMTQgMCAwMDE0IDE0aDlWMzYuOEgxMi42VjExaDIyLjV2N2gxMS4yVjE0QTE0IDE0IDAgMDAzMi40IDBIMTVBMTQgMTQgMCAwMDEgMTR6IiBmaWxsPSIjZmZmIi8+PHBhdGggZD0iTTM1LjIgNDhoMTEuMlYyNS41SDIzLjl2MTEuM2gxMS4zVjQ4eiIgZmlsbD0iI2ZmZiIvPjwvc3ZnPg==)](https://platform.grid.ai/#/runs?script=https://github.com/aribornstein/Keras3DImageClassifcation/blob/800e59c500af6a80c692d8a46b43c94505718adf/train.py&cloud=grid&instance=g4dn.xlarge&accelerators=1&disk_size=200&framework=tensorflow&script_args=grid%20train%20train.py%20--g_gpus%201%20--g_instance_type%20g4dn.xlarge%20--g_framework%20tensorflow%20--max_epochs%205)

![3D Brain Scan Segments](https://keras.io/img/examples/vision/3D_image_classification/3D_image_classification_19_0.png)


This demo is a slighly modifed version of the [Keras 3D Image Classification from CT Scans
](https://keras.io/examples/vision/3D_image_classification/) by [Hasib Zunair](https://hasibzunair.github.io/) from the [Keras IO examples repo](https://github.com/keras-team/keras-io/tree/master/examples). I have added tensorboard logging and argparse to enable more training customization and hyperparameter tuning. 

The example show the steps needed to build a 3D convolutional neural network (CNN) to predict the presence of viral pneumonia in computer tomography (CT) scans. 2D CNNs are commonly used to process RGB images (3 channels). A 3D CNN is simply the 3D equivalent: it takes as input a 3D volume or a sequence of 2D frames (e.g. slices in a CT scan), 3D CNNs are a powerful model for learning representations for volumetric data. It uses a subset of the [MosMedData: Chest CT Scans with COVID-19 Related Findings](https://arxiv.org/abs/2005.06465). This dataset consists of lung CT scans with COVID-19 related findings, as well as without such findings.

For more information please read the [original tutorial here](https://keras.io/examples/vision/3D_image_classification/)


## Running the Code

```
pip install -r requirements.txt
python train.py --max_epochs 3
```
