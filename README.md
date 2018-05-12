***Recommendation***

- Our GAN based work for facial attribute editing - https://github.com/LynnHo/AttGAN-Tensorflow.

---

---
### Frameworks
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434)
1. [cGAN](https://arxiv.org/abs/1411.1784) - Label-conditioning generation
1. [AcGAN](https://arxiv.org/abs/1610.09585) - Supervised generation (auxiliary classifier with labels)
1. [SGAN](https://arxiv.org/abs/1606.01583) - D outputs [CLASS-1, CLASS-2, . . . CLASS-N, FAKE]
1. [InfoGAN](https://arxiv.org/abs/1606.03657) - Unsupervised lantern space disentangling
1. [ALI](https://arxiv.org/abs/1606.00704), [BiGAN](https://arxiv.org/abs/1605.09782) - match p(G(z),z) and q(x,E(x))
1. [GMAN](https://arxiv.org/abs/1611.01673) - Multiple discriminator models <!-- TODO -->
1. [AdaGAN](https://arxiv.org/abs/1701.02386) - Multiple generative models <!-- TODO -->
1. [MGGAN](http://arxiv.org/abs/1708.02556) - Multiple generative models <!-- TODO -->


---
### High Resolution
1. [LAPGAN](http://papers.nips.cc/paper/5773-deep-generative-image-models-using-a-laplacian-pyramid-of-adversarial-networks.pdf) - Coarse-to-fine generation
1. [StackGAN](https://arxiv.org/abs/1612.03242) - Two-step generation
1. [PGGAN](http://arxiv.org/abs/1710.10196)


---
### Function ('~' means 'match')

#### g(Z) ~ X
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434)

#### g(Z|Y) ~ X|Y, where Y is label or lantern variable
1. [cGAN](https://arxiv.org/abs/1411.1784)
1. [AcGAN](https://arxiv.org/abs/1610.09585)
1. [InfoGAN](https://arxiv.org/abs/1606.03657)
1. [CFGAN](http://openaccess.thecvf.com/content_cvpr_2017/html/Kaneko_Generative_Attribute_Controller_CVPR_2017_paper.html)

#### g(Z),Z ~ X,E(X)
1. [ALI](https://arxiv.org/abs/1606.00704), [BiGAN](https://arxiv.org/abs/1605.09782)


---
### Objective Function

#### f-Divergence
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434) - JS divergence
1. [LSGAN (Least Squares GAN)](https://pdfs.semanticscholar.org/0bbc/35bdbd643fb520ce349bdd486ef2c490f1fc.pdf) - Pearson χ2 divergence
1. [f-GAN](https://arxiv.org/abs/1606.00709) - Variational divergence minimization
1. [f-GANs](https://arxiv.org/abs/1707.04385)

#### Integral Probability Metrics (IPM)
1. [WGAN](https://arxiv.org/abs/1701.07875) - Wasserstein distance
    - [WGAN-GP](https://arxiv.org/abs/1704.00028) - Gradient penalty, less capacity compromise
1. [McGAN](https://arxiv.org/abs/1702.08398) - Mean and covariance matching
1. [Geometric GAN](https://arxiv.org/abs/1705.02894)
1. [Fisher GAN](https://arxiv.org/abs/1705.09675) - Chi-squared distance
##### Maximum Mean Discrepancy (MMD)
1. [GMMN](http://proceedings.mlr.press/v37/li15.pdf)
1. [MMD nets](https://arxiv.org/abs/1505.03906)

#### Others
1. [CatGAN](https://arxiv.org/abs/1511.06390) - Entropy of P(Y|X)
1. [EBGAN](https://arxiv.org/abs/1609.03126) - D(x) = ||Dec(Enc(x)) − x||
1. [LS-GAN (Loss-Sensitive GAN)](https://arxiv.org/abs/1701.06264)
1. [BEGAN](https://arxiv.org/abs/1703.10717) - Wasserstein distance between the distribution of real/fake auto-encoder loss
1. [AGE](https://arxiv.org/abs/1704.02304) - $max_emin_g\Delta(e(g(Z))||Y)-\Delta(e(X)||Y)$ and encoder-generator reciprocity (bidirectional mapping)
1. [Softmax GAN](https://arxiv.org/abs/1704.06191)
1. [Cramér GAN](https://arxiv.org/abs/1705.10743) - Cramér Distance
1. [LDGAN](https://arxiv.org/abs/1705.10743)


---
### Regularized GAN
1. [DRGAN](https://arxiv.org/abs/1705.07215) - Vanilla GAN with gradient penalty
1. [Cramér GAN](https://arxiv.org/abs/1705.10743) - Cramér Distance
1. [Regularized GAN](https://arxiv.org/abs/1705.09367)
1. [CT-GAN](http://arxiv.org/abs/1803.01541)
1. [Varying k-Lipschitz Constraint for Generative Adversarial Networks](http://arxiv.org/abs/1803.06107)


---
### Representation Learning

#### Lantern Space Disentangling
1. [InfoGAN](https://arxiv.org/abs/1606.03657) - Unsupervised lantern space disentangling
1. [AcGAN](https://arxiv.org/abs/1610.09585) - Supervised lantern space disentangling

#### Specifying Lantern Space Distribution
1. [AAE](https://arxiv.org/abs/1511.06390)
1. [ALI](https://arxiv.org/abs/1606.00704), [BiGAN](https://arxiv.org/abs/1605.09782) - Match p(G(z),z) and q(x,E(x)), simultaneously learn an encoder and decoder
1. [AGE](https://arxiv.org/abs/1704.02304)


---
### Semi-supervised Learning
1. [CatGAN](https://arxiv.org/abs/1511.06390)
1. [SGAN](https://arxiv.org/abs/1606.01583) - D outputs [CLASS-1, CLASS-2, . . . CLASS-N, FAKE]
1. [Improved GAN](https://arxiv.org/abs/1606.03498)
1. [Triple-GAN](https://arxiv.org/abs/1703.02291)
1. [CT-GAN](http://arxiv.org/abs/1803.01541)


---
### Evaluations of GANs <!-- TODO -->
1. [Inception Score - Improved GAN](https://arxiv.org/abs/1606.03498)
1. [FCN Score - pix2pix](https://arxiv.org/pdf/1611.07004.pdf)
1. [AMT Perceptual Studies - pix2pix](https://arxiv.org/pdf/1611.07004.pdf)
1. [Semantic Segmentation Metrics - CycleGAN](https://arxiv.org/abs/1703.10593)
1. [FID, Precision, Recall and F1 Score - Are GANs Created Equal? A Large-Scale Study](http://arxiv.org/abs/1711.10337)


---
### Applications

#### Data Augmentation
1. [Adversarial Generation of Training Examples for Vehicle License Plate Recognition](https://arxiv.org/abs/1707.03124)

#### Domain Adaptation
1. [Unsupervised Pixel-Level Domain Adaptation with Generative Adversarial Networks](https://arxiv.org/abs/1612.05424)
1. [DTN](https://arxiv.org/abs/1611.02200)
1. [UNIT](arxiv.org/abs/1703.00848)
1. [CoGAN](http://papers.nips.cc/paper/6544-coupled-generative-adversarial-networks)

#### Image Denoising
1. [Deep Semantic Face Deblurring](http://arxiv.org/abs/1803.03345)

#### Image-to-Image Translation
##### Unpaired
1. [CoGAN](http://papers.nips.cc/paper/6544-coupled-generative-adversarial-networks)
1. [DTN](https://arxiv.org/abs/1611.02200)
1. [CycleGAN](https://arxiv.org/abs/1703.10593), [DiscoGAN](https://arxiv.org/abs/1703.05192), [DualGAN](https://arxiv.org/abs/1704.02510)
1. [UNIT](https://arxiv.org/abs/1703.00848)
1. [Face Transfer with Generative Adversarial Network](http://arxiv.org/abs/1710.06090)
1. [XGAN](http://arxiv.org/abs/1711.05139) - Semantic consistency
##### Paired
1. [pix2pix/PatchGAN](https://arxiv.org/abs/1611.07004)
1. [Scribbler](https://arxiv.org/abs/1612.00835)
1. [PAN](https://arxiv.org/abs/1706.09138) - Perceptual adversarial loss
1. [Cross-View Image Synthesis using Conditional GANs](http://arxiv.org/abs/1710.06090)

#### Inpainting
1. [Context Encoder](http://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Pathak_Context_Encoders_Feature_CVPR_2016_paper.html)
1. [PAN](https://arxiv.org/abs/1706.09138)

#### Super-Resolution
1. [SRGAN](https://arxiv.org/abs/1609.04802)

#### Text-to-Image Synthesis
1. [GAN-INT-CLS](http://proceedings.mlr.press/v48/reed16.pdf) <!-- TODO -->
1. [GAWWN](http://papers.nips.cc/paper/6111-learning-what-and-where-to-draw) <!-- TODO -->
1. [StackGAN](https://arxiv.org/abs/1612.03242)

#### Face Editing
1. [VAE/GAN](https://arxiv.org/abs/1512.09300) - Visual attribute vectors
1. [IcGAN](https://arxiv.org/abs/1611.06355)
1. [DIAT](https://arxiv.org/abs/1610.05586)
1. [Learning Residual Images for Face Attribute Manipulation](https://arxiv.org/abs/1612.05363)
1. [DistanceGAN](https://arxiv.org/abs/1706.00826)
1. [CFGAN](http://openaccess.thecvf.com/content_cvpr_2017/html/Kaneko_Generative_Attribute_Controller_CVPR_2017_paper.html)
1. [Age-cGAN](https://arxiv.org/abs/1702.01983)
1. [UNIT](arxiv.org/abs/1703.00848)
1. [SL-GAN](https://arxiv.org/abs/1704.02166)
1. [IAN](https://arxiv.org/abs/1609.07093)
1. [Neural Face Editing with Intrinsic Image Disentangling](http://arxiv.org/abs/1704.04131)
1. [GeneGAN](https://arxiv.org/abs/1705.04932) - Object transfiguration
1. [Fader Networks](https://arxiv.org/abs/1706.00409)
1. [Unsupervised Visual Attribute Transfer with Reconfigurable Generative Adversarial Networks](http://arxiv.org/abs/1707.09798)
1. [ExprGAN](http://arxiv.org/abs/1709.03842)
1. [StarGAN](http://arxiv.org/abs/1711.09020)
1. [GLCA-GAN](http://arxiv.org/abs/1801.08390)

#### Face Frontalization/Profiling
1. [DR-GAN](http://cvlab.cse.msu.edu/pdfs/Tran_Yin_Liu_CVPR2017.pdf)
1. [TP-GAN](https://arxiv.org/abs/1704.04086)

#### Others
1. [iGAN](https://link.springer.com/chapter/10.1007/978-3-319-46454-1_36) - Image manipulation
1. [TVSN](https://arxiv.org/abs/1703.02921) - 3D view synthesis <!-- TODO -->
1. [ID-CGAN](https://arxiv.org/abs/1701.05957) - Image de-raining
1. [Perceptual GAN](https://arxiv.org/abs/1706.05274) - Small object detection


---
### Survey
1. [Generative Adversarial Networks: An Overview](http://arxiv.org/abs/1710.07035)
1. [How Generative Adversarial Nets and its variants Work](http://arxiv.org/abs/1711.05914)
1. [Comparative Study on Generative Adversarial Networks](http://arxiv.org/abs/1801.04271)
1. [An Introduction to Image Synthesis with Generative Adversarial Nets](http://arxiv.org/abs/1803.04469)


---
### Unclassified
1. [DeePSiM](http://arxiv.org/abs/1602.02644)
1. [Unrooled GAN](https://arxiv.org/abs/1611.02163)
1. [SGAN](http://arxiv.org/abs/1612.04357)
1. [AM-GAN](https://arxiv.org/abs/1703.02000)
1. [DeLiGAN](https://arxiv.org/abs/1706.02071) - Mixture Gaussian prior distribution
1. [TTUR](https://arxiv.org/abs/1706.08500)


---
### Datasets
1. [MNIST](https://pdfs.semanticscholar.org/eea7/573f64552685cdf8d144ec446c5fff1405fc.pdf)
1. [CIFAR10/CIFAR100](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.222.9220&rep=rep1&type=pdf)
1. [SVHN](https://research.google.com/pubs/pub37648.html)
1. [CelebA](http://openaccess.thecvf.com/content_iccv_2015/papers/Liu_Deep_Learning_Face_ICCV_2015_paper.pdf)