### Divergence, Objective Function
1. [GAN](https://papers.nips.cc/paper/5423-generative-adversarial-nets.pdf), [DCGAN](https://arxiv.org/abs/1511.06434) - KL divergence
2. [WGAN](https://arxiv.org/abs/1701.07875) - Wasserstein distance
    - [WGAN-GP](https://arxiv.org/abs/1704.00028) - Gradient penalty
3. [EBGAN](https://arxiv.org/abs/1609.03126) - D(x) = ||Dec(Enc(x)) − x||
4. [Least Square GAN](https://pdfs.semanticscholar.org/0bbc/35bdbd643fb520ce349bdd486ef2c490f1fc.pdf) - Pearson χ2 divergence
5. [BEGAN](https://arxiv.org/abs/1703.10717) - Wasserstein distance between the distribution of real/fake auto-encoder loss

### Evaluations of GANs
1. [Improved GAN](https://arxiv.org/abs/1606.03498) - Inception score