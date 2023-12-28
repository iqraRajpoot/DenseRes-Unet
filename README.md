# DenseRes-Unet: Segmentation of Overlapped/Clustered Nuclei from Multi-Organ Histopathology Images

![DenseRes-Unet](link-to-your-image-here)

## Overview
This repository contains the implementation of DenseRes-Unet, a convolutional neural network model designed for segmenting clustered or overlapped nuclei from multi-organ histopathology images. DenseRes-Unet combines the strengths of dense connections and residual paths for enhanced performance in segmentation tasks.

## Model Description
The DenseRes-Unet architecture is constructed with a series of convolutional, batch normalization, and ReLU activation layers. The model consists of:
- **ConvBNReLU Blocks:** These blocks perform convolution, batch normalization, and ReLU activation.
- **ResPath Blocks:** These blocks establish residual connections between layers to aid in feature propagation.
- **Final Convolution Layer:** Concludes the network for generating the segmented output.

## Input Image Size
The model expects input images with dimensions of 256x256 pixels.

## Usage
### Requirements
- PyTorch
- Torchvision

### Training the Model
To train the DenseRes-Unet model, follow these steps:
1. Prepare your dataset in the required format.
2. Set the input image size to 256x256 pixels.
3. Instantiate the model using the provided code.
4. Define your training routine using appropriate loss functions and optimizers.
5. Train the model on the mentioned dataset.

### Datasets

1. MonuSeg-2018
   https://www.kaggle.com/datasets/tuanledinh/monuseg2018 
2. CryoNuSeg
   https://www.kaggle.com/datasets/ipateam/segmentation-of-nuclei-in-cryosectioned-he-images
3. BBBC039V
   https://bbbc.broadinstitute.org/BBBC039

### Citation
If you find this work helpful for your research, please consider citing:

```
@article{DenseResUnet2022,
  title = {DenseRes-Unet: Segmentation of overlapped/clustered nuclei from multi-organ histopathology images},
  journal = {Computers in Biology and Medicine},
  volume = {143},
  pages = {105267},
  year = {2022},
  url = {https://www.sciencedirect.com/science/article/abs/pii/S0010482522000592},
  author = {Iqra Kiran and Basit Raza and Areesha Ijaz and Muazzam A. Khan}
}
```

