### Frameworks
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434)
1. [cGAN](arxiv.org/abs/1411.1784)
1. [AcGAN](https://arxiv.org/abs/1610.09585)
1. [InfoGAN](https://arxiv.org/abs/1606.03657)
1. [LAPGAN](http://papers.nips.cc/paper/5773-deep-generative-image-models-using-a-laplacian-pyramid-of-adversarial-networks.pdf) - Coarse-to-fine generation
1. [StackGAN](https://arxiv.org/abs/1612.03242) - Two step generation
1. [AGE](https://arxiv.org/abs/1704.02304) - $max_emin_g\Delta(e(g(Z))||Y)-\Delta(e(X)||Y)$ and encoder-generator reciprocity (bidirectional mapping)


### Objective Function

#### f-Divergence
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434) - JS divergence
1. [LSGAN (Least Squares GAN)](https://pdfs.semanticscholar.org/0bbc/35bdbd643fb520ce349bdd486ef2c490f1fc.pdf) - Pearson χ2 divergence
1. [f-GAN](https://arxiv.org/abs/1606.00709) - f-divergence

#### MMD
1. [GMMN](http://proceedings.mlr.press/v37/li15.pdf)
1. [MMD nets](https://arxiv.org/abs/1505.03906)

#### IPM
1. [McGAN](https://arxiv.org/abs/1702.08398) - Mean and covariance matching
1. [WGAN](https://arxiv.org/abs/1701.07875) - Wasserstein distance
    - [WGAN-GP](https://arxiv.org/abs/1704.00028) - Gradient penalty, less capacity compromise
1. [Geometric GAN](https://arxiv.org/abs/1705.02894) - SVM margin
1. [Fisher GAN](https://arxiv.org/abs/1705.09675) - Chi-squared distance

#### Others
1. [EBGAN](https://arxiv.org/abs/1609.03126) - $D(x) = ||Dec(Enc(x)) − x||$
1. [CatGAN](https://arxiv.org/abs/1511.06390) - Entropy of P(Y|X)
1. [LS-GAN (Loss-Sensitive GAN)](https://arxiv.org/abs/1701.06264)
    - https://github.com/guojunq
1. [BEGAN](https://arxiv.org/abs/1703.10717) - Wasserstein distance between the distribution of real/fake auto-encoder loss
    - https://github.com/carpedm20/BEGAN-tensorflow


### Representation Learning

#### Lantern Space Disentangling
1. [AcGAN](https://arxiv.org/abs/1610.09585) - Supervised lantern space disentangling
1. [InfoGAN](https://arxiv.org/abs/1606.03657) - Unsupervised lantern space disentangling
    - Easy comprehension - https://github.com/buriburisuri/sugartensor/blob/master/sugartensor/example/mnist_info_gan.py
    - Supervised InfoGAN - https://github.com/buriburisuri/supervised_infogan
    - Official - https://github.com/openai/InfoGAN

#### Specifying Lantern Space Distribution
1. [AAE](https://arxiv.org/abs/1511.06390)


### Unclassified
1. [Improved GAN](https://arxiv.org/abs/1606.03498)
1. [Unrooled GAN](https://arxiv.org/abs/1611.02163)
1. [DeLiGAN](https://arxiv.org/abs/1706.02071) - Mixture Gaussian prior distribution


### Evaluations of GANs
1. [FCN score - pix2pix](https://arxiv.org/pdf/1611.07004.pdf)
1. [AMT perceptual studies - pix2pix](https://arxiv.org/pdf/1611.07004.pdf)
1. [Inception score - Improved GAN](https://arxiv.org/abs/1606.03498)
1. [Semantic segmentation metrics - CycleGAN](https://arxiv.org/abs/1703.10593)


### Applications

#### Domain Adaptation, Image to Image Translation (Unpaired)
1. [DTN](https://arxiv.org/abs/1611.02200)
1. [CoGAN](http://papers.nips.cc/paper/6544-coupled-generative-adversarial-networks)
1. [UNIT](arxiv.org/abs/1703.00848)
1. [pix2pix](https://arxiv.org/abs/1611.07004)
1. [CycleGAN](https://arxiv.org/abs/1703.10593)
1. [DiscoGAN](https://arxiv.org/abs/1703.05192)
1. [DualGAN](https://arxiv.org/abs/1704.02510)

#### Face Editing
1. [Fader Networks](https://arxiv.org/abs/1706.00409)
1. [Learning Residual Images for Face Attribute Manipulation](https://arxiv.org/abs/1612.05363)
1. [GeneGAN](https://arxiv.org/abs/1705.04932) - Object transfiguration 
1. [Convolutional Network for Attribute-driven and Identity-preserving Human Face Generation](https://arxiv.org/abs/1608.06434)
1. [DIAT](https://arxiv.org/abs/1610.05586)
1. [IcGAN](https://arxiv.org/abs/1611.06355)
1. [Age-cGAN](https://arxiv.org/abs/1702.01983)
1. [VAE/GAN](https://arxiv.org/abs/1512.09300) - Visual attribute vectors
1. [UNIT](arxiv.org/abs/1703.00848)
1. [IAN](https://arxiv.org/abs/1609.07093)

#### Face Frontalization/Profiling
1. [TP-GAN](https://arxiv.org/abs/1704.04086)
1. [DR-GAN](http://cvlab.cse.msu.edu/pdfs/Tran_Yin_Liu_CVPR2017.pdf)



