# Fashion MNIST Image Generator using GAN

This is a project for generating fashion item images using a Generative Adversarial Network (GAN). In this project, we will use TensorFlow to implement and train a GAN model for generating fashion item images from random noise.

## Prerequisites

Before running the code, ensure you have the following prerequisites:

- TensorFlow
- TensorFlow Datasets
- NumPy
- Matplotlib
- Python 3.x
- GPU (optional but recommended for faster training)

## Getting Started

Follow these steps to get started with the project:

1. Clone the repository or download the code file.
2. Install the required dependencies using `pip install tensorflow tensorflow-datasets numpy matplotlib` or `pip install -r requirements.txt`.
3. Run the code in your Python environment. Make sure you have a compatible GPU for faster training, as the code is set to utilize GPU if available.

## Dataset

This project uses the Fashion MNIST dataset, which consists of grayscale images of fashion items. The dataset is automatically loaded and prepared in the code.

## Training

The training loop is defined in the `fit` method of the GAN model in the code. The code will train the GAN for a specified number of epochs, generating and saving images after each epoch.

## Model Architecture

The code includes the definition of the generator and discriminator models. The generator takes random noise as input and generates fashion item images. The discriminator tries to distinguish between real and fake images.

## Custom Training Loop

A custom training loop is implemented in the code, which involves training both the discriminator and generator. This loop calculates losses and updates model weights accordingly.

## Callback

A custom callback is defined to monitor the model's progress and save generated images after each epoch.

## Reviewing Performance

The code allows you to review the model's performance by plotting the discriminator and generator losses over epochs.

## Generating Images

The trained generator can be used to generate fashion item images. You can see the generated images in the code.

## Saving the Models

The trained generator and discriminator models can be saved for later use using `generator.save('generatormodel.h5')` and `discriminator.save('discriminatormodel.h5')`.

Feel free to modify the code or experiment with different parameters to generate various fashion item images using GAN.

Enjoy generating fashion item images with your GAN model!