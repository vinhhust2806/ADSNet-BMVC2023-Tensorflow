# ADSNet: Adaptation of Distinct Semantic for Uncertain Areas in Polyp Segmentation, BMVC 2023 

Official Tensorflow implementation of [ADSNet: Adaptation of Distinct Semantic for Uncertain Areas in Polyp Segmentation](https://arxiv.org/pdf/2405.07523) BMVC 2023. 
 <br>

In The 34th British Machine Vision Conference, 20th - 24th November 2023, Aberdeen, UK.

## Architecture

<p align="center">
<img src="architecture.png" width=75% height=40% 
class="center">
</p>

## 1. Usage:
### Recommended environment:
Please use ```pip install -r requirements.txt``` to install the libraries.

### Data preparation:
Download the training and testing datasets [Google Drive](https://drive.google.com/file/d/1pFxb9NbM8mj_rlSawTlcXG1OdVGAbRQC/view?usp=sharing) and move them into 'polyp/' folder.

### Training:
Run ```python train.py --epoch 200 --batch_sise 16 --lr 1e-4 --min_lr 1e-8 --val_name kvasir```

### Testing:
Run ```python test.py --pretrain_path weight.hdf5 --test_name kvasir```

### 2. Polyp Segmentation Compared Results:
We also provide some result of baseline methods, You could download from [Google Drive](https://drive.google.com/file/d/1xvjRl70pZbOO6wI5p94CSpZK2RAUnUnx/view?usp=sharing), including results of compared models.

## 3. Citation
If you have found our work useful, please use the following reference to cite this project:
```
@article{nguyen2024adaptation,
  title={Adaptation of Distinct Semantics for Uncertain Areas in Polyp Segmentation},
  author={Nguyen, Quang Vinh and Huynh, Van Thong and Kim, Soo-Hyung},
  journal={arXiv preprint arXiv:2405.07523},
  year={2024}
}

@inproceedings{Nguyen_2023_BMVC,
author    = {Quang Vinh Nguyen and Van Thong Huynh and Soo-Hyung Kim},
title     = {Adaptation of Distinct Semantics for Uncertain Areas in Polyp Segmentation},
booktitle = {34th British Machine Vision Conference 2023, {BMVC} 2023, Aberdeen, UK, November 20-24, 2023},
publisher = {BMVA},
year      = {2023},
url       = {https://papers.bmvc2023.org/0806.pdf}
}
```
