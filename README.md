# Explainable Image Captioning with SHAP and PyTorch

This project demonstrates how to explain the outputs of an image captioning model using the SHAP framework. The main objective is to understand how different parts of an input image contribute to the generated captions by using SHAP's partition explainer.

## Overview

Leveraging SHAP documentation, this notebook utilizes a pre-trained open-source model from [ImageCaptioning.pytorch](https://github.com/ruotianluo/ImageCaptioning.pytorch). The SHAP framework is used to generate explanations for the captions by masking image segments and analyzing the corresponding changes in the caption predictions.

The project uses:
- **PyTorch** for loading the pre-trained image captioning model based on **ResNet101**. Using the **DistilBART** transformer language model for alignment scoring between masked and original image captions.
- **SHAP** to explain the predictions of the image captioning model by masking various parts of the image.

## [Setup](https://shap.readthedocs.io/en/latest/example_notebooks/image_examples/image_captioning/Image%20Captioning%20using%20Open%20Source.html#Setting-up-open-source-model).

## Example Results

- SHAP will generate a visualization showing the most important regions in the image that contributed to the caption generation.