---
### Tricks
1. Use leaky relu in down-sampling and relu in up-sampling 
    - https://arxiv.org/abs/1703.05192

1. Use L1 distance instead of L2 in image reconstruction since L2 often leads blurriness
    - https://arxiv.org/abs/1704.02510
    - https://arxiv.org/abs/1703.10593
    - [pix2pix](https://arxiv.org/abs/1611.07004)

1. Network architectures
    - 

1. Optimizing just for similarity in a high-level feature space typically leads to high-frequency artifacts. This is because for each natural image there are many non-natural images mapped to the same feature vector.
    - http://arxiv.org/abs/1602.02644

---
### Enhancement
1. TV loss for smoothness
    - https://link.springer.com/chapter/10.1007/978-3-319-46475-6_43

---
### Traps

#### Coding Traps
1. To keep an eye on your image range [-1.0, 1.0], [0.0, 1.0] or [0, 255]

#### Technique Traps
1. WGAN-GP
    - the normalization in discriminator shouldn't be batch normalization