# Autoencoder-Denoiser
### A tensorflow implmentation of image denoiser using autoencder (CNN) structure.

The network consist of an encoder and a decoder. It encodes 2D images into 100 dimemsion embedding and then decodes to reconstruct 2D images. The encoder contains 2 convolutional layers and 1 fully connected layer, and the decoder contains 2 fully connected layer, 2 deconvolutional layers.
The network structure is simple, but very effective. I use mnist dataset as example. The network clearly have learnt how to remove random gaussian noise in less than 3000 iterations(not epochs) of training.

## Examples

### Training Data

Reconstructed training image (3000 iterations)<br/>
![train-3000-iters](Examples/train-3000-iters.png)

<br/>Reconstructed training image (6000 iterations)<br/>
![train-6000-iters](Examples/train-6000-iters.png)

<br/>Reconstructed training image (9000 iterations)<br/>
![train-9000-iters](Examples/train-9000-iters.png)

### Test data

Noisy image 1<br/>
![test-noisy-1](Examples/test-noisy-1.png)

<br/>Reconstructed image 1<br/>
![test-reconstructed-1](Examples/test-reconstructed-1.png)

<br/>Noisy image 2<br/>
![test-noisy-2](Examples/test-noisy-2.png)

<br/>Reconstructed image 2<br/>
![test-reconstructed-2](Examples/test-reconstructed-2.png)
