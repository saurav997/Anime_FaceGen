# Anime Face Generation with Generative Adversarial Networks

This repository contains code for generating anime faces using a Generative Adversarial Network (GAN).

## Project Description:

This project implements a Deep Convolutional GAN (DCGAN) architecture to create new anime faces based on a dataset of existing anime images. The GAN consists of two main components:

- **Generator:** A neural network that learns to generate realistic anime faces from random noise vectors.
- **Critic:** A neural network that discriminates between real anime faces from the dataset and fake faces generated by the generator.

The generator and critic are trained in an adversarial process. The generator tries to improve its ability to create realistic faces that fool the critic, while the critic tries to become better at distinguishing real from fake faces.

## Requirements:

- Python 3.6+
- PyTorch
- torchvision
- datasets
- tqdm
- matplotlib

## Running the Script:

1. Clone this repository.
3. Download the Anime Face Dataset (instructions provided in the dataset source).
4. Update the dataset path in the `load_dataset` function within the script (`anime_facegen.py`).
5. Run the script using `python anime_facegen.py`.

## Training Process:

The script trains the GAN for a specified number of epochs. During training, it will periodically display generated images and training loss metrics. Saved checkpoints of the generator model will be created at specific intervals for later use.

## Generated Images:

The script will display a grid of generated anime faces throughout the training process. You can also use the saved generator models to generate new faces after training is complete.

## Further Exploration:

This is a basic implementation of a DCGAN for anime face generation. You can explore further improvements by:

- Experimenting with different network architectures for the generator and critic.
- Training on a larger dataset of anime images.
- Conditioning the generator on additional inputs, such as facial expressions or hairstyles.

## Disclaimer:

This code is provided for educational purposes only. The dataset used in this project may have usage restrictions. Please refer to the dataset source for details.
