# Image-Generation-with-GAN-on-MNIST-Dataset

In this assignment, I have implemented a Generative Adversarial Network (GAN) using the MNIST dataset. The project was completed using Python 3 and PyTorch.

## Dataset
The MNIST dataset consists of handwritten numbers and their corresponding labels. Each MNIST image is a 28x28 grayscale image labeled with an integer value between 0 and 9, representing the actual value in the image. The dataset contains 60,000 images and labels for training and 10,000 images and labels for testing. Since this project is an unsupervised learning task, only the 60,000 images from the training set were used.

To download the MNIST dataset directly in PyTorch, the following code snippet was used:

```python
from torchvision import datasets

mnist_trainset = datasets.MNIST(root='./data', train=True, download=True, transform=None)
mnist_testset = datasets.MNIST(root='./data', train=False, download=True, transform=None)
```

## Implementation
The implementation involved developing a GAN architecture using PyTorch to generate realistic handwritten digits resembling those in the MNIST dataset. The GAN model consists of a generator network and a discriminator network trained simultaneously in a minimax game framework.


## Next Steps
Moving forward, I plan to explore further enhancements to the GAN model, such as experimenting with different architectures, optimization techniques, and hyperparameter tuning, to improve the quality of generated images. Additionally, I aim to apply GANs to other datasets and explore their applications in various domains.
