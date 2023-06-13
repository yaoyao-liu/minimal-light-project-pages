---
layout: project
---

## Abstract

Class-incremental learning (CIL) aims to train a classification model while the number of classes increases phase-by-phase. An inherent challenge of CIL is the stability-plasticity tradeoff, i.e., CIL models should keep stable to retain old knowledge and keep plastic to absorb new knowledge. However, none of the existing CIL models can achieve the optimal tradeoff in different data-receiving settings—where typically the training-from-half (TFH) setting needs more stability, but the training-from-scratch (TFS) needs more plasticity. To this end, we design an online learning method that can adaptively optimize the tradeoff without knowing the setting as a priori. Specifically, we first introduce the key hyperparameters that influence the tradeoff, e.g., knowledge distillation (KD) loss weights, learning rates, and classifier types. Then, we formulate the hyperparameter optimization process as an online Markov Decision Process (MDP) problem and propose a specific algorithm to solve it. We apply local estimated rewards and a classic bandit algorithm Exp3 (Auer et al. 2002) to address the issues when applying online MDP methods to the CIL protocol. Our method consistently improves top-performing CIL methods in both TFH and TFS settings, e.g., boosting the average accuracy of TFH and TFS by 2.2 percentage points on ImageNet-Full, compared to the state-of-the-art (Liu et al. 2021b).


## Video

<center>
  <iframe height="540" width="960" style="max-width:100%;max-height:100%;" src="https://class-il.mpi-inf.mpg.de/online/files/video.mp4" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</center>
<br>

## Citation

Please cite our paper if it is helpful to your work:
```bibtex
@inproceedings{Liu2023Online,
  author       = {Liu, Yaoyao and
                  Li, Yingying and
                  Schiele, Bernt and
                  Sun, Qianru},
  title        = {Online Hyperparameter Optimization for Class-Incremental Learning},
  booktitle    = {Thirty-Seventh {AAAI} Conference on Artificial Intelligence},
  year         = {2023}
}
```


## Contact

If you have any questions, please feel free to contact us via email: <yliu538@jhu.edu>.
