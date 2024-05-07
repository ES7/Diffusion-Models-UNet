# Diffusion-Models-UNet
What is the goal of diffusion models? Well we have a lot of training data, such as sprite images of video game characters. We want even more of these sprites that are not represented in our training data set and we can use a neural neotwork that can generate more of these sprites following the diffusion model process.<br>
How do we make these images useful to the neural network? We want the neural network to learn generally the concept of a sprite, what it is. And that could be finer details. Such as the hair color of the sprite, or it wears a buckle for its belt. It also could be general outlines like of its head and body. And one way to take the data and be able to emphasize either finer details or general outlines, is actually to add different levels of noise. So this is just adding noise to the image. And it is known as the "Noising Process".<br>
What should the neural network be thinking at each level of noise? When it is in the first image we want neural network to say "it's Bob the sprite", if it is the second image then neural network should say "there is some noise" and suggest possible details to make it look just like the first image. And if it is just an outline of the sprite then we only get a sense that this is probably a sprite person so here we need to suggest more details.<br>
The neural network learns to take different noisy images and turn them back into sprites. It learns to remove the noise we added. The no idea level of noise is important because it is normally distributed. Means each of the pixels is sampled from a normal distribution also known as a "Gaussian distribution" or "bell-shaped curve". After getting the noisy image, pass it into the NN and we will get a completely new image.

**`1. Sampling_&_Model_Architecture.ipynb:`** In this notebook you will get to know how sampling works across multiple iterations and the UNet architecture used for diffusion models.

**`2. Training.ipynb:`** Here you will get to know about the training of the UNet model.

**`3. Context.ipynb:`** In this notebook you will see how we can pass an image with a caption or description.

**`4. FastSampling.ipynb:`** In this notebook you will see an improved way of sampling and how quickly you can generate output.
