1. Use leaky relu in down-sampling and relu in up-sampling 
    - https://arxiv.org/abs/1703.05192

2. Use L1 distance instead of L2 in image reconstruction since L2 often leads blurriness
    - (https://arxiv.org/abs/1704.02510)
    - (https://arxiv.org/abs/1703.10593)
    - [pix2pix](https://arxiv.org/abs/1611.07004)

3. Network architectures
    - 

4. Use Layer Normalization or Instance Normalization in D and Batch Normalization in G when using WGAN-GP