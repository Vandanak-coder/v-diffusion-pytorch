# v-diffusion-pytorch

v objective diffusion inference code for PyTorch, by Vandana Kattamreddy

The models are denoising diffusion probabilistic models (https://arxiv.org/abs/2006.11239), which are trained to reverse a gradual noising process, allowing the models to generate samples from the learned data distributions starting from random noise. The models are also trained on continuous timesteps. They use the 'v' objective from Progressive Distillation for Fast Sampling of Diffusion Models (https://openreview.net/forum?id=TIdIXIpzhoI). Guided diffusion sampling scripts (https://arxiv.org/abs/2105.05233) are included, specifically CLIP guided diffusion. This repo also includes a diffusion model conditioned on CLIP text embeddings that supports classifier-free guidance (https://openreview.net/pdf?id=qw8AKxfYbI), similar to GLIDE (https://arxiv.org/abs/2112.10741). Sampling methods include DDPM, DDIM (https://arxiv.org/abs/2010.02502), and PRK/PLMS (https://openreview.net/forum?id=PlKWVd2yBkY).

Thank you to [stability.ai](https://www.stability.ai) for compute to train these models!

## Installation

`pip install v-diffusion-pytorch`

or git clone then `pip install -e .`


### Colab

There is a cc12m_1_cfg Colab (a simplified version of `cfg_sample.py`) [here](https://colab.research.google.com/drive/1KSSufk7j7CrWpEHoTMOjBvW6DkiNmRFm), which can be used for free.


0, can lower for faster but lower quality sampling)
