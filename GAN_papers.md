### Frameworks
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434)
1. [cGAN](arxiv.org/abs/1411.1784)
1. [LAPGAN](http://papers.nips.cc/paper/5773-deep-generative-image-models-using-a-laplacian-pyramid-of-adversarial-networks.pdf) - Coarse-to-fine generation
1. [DeLiGAN](https://arxiv.org/abs/1706.02071) - Mixture Gaussian prior distribution
1. [AGE](https://arxiv.org/abs/1704.02304) - $max_emin_g\Delta(e(g(Z))||Y)-\Delta(e(X)||Y)$ and encoder-generator reciprocity(bidirectional mapping)


### Divergence, Objective Function
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434) - JS divergence
1. [LSGAN(Least Squares GAN)](https://pdfs.semanticscholar.org/0bbc/35bdbd643fb520ce349bdd486ef2c490f1fc.pdf) - Pearson χ2 divergence
1. [f-GAN](https://arxiv.org/abs/1606.00709) - f-divergence
1. [EBGAN](https://arxiv.org/abs/1609.03126) - $D(x) = ||Dec(Enc(x)) − x||$
1. [LS-GAN(Loss-Sensitive GAN)](https://arxiv.org/abs/1701.06264)
1. [BEGAN](https://arxiv.org/abs/1703.10717) - Wasserstein distance between the distribution of real/fake auto-encoder loss

#### IPM
1. [McGAN]()
1. [WGAN](https://arxiv.org/abs/1701.07875) - Wasserstein distance
    - [WGAN-GP](https://arxiv.org/abs/1704.00028) - Gradient penalty
1. [Geometric GAN](https://arxiv.org/abs/1705.02894) - SVM margin
1. [Fisher GAN](https://arxiv.org/abs/1705.09675) - Chi-squared distance


### Lantern space disentangling
1. [InfoGAN](https://arxiv.org/abs/1606.03657) - Unsupervised lantern space disentangling


### Evaluations of GANs
1. [AMT perceptual studies - pix2pix](https://arxiv.org/pdf/1611.07004.pdf)
1. [FCN score - pix2pix](https://arxiv.org/pdf/1611.07004.pdf)
1. [Semantic segmentation metrics - CycleGAN](https://arxiv.org/abs/1703.10593)
1. [Inception score - Improved GAN](https://arxiv.org/abs/1606.03498)


### Applications

#### Image to Image Translation
1. [CycleGAN](https://arxiv.org/abs/1703.10593)
1. [DiscoGAN](https://arxiv.org/abs/1703.05192)
1. [DualGAN](https://arxiv.org/abs/1704.02510)