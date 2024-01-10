# E<sup>2</sup>GAN: Efficient Training of Efficient GANs for Image-to-Image Translation

[Yifan Gong](https://yifanfanfanfan.github.io/)<sup>1,2</sup>, [Zheng Zhan](https://zhanzheng8585.github.io/)<sup>2</sup>, [Qing Jin](https://research.snap.com/team/team-member.html#qing-jin)<sup>1</sup>, [Yanyu Li](https://scholar.google.com/citations?user=XUj8koUAAAAJ&hl=en)<sup>1,2</sup>, [Yerlan Idelbayev](https://www.linkedin.com/in/yerlan-idelbayev/)<sup>1</sup>, [Xian Liu](https://alvinliu0.github.io/")<sup>1</sup>, [Andrey Zharkov](https://www.linkedin.com/in/asmekal/)<sup>1</sup>, [Kfir Aberman](https://kfiraberman.github.io/)<sup>1</sup>, [Sergey Tulyakov](http://www.stulyakov.com/)<sup>1</sup>, [Yanzhi Wang](https://web.northeastern.edu/yanzhiwang/)<sup>2</sup>, [Jian Ren](https://alanspike.github.io/)<sup>1</sup>.  
<sup>1</sup>Snap Inc.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<sup>2</sup>Northeastern University&nbsp;&nbsp;&nbsp;&nbsp;  

### [Project](https://github.com/Yifanfanfanfan/Yifanfanfanfan.github.io/tree/main/e2gan) | [Paper](https://snap-research.github.io/HyperHuman/content/hyperhuman.pdf) | [arXiv](https://arxiv.org/abs/2310.08579) | [Demo](https://www.youtube.com/watch?v=uGFWVT_qm9Q)

One highly promising direction for enabling flexible real-time on-device image editing is utilizing data distillation by leveraging large-scale text-to-image diffusion models, such as Stable Diffusion, to generate paired datasets used for training generative adversarial networks (GANs). This approach notably alleviates the stringent requirements typically imposed by high-end commercial GPUs for performing image editing with diffusion models. However, unlike text-to-image diffusion models, each distilled GAN is specialized for a specific image editing task, necessitating costly training efforts to obtain models for various concepts. In this work, we introduce and address a novel research direction: can the process of distilling GANs from diffusion models be made significantly more efficient? To achieve this goal, we propose a series of innovative techniques. First, we construct a base GAN model with generalized features, adaptable to different concepts through fine-tuning, eliminating the need for training from scratch. Second, we identify crucial layers within the base GAN model and employ Low-Rank Adaptation (LoRA) with a simple yet effective rank search process, rather than fine-tuning the entire base model. Third, we investigate the minimal amount of data necessary for fine-tuning, further reducing the overall training time. Extensive experiments show that we can efficiently empower GANs with the ability to perform real-time high-quality image editing on mobile devices with remarkable reduced training cost and storage for each concept.

<img src='./static/images/motivation.jpg' width=800>

## Citation

If you find our work useful, please kindly cite as:
```
@article{gong2024e2gan,
  title   = {E2GAN: Efficient Training of Efficient GANs for Image-to-Image Translation},
  author  = {Gong, Yifan and Zhan, Zheng and Jin, Qing and Li, Yanyu and Idelbayev, Yerlan and Liu, Xian and Zharkov, Andrey and Aberman, Kfir and Tulyakov, Sergey and Wang, Yanzhi and Ren, Jian},
  journal = {arXiv preprint arXiv:2304.14404},
  year    = {2024}
}
```
