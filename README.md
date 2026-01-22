# HyperAlign: Hypernetwork for Efficient Test-Time Alignment of Diffusion Models
[Xin Xie](https://shelsin.github.io/), [Jiaxian Guo](https://cr-gjx.github.io/), [Dong Gong](https://donggong1.github.io/)

This is the official implementation of HyperAlign, introduced in [HyperAlign: Hypernetwork for Efficient Test-Time Alignment of Diffusion Models](https://arxiv.org/abs/xxxx.xxxxx).

## TODO
- [x] Release the inference code of HyperAlign (Coming soon/Almost there🤓).


## Abstract
<p>
Diffusion models achieve state-of-the-art performance but often fail to generate outputs that align with human preferences and intentions, resulting in images with poor aesthetic quality and semantic inconsistencies. Existing alignment methods present a difficult trade-off: fine-tuning approaches suffer from loss of diversity with reward over-optimization, while test-time scaling methods introduce significant computational overhead and tend to under-optimize.
</p>
<p>
To address these limitations, we propose HyperAlign, a novel framework that trains a hypernetwork for efficient and effective test-time alignment. Instead of modifying latent states, HyperAlign dynamically generates low-rank adaptation weights to modulate the diffusion model's generation operators. This allows the denoising trajectory to be adaptively adjusted based on input latents, timesteps and prompts for reward-conditioned alignment. We introduce multiple variants of HyperAlign that differ in how frequently the hypernetwork is applied, balancing between performance and efficiency. Furthermore, we optimize the hypernetwork using a reward score objective regularized with preference data to reduce reward hacking.
</p>
<p>
We evaluate HyperAlign on multiple extended generative paradigms, including Stable Diffusion and FLUX. It significantly outperforms existing fine-tuning and test-time scaling baselines in enhancing semantic consistency and visual appeal.
</p>


## Method Overview
![method_overview](assets/method.png)
