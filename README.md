# HyperAlign: Hypernetwork for Efficient Test-Time Alignment of Diffusion Models
[Xin Xie<sup>1</sup>](https://shelsin.github.io/), [Jiaxian Guo<sup>2</sup>](https://cr-gjx.github.io/), [Dong Gong<sup>1 †</sup>](https://donggong1.github.io/)

<sup>1</sup>University of New South Wales (UNSW Sydney), <sup>2</sup>Google Research

This is the official implementation of HyperAlign, introduced in [HyperAlign: Hypernetwork for Efficient Test-Time Alignment of Diffusion Models](https://arxiv.org/abs/2601.15968).

## TODO
- [x] Release the training and inference code of HyperAlign. (Coming soon/Almost there🤓)

## Abstract
<p>
Diffusion model alignment aims to bridge the gap between generated outputs and human preferences by enhancing both semantic consistency with textual prompts and overall visual quality. Existing alignment methods face a challenging trade-off: test-time approaches enable input-specific adaptability but introduce significant computational overhead and tend to under-optimize, while fine-tuning approaches risk reward over-optimization and loss of generation diversity.
</p>
<p>
To bridge this gap, we propose HyperAlign, a framework that trains a hypernetwork for efficient and effective test-time alignment. Instead of modifying latent states directly, HyperAlign dynamically generates input-and-state-conditioned low-rank adaptation weights to modulate the denoising trajectory toward target rewards. We introduce multiple HyperAlign variants of varying granularity to balance alignment quality and computational efficiency. The hypernetwork is optimized with a reward objective regularized by preference data to mitigate reward hacking.
</p>
<p>
We evaluate HyperAlign across multiple generative paradigms, including Stable Diffusion and FLUX, where it significantly outperforms existing alignment methods in semantic consistency and visual quality.
</p>


## Method Overview
![method_overview](assets/method.png)
