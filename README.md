# NeRF based 3D Reconstruction and Neural view Synthesis

This project provides an implementation of a Neural Radiance Field (NeRF) renderer using PyTorch. NeRF is a method for synthesizing novel views of complex scenes by directly optimizing a neural network to represent the scene's volumetric scene function.

## Overview
Neural Radiance Fields (NeRF) has emerged as a groundbreaking technique in the realm of 3D scene representation and rendering. By leveraging the power of neural networks, NeRF synthesizes novel views of intricate scenes without the need for traditional 3D modeling. This project offers a streamlined implementation of NeRF, aiming to provide users with the core functionalities of this technique without the overhead of more extensive frameworks. Written in C++, the codebase harnesses the capabilities of LibTorch, PyTorch's C++ API, ensuring efficient computations and leveraging automatic differentiation. Whether you're a researcher looking to experiment with NeRF or a developer aiming to integrate it into a larger system, this project serves as an ideal starting point.

The main functionality of this project is to train a NeRF model using a set of images, poses, and focal lengths. Once trained, the model can be used to render high-resolution images from different viewpoints.

**Key features include:**
- Parsing command-line arguments for data and output paths.
- Setting a random seed for reproducibility.
- Loading data tensors from binary files.
- Training the NeRF model using the Adam optimizer.
- Rendering images using the trained model.
- Saving rendered images to disk.

## Results
After running the NeRF renderer, you will obtain synthesized views of your input scenes. These views are generated based on the trained NeRF model and will be saved in the specified output directory. The quality and accuracy of the results depend on the training data and the number of iterations the model has been trained for.

You can visualize the results using any standard image viewer or incorporate them into further post-processing workflows. The generated images offer a novel perspective of the scene, showcasing the power of Neural Radiance Fields in 3D scene representation and rendering.