This is a modded version of StyleGAN2 with differential augmentation and other parameter changes. Project done for class on Deep Generative Models at UC San Diego.

Disclaimer: I only made minor edits to this, just implemented two time-scale update rule (TTUR) and exploited batch size to maximum VRAM usage.

Requires tensorflow-gpu==1.15.0

To excecute training unzip ./datasets/Monet.7z (had to use .7z filetype for gradescope to upload)
Then, run this line on terminal:
run_low_shot.py --dataset=./datasets/Monet --resolution=128 --num-gpus=1 --total-kimg=300 --batch-size=24

Differentiable Augmentation paper: https://arxiv.org/pdf/2006.10738.pdf

Differentiable Augmentation code: https://github.com/mit-han-lab/data-efficient-gans/tree/master/DiffAugment-stylegan2

StyleGAN2 paper: https://arxiv.org/pdf/1912.04958.pdf

Two Time-scale Update Rule paper: https://arxiv.org/pdf/1706.08500v6.pdf

Source of Monet dataset: https://www.kaggle.com/c/gan-getting-started
