# Neural Style Transfer with PyTorch

## Overview

This Jupyter notebook, demonstrates the implementation of Neural Style Transfer using PyTorch. The primary goal is to apply artistic styles to existing images.

## Dependencies

The key Python libraries used in this notebook are:

- **torch**: The PyTorch library for training neural networks.
- **torch.nn**: A sub-library providing classes for defining neural network layers.
- **torchvision**: A library for working with pre-trained models.
- **PIL**: Python Imaging Library for image file manipulation.
- **matplotlib**: A library for creating visualizations in Python.
- **numpy**: A library supporting large, multi-dimensional arrays and matrices, along with mathematical functions.

## Implementation

The notebook begins by importing necessary libraries and defining the computation device. It utilizes the pre-trained VGG19 model from torchvision to extract features capturing content and style information.

Functions are defined for transforming input images to the required format and reversing this transformation.

The core of the notebook is the `fit` function, optimizing a noise image to match the content features of a target image using the Adam optimizer and mean squared error loss.

The notebook also includes code to download and instantiate the pre-trained VGG19 model.

## Usage

To use this notebook:

1. pip install -r requirements.txt
2. Import required libraries.
3. Define the computation device.
4. Instantiate the VGG19 model.
5. Define transformation functions.
6. Load content and style images.
7. Run the `fit` function to generate an image matching the content.

You can add your own images to try out.

## Conclusion

Neural Style Transfer finds applications in various domains, from artistic expression to content personalization. However, its efficiency and success heavily depend on fine-tuning parameters, layer choices, and the choice of optimization algorithms. You can play around with content and style layers.
