# (Deep Convolutional Generative Adversarial Network)-MNIST dataset

Generative Adversarial Networks (GANs) are one of the most interesting ideas in computer science today. Two models are trained simultaneously by an adversarial process. A generator ("the artist") learns to create images that look real, while a discriminator ("the art critic") learns to tell real images apart from fakes. During training, the generator progressively becomes better at creating images that look real, while the discriminator becomes better at telling them apart. The process reaches equilibrium when the discriminator can no longer distinguish real images from fakes. This notebook demonstrates this process on the MNIST dataset. 

Implemented DCGAN on MNIST dataset using Pytorch. The below gif shows how quickly dcgan learns the distribution of mnist and generates real looking digits.




![](https://github.com/chiggshiggs/dcgan-MNIST/blob/main/animated.gif)


## How Gan's Work:
* The Gan's were introduced by Ian Goodfellow in 2014. Generative adversarial networks (GANs) are algorithmic architectures that use two neural networks, pitting one against the other (thus the “adversarial”) in order to generate new, synthetic instances of data that can pass for real data.

* It is more like a chor police game or a minimax game where the chor tries to counterfeit notes and everytime the chor makes a mistake it is penalized and it tries to get better and better on counterfeiting the notes and the police tries to catch the chor evrytime and the police gets better and better on catching the chor . At some point of time the police would not be able to tell the difference between real and fake notes. 

* Discrminator Loss: △ log( Discriminator(Real image) ) + ( 1 - Discriminator(Generated Image) )<br>
Generator Loss: ▽ log(1-Discrminator(Generated image))<br>
(Note: △ symbol means maximize and ▽ symbol means minimize )

* Below given is a architectural view of GAN.<br><kbd><img src="https://miro.medium.com/max/601/1*Y_AGVp0EEGEpB1Q25G6edQ.jpeg"/></kbd>

