This is a modded version of StyleGAN2 with differential augmentation and other parameter changes. Project done for class on Deep Generative Models at UC San Diego.

Disclaimer: didn't edit code that much, just implemented two time-scale update rule (TTUR) and exploited batch size to maximum VRAM usage. Also intergrated Differentiable Augmentation.

Requires tensorflow-gpu==1.15.0

To excecute training unzip ./datasets/Monet.7z (had to use .7z filetype for gradescope to upload)
Then, run this line on terminal:
run_low_shot.py --dataset=./datasets/Monet --resolution=128 --num-gpus=1 --total-kimg=300 --batch-size=24

Credits:
@inproceedings{zhao2020diffaugment,
  title={Differentiable Augmentation for Data-Efficient GAN Training},
  author={Zhao, Shengyu and Liu, Zhijian and Lin, Ji and Zhu, Jun-Yan and Han, Song},
  booktitle={Conference on Neural Information Processing Systems (NeurIPS)},
  year={2020}
}

@inproceedings{Karras2019stylegan2,
  title     = {Analyzing and Improving the Image Quality of {StyleGAN}},
  author    = {Tero Karras and Samuli Laine and Miika Aittala and Janne Hellsten and Jaakko Lehtinen and Timo Aila},
  booktitle = {Proc. CVPR},
  year      = {2020}
}

