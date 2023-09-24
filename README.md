# DCGAN with cifar10

Cifar10 is a benchmark dataset.
DCGAN stands for Deep Convolutional Generative Adversarial Network.
The adversity stems from two competing models (generator and discriminator) and works in a tom and jerry fashion, as the generator *creates* "realistic" images and the discriminator tries to *debunk* them. 
The two models work in an endless cycle (if allowed) with the possibility of mode collapse though that is not guaranteed. It would be cool to see though.

The generator starts with random noise pixel values and works its way up to replicating patterns from the cifar10 dataset.

I trained them for 100 epochs which is overkill, and saved an image for every epoch, resulting in a beautiful gif which is ruined by matplotlibs weird colors. I tried other colormaps but they were somehow worse.
Despite everything looking radioactive, at least you can make out the shapes.

![](/cifar10/dcgan.gif)