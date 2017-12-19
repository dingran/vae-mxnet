# Variational autoencoders in MXNet/Gluon

Implementations of variational autoencoders using MXNet/Gluon.

### References:

1. Kingma, Diederik P., and Max Welling.
["Auto-encoding variational bayes."](https://arxiv.org/abs/1312.6114)
arXiv preprint arXiv:1312.6114 (2013).
2. Rezende, Danilo Jimenez, Shakir Mohamed, and Daan Wierstra.
["Stochastic backpropagation and approximate inference in deep generative models."](https://arxiv.org/abs/1401.4082)
 arXiv preprint arXiv:1401.4082 (2014).

### Code:

- Implementation using MXNet API (i.e. mxnet.sym, mxnet.mod) [vae-mxnet.ipynb](code/vae-mxnet.ipynb)
- Implementation using Gluon API (i.e. gluon.HybridBlock, autograd) [vae-gluon.ipynb](code/vae-gluon.ipynb)
- CNN-based version, implemented using Gluon [vaecnn-gluon.ipynb](code/vaecnn-gluon.ipynb)

### Results:

- Generated MNIST figures by randomly sampling learned latent space

With 2-D latent space | With 10-D latent space | With 20-D latent space
--- | --- | ---
![](code/generated_samples_with_2D_latent_space.png) | ![](code/generated_samples_with_10D_latent_space.png) |![](code/generated_samples_with_20D_latent_space.png)

- Learned 2-D manifold

Latent feature Z corresponding to 1000 test images | Generated images from grid scan in Z | 
--- | ---
![](code/2d_latent_space_for_test_samples.png) | ![](code/2d_latent_space_scan_for_generation.png)






