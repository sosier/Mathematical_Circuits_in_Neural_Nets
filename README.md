# Mathematical Circuits in Neural Nets

By: Sean Osier

## Motivation

[Olah et al.](https://distill.pub/2020/circuits/zoom-in/) make three claims about the fundamental interpretability of neural networks:

![Three Claims](https://user-images.githubusercontent.com/13408985/189792395-8c4ee31b-3d4b-42db-aa62-6a05e3ae6b0c.png)

They demonstrates these claims in the context of image models:

*Features / Circuits:*

![Features / Circuit](https://user-images.githubusercontent.com/13408985/189792613-42663d32-3e48-4a3b-846d-331714dca639.png)

*Universality:*

![Universality](https://user-images.githubusercontent.com/13408985/189792851-3a05d17b-cb22-4b7f-a6fd-09775510401a.png)

This work demonstrates the same concepts apply in the space of neural networks modeling basic mathematical functions.

## Results

Specifically, I show that the optimal network for calculating the minimum of two arbitary numbers, is fully constructed from smaller "features" and "circuits" used across even simpler mathematical functions such as:
 - "Positiveness" and "Negativeness" Detectors
 - Identity Circuits (i.e. f(x) = x)
 - Negative Identity Circuits (i.e. f(x) = -x)
 - "Greaterness" Detectors
 - Subtraction Circuits (i.e. f(x1, x2) = x1 - x2)
 
*Minimum Network:*

![Minimum Network](https://user-images.githubusercontent.com/13408985/189795184-f6bc5477-dde0-4042-b200-559a2f02f10d.png)

I also demonstrate that these theoretical results hold in practice*. [The code for these experiments](Mathematical_Circuits.ipynb) can be found in the Jupyter Notebook in this repo. 

For full details, please see the [PDF presenation](Basic_Neural_Network_Circuits.pdf) in this repo.

--- 

_* For full disclosure, while I was able to replicate all the smaller "features" and "circuits" discussed, I haven't been able to get my minimum network to learn the optimal configuration. Right now, it gets stuck in a local minimum. (I think the issue may be related to the fact that certain weights have to be completley zeroed out in the optimal network.) Getting the model to actually learn the optimal weights is the primary next step for this work._
