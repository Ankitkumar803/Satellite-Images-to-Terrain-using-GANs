# Satellite-Images-to-Terrain-using-GANs

This notebook demonstrates how to use Generative Adversarial Networks (GANs) to convert satellite images to terrain height maps.

## Introduction
The goal of this project is to generate terrain height maps from satellite images using GANs. The idea is to use the GAN architecture to learn the mapping between the satellite images and the corresponding terrain height maps.

The dataset used in this notebook is the [Pix2Pix Maps from kaggle](https://www.kaggle.com/datasets/alincijov/pix2pix-maps) which provides global terrain elevation data at a resolution of 1 arc-second. We will use the rasterio library to load and manipulate the SRTM data.

## Implementation
The GAN architecture used in this project is a modified version of the pix2pix GAN. The generator takes a satellite image as input and generates a terrain height map as output. The discriminator takes a pair of satellite image and terrain height map as input and tries to distinguish between real and generated pairs.

We will train the GAN on a small subset of the SRTM dataset and use it to generate terrain height maps for unseen satellite images.

The notebook has the following sections:

- Load the dataset
- Preprocess the data
- Define the GAN architecture
- Train the GAN
- Generate terrain height maps
- Visualize the results
## Results
The GAN was able to learn the mapping between the satellite images and the corresponding terrain height maps. The generated terrain height maps are smooth and exhibit similar features to the real terrain height maps.

##Conclusion
In this notebook, we have demonstrated how to use GANs to generate terrain height maps from satellite images. We have used a modified version of the pix2pix GAN architecture and trained it on a small subset of the SRTM dataset. The results show that the GAN is able to generate realistic terrain height maps from satellite images.

##References
- [Generative Adversarial Networks (GANs)](https://en.wikipedia.org/wiki/Generative_adversarial_network)
- [Image-to-Image Translation with Conditional Adversarial Networks (pix2pix)](https://arxiv.org/abs/1611.07004)
