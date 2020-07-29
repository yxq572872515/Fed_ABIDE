# PyTorch implementation of Multi-site fMRI Analysis Using Privacy-preserving Federated Learning and Domain Adaptation: ABIDE Results
Our manuscript is available on arxiv https://arxiv.org/pdf/2001.05647.pdf and will be coming soon on Medical Image Analysis.

## Dependencies
- Python 3.6
- Pytorch 1.1.0
- tensorboardX

## Data
### Data Download
[ ] TBD
### Data Preprocessing
[ ] TBD

## How to run ?
Here we show a few examples using different strategies listed in the paper. Please check the meaning of configurations in each script.
### Single 
```
python single.py --split ${SPLIT} --site ${SITE}
```
### Ensemble
```
python ensemble.py --split ${SPLIT} --site ${SITE}
```
### Cross
```
python cross.py --trainsite ${TRAINSITE}
```
### MIX
```
python mix.py --split ${SPLIT}
```
### Vanilla Fed
#### vary on noise
```
python federated.py --split ${SPLIT} --noise ${NOISE} --type ${TYPE}
```
#### vary on pace
```
python federated.py --split ${SPLIT} --pace ${PACE}
```
### Fed + MOE
```
python federated_MoE.py --split ${SPLIT}
```
### Fed + Align
```
python federated_align.py --split ${SPLIT}
```

## Reference
[1]Li, X., Gu, Y., Dvornek, N., Staib, L., Ventola, P. and Duncan, J.S., 2020. Multi-site fmri analysis using privacy-preserving federated learning and domain adaptation: Abide results. arXiv preprint arXiv:2001.05647.

Please cite our paper if you find this repository useful:
```
@article{li2020multi,
  title={Multi-site fmri analysis using privacy-preserving federated learning and domain adaptation: Abide results},
  author={Li, Xiaoxiao and Gu, Yufeng and Dvornek, Nicha and Staib, Lawrence and Ventola, Pamela and Duncan, James S},
  journal={Medical Image Analysis},
  year={2020}
}
```




