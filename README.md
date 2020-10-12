# Steam StyleGAN2-ADA

The goal of this [Colab][colab-website] notebook is to capture the distribution of Steam banners with a StyleGAN2-ADA model.

## Usage

-   Acquire the data, e.g. as a snapshot called `256x256.zip` in [my data repository][data-repository],
-   Run [`StyleGAN2-ADA_training.ipynb`][colab-notebook] to train a StyleGAN2-ADA model from scratch.
[![Open In Colab][colab-badge]][colab-notebook]

## Data

The dataset consists of 14,176 Steam banners with RGB channels and resized from 300x450 to 256x256 resolution.

Images were downloaded with [`download_steam_banners.ipynb`][download_steam_banners].
[![Open In Colab][colab-badge]][download_steam_banners]

Images were then filtered (duplicates, outliers, etc.) with [`remove_duplicates.ipynb`][filter_steam_banners].
[![Open In Colab][colab-badge]][filter_steam_banners]

## References

-   DCGAN:
    -   [Radford, Alec, et al. *Unsupervised Representation learning with Deep Convolutional GAN*. ICLR 2016.][dcgan-paper]
    -   [Official implementation][dcgan-official-repository]
    -   [Application to Steam banners][dcgan-applied-to-steam-banners]
-   StyleGAN:
    -   [Karras, Tero, et al. *A Style-Based Generator Architecture for Generative Adversarial Networks*. CVPR 2019.][stylegan1-paper]
    -   [Official implementation][stylegan1-official-repository]
    -   [Application to Steam banners][stylegan1-applied-to-steam-banners]
-   StyleGAN2:
    - [Karras, Tero, et al. *Analyzing and Improving the Image Quality of StyleGAN*. CVPR 2020.][stylegan2-paper]
    -   [Official implementation][stylegan2-official-repository]
    -   [Application to Steam banners][stylegan2-applied-to-steam-banners]
-   StyleGAN2-ADA:
    -   [Karras, Tero, et al. *Training generative adversarial networks with limited data*. arXiv 2020.][stylegan2-ada-paper]
    -   [Official implementation][stylegan2-ada-official-repository]
    -   [Application to Steam banners][stylegan2-ada-applied-to-steam-banners]

<!-- Definitions -->

[download_steam_banners]: <https://colab.research.google.com/github/woctezuma/google-colab/blob/master/download_steam_banners.ipynb>
[filter_steam_banners]: <https://colab.research.google.com/github/woctezuma/steam-stylegan2-ada/blob/main/remove_duplicates.ipynb>

[colab-website]: <https://colab.research.google.com>
[colab-notebook]: <https://colab.research.google.com/github/woctezuma/steam-stylegan2-ada/blob/main/StyleGAN2-ADA_training.ipynb>
[colab-badge]: <https://colab.research.google.com/assets/colab-badge.svg>

[data-repository]: <https://github.com/woctezuma/download-steam-banners-data>

[dcgan-paper]: <https://arxiv.org/abs/1511.06434>
[stylegan1-paper]: <https://arxiv.org/abs/1812.04948>
[stylegan2-paper]: <https://arxiv.org/abs/1912.04958>
[stylegan2-ada-paper]: <https://arxiv.org/abs/2006.06676>

[dcgan-official-repository]: <https://github.com/Newmu/dcgan_code>
[stylegan1-official-repository]: <https://github.com/NVlabs/stylegan>
[stylegan2-official-repository]: <https://github.com/NVlabs/stylegan2>
[stylegan2-ada-official-repository]: <https://github.com/NVlabs/stylegan2-ada>

[dcgan-applied-to-steam-banners]: <https://github.com/woctezuma/google-colab>
[stylegan1-applied-to-steam-banners]: <https://github.com/woctezuma/steam-stylegan>
[stylegan2-applied-to-steam-banners]: <https://github.com/woctezuma/steam-stylegan2>
[stylegan2-ada-applied-to-steam-banners]: <https://github.com/woctezuma/steam-stylegan2-ada>
