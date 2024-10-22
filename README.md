# SpotDiffusion (WACV 2025)
Official Pytorch Implementation for "SpotDiffusion: A Fast Approach For Seamless Panorama Generation Over Time"

[![arXiv](https://img.shields.io/badge/Link_to-Project_Page-blue)](https://spotdiffusion.github.io) 
[![arXiv](https://img.shields.io/badge/arXiv_Paper-SpotDiffusion-b31b1b.svg)](https://arxiv.org/abs/2407.15507)

[//]: # (### Abstract)
>Generating high-resolution images with generative models has recently been made widely accessible by leveraging diffusion models pre-trained on large-scale datasets. Various techniques, such as MultiDiffusion and SyncDiffusion, have further pushed image generation beyond training resolutions, i.e., from square images to panorama, by merging multiple overlapping diffusion paths or employing gradient descent to maintain perceptual coherence. However, these methods suffer from significant computational inefficiencies due to generating and averaging numerous predictions, which is required in practice to produce high-quality and seamless images. This work addresses this limitation and presents a novel approach that eliminates the need to generate and average numerous overlapping denoising predictions. Our method shifts non-overlapping denoising windows over time, ensuring that seams in one timestep are corrected in the next. This results in coherent, high-resolution images with fewer overall steps. We demonstrate the effectiveness of our approach through qualitative and quantitative evaluations, comparing it with MultiDiffusion, SyncDiffusion, and StitchDiffusion. Our method offers several key benefits, including improved computational efficiency and faster inference times while producing comparable or better image quality.

# Run
```
git clone https://github.com/stanifrolov/spotdiffusion.git
pip install -r requirements.txt
python panorama.py
```

# Citation
If you find our work useful in your research, please consider citing:

```bibtex
@article{frolov2024spotdiffusion,
  title={SpotDiffusion: A Fast Approach For Seamless Panorama Generation Over Time},
  author={Frolov, Stanislav and Moser, Brian B and Dengel, Andreas},
  journal={arXiv preprint arXiv:2407.15507},
  year={2024}
}
```

# Acknowledgements
This code is based on the official implementation of [MultiDiffusion](https://github.com/omerbt/MultiDiffusion/).
Thanks to the authors for releasing their codebase.
