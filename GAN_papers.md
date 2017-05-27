### Frameworks
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434)
1. [cGAN](arxiv.org/abs/1411.1784)

### Divergence, Objective Function
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434) - JS divergence
2. [WGAN](https://arxiv.org/abs/1701.07875) - Wasserstein distance
    - [WGAN-GP](https://arxiv.org/abs/1704.00028) - Gradient penalty
3. [EBGAN](https://arxiv.org/abs/1609.03126) - D(x) = ||Dec(Enc(x)) − x||
4. [LSGAN](https://pdfs.semanticscholar.org/0bbc/35bdbd643fb520ce349bdd486ef2c490f1fc.pdf) - Pearson χ2 divergence
5. [BEGAN](https://arxiv.org/abs/1703.10717) - Wasserstein distance between the distribution of real/fake auto-encoder loss

### Evaluations of GANs
1. [AMT perceptual studies - pix2pix](https://arxiv.org/pdf/1611.07004.pdf)
2. [FCN score - pix2pix](https://arxiv.org/pdf/1611.07004.pdf)
3. [Semantic segmentation metrics - CycleGAN](https://arxiv.org/abs/1703.10593)
4. [Inception score - Improved GAN](https://arxiv.org/abs/1606.03498)

### Applications
#### Image to Image Translation
1. [CycleGAN](https://arxiv.org/abs/1703.10593)
2. [DiscoGAN](https://arxiv.org/abs/1703.05192)
3. [DualGAN](https://arxiv.org/abs/1704.02510)