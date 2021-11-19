# Generative-Deep-Learning

## Some of the most popular GAN architectures are :
1. CycleGAN   
2.StyleGAN  
3.LSGAN   
4.DiscoGAN    

### 1. CycleGAN
It is a technique that involves the automatic training of image to image translation models without paired examples. Example of the image to image translation is translating horse to zebra or vice versa. CycleGAN uses a cycle consistency loss to enable training without the need for paired data. It can translate from one domain to another without a one-to-one mapping between the source and the target domain. The goal of the image-to-image translation problem is to learn the mapping between an input image and an output image using a training set of aligned image pairs.
For two domains X and Y, CycleGAN learns a mapping G:X -> Y and F:Y -> X.
CycleGAN has three sections: Encoder, Transformer and Decoder.
CycleGAN can be helpful when there is a need for colour transformation.

### 2. StyleGAN
Introduced by Nvidia researchers, StyleGAN is a novel generative adversarial network.The StyleGAN is an extension to the GAN architecture that proposes large changes to the generator model, including the use of a mapping network to map points in latent space to an intermediate latent space, the use of the intermediate latent space to control style at each point in the generator model, and the introduction to noise as a source of variation at each point in the generator model.
The resulting model is capable not only of generating impressively photorealistic high-quality photos of faces, but also offers control over the style of the generated image at different levels of detail through varying the style vectors and noise.

### 3. LSGAN(Least Square Adversial Network)
In a normal GAN, the discriminator uses cross-entropy loss function which sometimes leads to vanishing gradient problems. Instead of that LSGAN uses the least-squares loss function for the discriminator. It has the desire to provide a signal to the generator about the fake samples that are far from the discriminator model’s decision boundary for classifying them as real or fake. It can be implemented with a minor change to the output layer of the discriminator layer and the adoption of the least-squares, or loss function.

### 4. DiscoGAN
It generates images of products in domain B given an image in domain A. It transfers elements from one image to another.
DiscoGAN has two generators. The first generator maps the input image from Domain A to Domain B. The second generator reconstructs the image from Domain B to Domain A.
There is a slight similarity between CycleGAN and DiscoGAN. In CycleGAN it has an addition hyperparameters to adjust the contribution of reconstruction/cycle-consistency loss in the overall loss function.
DiscoGAN can be used for transferring decoration from a fashion item such as a bag to another fashion item as a pair of shoes.
Conclusion
There are thousands of papers on GANs and many hundreds of named-GANs, that is, models with a defined name that often includes “GAN“.There can be some difficulties while creating a new architecture using the GAN architecture. It is known that training GAN networks is highly unstable. Hyperparameter optimization is difficult to find the right balance between learning rates to efficiently train the network. In all of the architectures generators is most used for training the data.
