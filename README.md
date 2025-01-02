## Pixel-level and Semantic-level Adjustable Super-resolution: A Dual-LoRA Approach


<a href='https://arxiv.org/pdf/2412.03017'><img src='https://img.shields.io/badge/Paper-Arxiv-red'></a>

[Lingchen Sun](https://scholar.google.com/citations?hl=zh-CN&tzom=-480&user=ZCDjTn8AAAAJ)<sup>1,2</sup>
| [Rongyuan Wu](https://scholar.google.com/citations?user=A-U8zE8AAAAJ&hl=zh-CN)<sup>1,2</sup> | 
[Zhiyuan Ma](https://scholar.google.com/citations?user=F15mLDYAAAAJ&hl=en)<sup>1</sup> | 
[Shuaizheng Liu](https://scholar.google.com/citations?user=wzdCc-QAAAAJ&hl=en)<sup>1,2</sup> | 
[Qiaosi Yi](https://dblp.org/pid/249/8335.html)<sup>1,2</sup> |
[Lei Zhang](https://www4.comp.polyu.edu.hk/~cslzhang)<sup>1,2</sup>

<sup>1</sup>The Hong Kong Polytechnic University, <sup>2</sup>OPPO Research Institute



## ⏰ Update
- **2025.1.2**: The code and model are released
- **2024.12.4**: The paper and this repo are released.

:star: If PiSA-SR is helpful to your images or projects, please help star this repo. Thanks! :hugs:

## 🌟 Overview Framework

![PiSA-SR](figs/framework.png)


(a) Training procedure of PiSA-SR. During the training process, two LoRA modules are respectively optimized for pixel-level and semantic-level enhancement.

(b) Inference procedure of PiSA-SR. During the inference stage, users can use the default setting to reconstruct the high-quality image in one-step diffusion or adjust λ<sub>pix</sub> and λ<sub>sem</sub> to control the strengths of pixel-level and semantic-level enhancement.
## 😍 Visual Results
### Adjustable SR Results
<div align="center">
<img src="figs/fig1_github.png" alt="PiSA-SR" width="800">
</div>

By increasing the guidance scale λ<sub>pix</sub> on the pixel-level LoRA module, the image degradations such as noise and compression artifacts can be gradually removed; however, a too-strong λ<sub>pix</sub> will make the SR image over-smoothed. By increasing the guidance scale λ<sub>sem</sub> on the semantic-level LoRA module, the SR images will have more semantic details; nonetheless, a too-high λ<sub>sem</sub> will generate visual artifacts.

### Comparisons with Other DM-Based SR Methods
![PiSA-SR](figs/comparison.png)

### Citations
If our code helps your research or work, please consider citing our paper.
The following are BibTeX references:

```
@article{sun2024pisasr,
  title={Pixel-level and Semantic-level Adjustable Super-resolution: A Dual-LoRA Approach},
  author={Sun, Lingchen and Wu, Rongyuan and Ma, Zhiyuan and Liu, Shuaizheng and Yi, Qiaosi and Zhang, Lei},
  journal={arXiv preprint arXiv:2412.03017},
  year={2024}
}
```

### License
This project is released under the [Apache 2.0 license](LICENSE).

### Acknowledgement

### Contact
If you have any questions, please contact: ling-chen.sun@connect.polyu.hk


<details>
<summary>statistics</summary>

![visitors](https://visitor-badge.laobi.icu/badge?page_id=csslc/PiSA-SR)

</details>