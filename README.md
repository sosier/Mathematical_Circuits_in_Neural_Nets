# Mathematical Circuits in Neural Nets

By: Sean Osier

## Motivation

[Olah et al.](https://distill.pub/2020/circuits/zoom-in/) make three claims about the fundamental interpretability of neural networks:

![Three Claims](https://user-images.githubusercontent.com/13408985/189792395-8c4ee31b-3d4b-42db-aa62-6a05e3ae6b0c.png)

They demonstrate these claims in the context of image models:

*Features / Circuits:*

![Features / Circuit](https://user-images.githubusercontent.com/13408985/189792613-42663d32-3e48-4a3b-846d-331714dca639.png)

*Universality:*

![Universality](https://user-images.githubusercontent.com/13408985/189792851-3a05d17b-cb22-4b7f-a6fd-09775510401a.png)

This work demonstrate the same concepts apply in the space of neural networks modeling basic mathematical functions.

## Results

Specifically, I show that the optimal network for calculating the minimum of two arbitrary numbers is fully constructed from smaller "features" and "circuits" used across even simpler mathematical functions. Along the way, I explore:
 - "Positiveness" and "Negativeness" Detectors
 - Identity Circuits (i.e. f(x) = x)
 - Negative Identity Circuits (i.e. f(x) = -x)
 - Subtraction Circuits (i.e. f(x1, x2) = x1 - x2)
 - "Greaterness" Detectors
 - And More

*Minimum Network:*

![Minimum Network](https://user-images.githubusercontent.com/13408985/190928502-f908fead-78f7-4568-83f6-2b1d001fafe6.png)

I also demonstrate that each of these theoretical results hold in practice. [The code for these experiments](Mathematical_Circuits.ipynb) can be found in the Jupyter Notebook in this repo. 

## Full Details

For full details, please see the [PDF presenation](Mathematical_Circuits_in_Neural_Networks.pdf) in this repo.

### Watch the Video! (Click image below)

You can watch a full walkthrough of the presenation by clicking the image below:

[![Watch the Video](Video_Thumbnail.png)](https://youtu.be/jGQN0TVCtMo)
