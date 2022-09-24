# README
This repository is the official implementation of "MAtt: A Manifold Attention Network for EEG Decoding, NeurIPS 2022". 

MAtt is a novel manifold attention network applied in decoding complex EEG signals. Proposed MAtt executes the forward procedure on both Euclidean space and SPD manifold, but backpropagates the network on Stiefel manifold. For more details for MAtt, please refer to our work: 'MAtt: A Manifold Attention Network for EEG Decoding, NeurIPS 2022'.

## Requirements
#### Step1:
To install requirements:
```setup
conda env create -f /path/to/mAtt_env.yml
conda activate mAtt_env
```
#### Step2:
Download datasets and unzip them to the folder "code_2022".

## Dataset
1. BCICIV2a:
    https://www.bbci.de/competition/iv/
2. MAMEM SSVEP:
   https://www.mamem.eu/results/datasets/
3. BCI challenge:
    https://www.kaggle.com/competitions/inria-bci-challenge/data

<!-- Link to download [data](https://drive.google.com/file/d/1_KBfSNzvxCZ-HwiOASQhlFe8wwsq4vHt/view?usp=sharing) -->

## Training and testing

To train and test the mAtt in the paper, run this command:

```train and test
python mAtt_<which_dataset>.py
```
All default hyperparameters are already set in files. 'which_dataset' can be chosen as 'bci', 'mamem', or 'bcicha'.



## Reference
- MAtt: A Manifold Attention Network for EEG Decoding, NeurIPS 2022.

```bash
@misc{spdnet2020,
  author={adavoudi},
  title={spdnet},
  year={2020},
  url={https://github.com/adavoudi/spdnet},
}
```

```bash
@inproceedings{wei2019spatial,
  title={Spatial component-wise convolutional network (SCCNet) for motor-imagery EEG classification},
  author={Wei, Chun-Shu and Koike-Akino, Toshiaki and Wang, Ye},
  booktitle={2019 9th International IEEE/EMBS Conference on Neural Engineering (NER)},
  pages={328--331},
  year={2019},
  organization={IEEE}
}
```

```bash
@article{brunner2008bci,
  title={{BCI Competition 2008--Graz data set A}},
  author={Brunner, Clemens and Leeb, Robert and M{\"u}ller-Putz, Gernot and Schl{\"o}gl, Alois and Pfurtscheller, Gert},
  journal={Institute for Knowledge Discovery (Laboratory of Brain-Computer Interfaces), Graz University of Technology},
  volume={16},
  pages={1--6},
  year={2008}
}
```


```bash
@article{Nikolopoulos2021,
author = "Spiros Nikolopoulos",
title = "{MAMEM EEG SSVEP Dataset II (256 channels, 11 subjects, 5 frequencies presented simultaneously)}",
year = "2021",
month = "5",
url = "https://figshare.com/articles/dataset/MAMEM_EEG_SSVEP_Dataset_II_256_channels_11_subjects_5_frequencies_presented_simultaneously_/3153409",
doi = "10.6084/m9.figshare.3153409.v4"
}

```

```bash
@article{margaux2012objective,
  title={{Objective and subjective evaluation of online error correction during P300-based spelling}},
  author={Margaux, Perrin and Emmanuel, Maby and S{\'e}bastien, Daligault and Olivier, Bertrand and J{\'e}r{\'e}mie, Mattout},
  journal={Advances in Human-Computer Interaction},
  volume={2012},
  year={2012},
  publisher={Hindawi}
}
```







