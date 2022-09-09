# Awesome Sound Source Localization
## Table of contents
- [Awesome Sound Source Localization](#awesome-sound-source-localization)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
  - [Publications](#publications)
    - [Survey](#survey)
    - [Databases](#databases)
    - [Network design](#network-design)
      - [MLP](#mlp)
      - [CNN](#cnn)
      - [RNN & LSTM & GRU](#rnn--lstm--gru)
      - [CRNN](#crnn)
      - [Attention](#attention)
      - [GAN](#gan)
    - [Phase reconstruction](#phase-reconstruction)
    - [Learning strategy](#learning-strategy)
      - [Loss function](#loss-function)
      - [Multi-task learning](#multi-task-learning)
      - [Semi-supervised](#semi-supervised)
    - [Other improvements](#other-improvements)
    - [SSL + Separation](#ssl--separation)
  - [Tools](#tools)
      - [Framework](#framework)
      - [Audio feature extraction](#audio-feature-extraction)
      - [Audio data augmentation](#audio-data-augmentation)
  - [Datasets](#datasets)
      - [Sound source localization datasets (in no particular order)](#sound-source-localization-datasets-in-no-particular-order)
      - [Augmentation noise sources (sorted by usage frequency in paper)](#augmentation-noise-sources-sorted-by-usage-frequency-in-paper)
  - [SOTA results](#sota-results)
      - [STOA results in dataset by University of Edinburgh. The following methods are all trained by "trainset_28spk" and tested by common testset. ("F" denotes frequency-domain and "T" is time-domain.)](#stoa-results-in-dataset-by-university-of-edinburgh-the-following-methods-are-all-trained-by-trainset_28spk-and-tested-by-common-testset-f-denotes-frequency-domain-and-t-is-time-domain)
  - [Learning materials](#learning-materials)
      - [Book or thesis](#book-or-thesis)
      - [Video](#video)
      - [Slides](#slides)

## Overview

This is a curated list of Awesome Sound Source Localization tutorials, papers, libraries, datasets, tools, scripts and results. The purpose of this repo is to organize the world’s resources for Sound Source Localization, and make them universally accessible and useful.

To add items to this page, simply send a pull request.

## Publications

### Survey
* A Survey of Sound Source Localization with Deep Learning Methods, 2021 [[paper]](https://arxiv.org/abs/2109.03465)

### Databases
* SLoClas: A Database for Joint Sound Localization and Classification, 2021 [[paper]](https://arxiv.org/abs/2108.02539)
* The LOCATA Challenge: Acoustic Source Localization and Tracking, TASLP 2020 [[paper]](https://arxiv.org/abs/1909.01008)

### Network design
#### MLP
  * Deep Neural Networks for Multiple Speaker Detection and Localization [[paper]](https://arxiv.org/pdf/1711.11565.pdf) [[code]]()

#### CNN
  * Deep Neural Networks for Multiple Speaker Detection and Localization, ICRA 2018 [[paper]](https://arxiv.org/pdf/1711.11565.pdf)
  * Joint Localization and Classification of Multiple Sound Sources Using a Multi-task Neural Network, Interspeech2018 [[paper]](https://www.isca-speech.org/archive_v0/Interspeech_2018/pdfs/1269.pdf)
  * Neural Network Adaptation and Data Augmentation for Multi-Speaker Direction-of-Arrival Estimation, TASLP 2021 [[paper]](https://ieeexplore.ieee.org/document/9357962)
  * Broadband DOA estimation using Convolutional neural networks trained with noise signals, 2017 [[paper]](https://arxiv.org/abs/1705.00919)
  * Multi-Speaker DOA Estimation Using Deep Convolutional Networks Trained with Noise Signals, JSTSP 2019 [[paper]](https://arxiv.org/abs/1807.11722)
  * Robust Source Counting and DOA Estimation Using Spatial Pseudo-Spectrum and Convolutional Neural Network, TASLP 2020 [[paper]](https://ieeexplore.ieee.org/document/9178434)

#### RNN & LSTM & GRU
  * Time Difference of Arrival Estimation of Speech Signals Using Deep Neural Networks with Integrated Time-frequency Masking, ICASSP 2019 [[paper]](https://ieeexplore.ieee.org/document/8682574)
  
#### CRNN
  * Direction of arrival estimation for multiple sound sources using convolutional recurrent neural network, EUSIPCO 2018 [[paper]](https://arxiv.org/abs/1710.10059)
  * Sound Event Localization and Detection of Overlapping Sources Using Convolutional Recurrent Neural Networks, JSTSP 2018 [[paper]](https://arxiv.org/abs/1807.00129)

#### Attention

  * Channel-attention dense u-net for multichannel speech enhancement, ICASSP 2020 [[paper]](https://arxiv.org/pdf/2001.11542.pdf)
  * T-GSA: transformer with gaussian-weighted self-attention for speech enhancement, ICASSP 2020 [[paper]](https://arxiv.org/pdf/1910.06762.pdf)

#### GAN
  * PAGAN: a phase-adapted generative adversarial networks for speech enhancement, ICASSP 2020 [[paper](https://ieeexplore.ieee.org/document/9054256) 
  * Time-frequency masking-based speech enhancement using generative adversarial network, ICASSP 2018 [[paper]](http://150.162.46.34:8080/icassp2018/ICASSP18_USB/pdfs/0005039.pdf)
  * SEGAN: speech enhancement generative adversarial network, Interspeech 2017 [[paper]](https://arxiv.org/pdf/1703.09452.pdf) 
### Phase reconstruction
* Phase reconstruction based on recurrent phase unwrapping with deep neural networks, ICASSP 2020 [[paper]](https://arxiv.org/pdf/2002.05832.pdf)
* PAGAN: a phase-adapted generative adversarial networks for speech enhancement, ICASSP 2020 [[paper](https://ieeexplore.ieee.org/document/9054256)
* Invertible dnn-based nonlinear time-frequency transform for speech enhancement, ICASSP 2020 [[paper]](https://arxiv.org/pdf/1911.10764.pdf)
* Phase-aware speech enhancement with deep complex u-net, ICLR 2019 [[paper]](https://openreview.net/pdf?id=SkeRTsAcYm) [[code]](https://github.com/sweetcocoa/DeepComplexUNetPyTorch)
### Learning strategy
#### Loss function
  * Speech denoising with deep feature losses, Interspeech 2019 [[paper]](https://arxiv.org/pdf/1806.10522.pdf)
  * End-to-end multi-task denoising for joint sdr and pesq optimization, Arxiv 2019 [[paper]](https://arxiv.org/pdf/1901.09146.pdf)
#### Multi-task learning
  * Joint Localization and Classification of Multiple Sound Sources Using a Multi-task Neural Network [[paper]](https://www.isca-speech.org/archive_v0/Interspeech_2018/pdfs/1269.pdf)
  * Robust Source Counting and DOA Estimation Using Spatial Pseudo-Spectrum and Convolutional Neural Network, TASLP 2020 [[paper]](https://ieeexplore.ieee.org/document/9178434)
#### Semi-supervised
  * Adaptation of Multiple Sound Source Localization Neural Networks with Weak Supervision and Domain-adversarial Training, ICASSP 2019 [[paper]](https://ieeexplore.ieee.org/document/8682655)

### Other improvements
* Improving robustness of deep learning based monaural speech enhancement against processing artifacts, ICASSP 2020 [[paper]](https://ieeexplore.ieee.org/document/9054145)
### SSL + Separation


## Tools
#### Framework

| Link | Language | Description |
| ---- | -------- | ----------- |
| [pyAudioAnalysis](https://github.com/tyiannak/pyAudioAnalysis) ![GitHub stars](https://img.shields.io/github/stars/tyiannak/pyAudioAnalysis?style=social) | Python | Python Audio Analysis Library: Feature Extraction, Classification, Segmentation and Applications. |
| [Beamformer](https://github.com/funcwj/setk/tree/master/doc/adaptive_beamformer) | Python | Implementation of the mask-based adaptive beamformer (MVDR, GEVD, MCWF). |
| [Time-frequency Mask](https://github.com/funcwj/setk/tree/master/doc/tf_mask) | Python | Computation of the time-frequency mask (PSM, IRM, IBM, IAM, ...) as the neural network training labels. |
| [SSL](https://github.com/funcwj/setk/tree/master/doc/ssl) | Python | Implementation of Sound Source Localization. |
| [Data format](https://github.com/funcwj/setk/tree/master/doc/format_transform) | Python | Format tranform between Kaldi, Numpy and Matlab. |

#### Audio feature extraction

| Link  | Language | Description |
| ----  | -------- | ----------- |
| [LPS](https://github.com/nanahou/LPS_extraction) | Python | Extract log-power-spectrum/magnitude spectrum/log-magnitude spectrum/Cepstral mean and variance normalization. |
| [MFCC](https://github.com/jameslyons/python_speech_features) ![GitHub stars](https://img.shields.io/github/stars/jameslyons/python_speech_features?style=social) | Python | This library provides common speech features for ASR including MFCCs and filterbank energies. |
| [pyAudioAnalysis](https://github.com/tyiannak/pyAudioAnalysis) ![GitHub stars](https://img.shields.io/github/stars/tyiannak/pyAudioAnalysis?style=social) | Python | Python Audio Analysis Library: Feature Extraction, Classification, Segmentation and Applications. |

#### Audio data augmentation

| Link  | Language | Description |
| ----  | -------- | ----------- |
| [Data simulation](https://github.com/funcwj/setk/tree/master/doc/data_simu) | Python | Add reverberation, noise or mix speaker. |
| [RIR simulation](https://github.com/funcwj/setk/tree/master/doc/rir) | Python | Generation of the room impluse response (RIR) using image method. |
| [pyroomacoustics](https://github.com/LCAV/pyroomacoustics) ![GitHub stars](https://img.shields.io/github/stars/LCAV/pyroomacoustics?style=social) | Python | Pyroomacoustics is a package for audio signal processing for indoor applications. |
| [gpuRIR](https://github.com/DavidDiazGuerra/gpuRIR) ![GitHub stars](https://img.shields.io/github/stars/DavidDiazGuerra/gpuRIR?style=social) | Python | Python library for Room Impulse Response (RIR) simulation with GPU acceleration |
| [rir_simulator_python](https://github.com/sunits/rir_simulator_python) ![GitHub stars](https://img.shields.io/github/stars/sunits/rir_simulator_python?style=social) | Python | Room impulse response simulator using python |


## Datasets
#### Sound source localization datasets (in no particular order) 

| Name | Utterances | Speakers | Language | Pricing | Additional information |
| ---- | ---------- | -------- | -------- | ------- | ---------------------- |
| [Dataset by University of Edinburgh](https://datashare.is.ed.ac.uk/handle/10283/1942) (2016)| 35K+ | 86 | English | Free | Noisy speech database for training speech enhancement algorithms and TTS models. |
| [TIMIT](https://catalog.ldc.upenn.edu/LDC93S1) (1993)| 6K+ | 630 | English | $250.00 | The TIMIT corpus of read speech is one of the earliest speaker recognition datasets. |
| [VCTK](https://homepages.inf.ed.ac.uk/jyamagis/page3/page58/page58.html) (2009) | 43K+ | 109 | English | Free | Most were selected from a newspaper plus the Rainbow Passage and an elicitation paragraph intended to identify the speaker's accent. |
| [WSJ0](https://catalog.ldc.upenn.edu/LDC93S6A) (1993) | -- | 149 | English | $1500 | The WSJ database was generated from a machine-readable corpus of Wall Street Journal news text. |
| [LibriSpeech](http://www.openslr.org/12) (2015) | 292K | 2K+ | English | Free | Large-scale (1000 hours) corpus of read English speech. |
| [CHiME series](https://chimechallenge.github.io/chime6/) (~2020) | -- | -- | English | Free | The database is published by CHiME Speech Separation and Recognition Challenge. | 

#### Augmentation noise sources (sorted by usage frequency in paper)

| Name | Noise types | Pricing | Additional information |
| ---- | ----------- | ------- | ---------------------- |
| [DEMAND](https://zenodo.org/record/1227121#.Xv2VsZP7RhE) (2013) | 18 | Free | Diverse Environments Multichannel Acoustic Noise Database provides a set of recordings that allow testing of algorithms using real-world noise in a variety of settings. |
| [115 Noise](http://staff.ustc.edu.cn/~jundu/The%20team/yongxu/demo/115noises.html) (2015)| 115 | Free | The noise bank for simulate noisy data with clean speech. For N1-N100 noises, they were collected by Guoning Hu and the other 15 home-made noise types by USTC.|
| [NoiseX-92](http://www.speech.cs.cmu.edu/comp.speech/Section1/Data/noisex.html) (1996)| 15 | Free | Database of recording of various noises available on 2 CDROMs. |

## SOTA results
#### STOA results in [dataset by University of Edinburgh](https://datashare.is.ed.ac.uk/handle/10283/1942). The following methods are all trained by "trainset_28spk" and tested by common testset. ("F" denotes frequency-domain and "T" is time-domain.)

| Methods | Publish | Domain | PESQ | CSIG | CBAK | COVL | SegSNR | STOI |
| ------- | ----- |------------ | ---- | ---- | ---- | ---- | ------ | ---- |
| [Noisy](https://arxiv.org/pdf/1703.09452.pdf) | -- | -- | 1.97 | 3.35 | 2.44 | 2.63 | 1.68 | 0.91 |
| [Wiener](https://arxiv.org/pdf/1703.09452.pdf) | -- | -- | 2.22 | 3.23 | 2.68 | 2.67 | 5.07 | -- |
| [SEGAN](https://arxiv.org/pdf/1703.09452.pdf) | INTERSPEECH 2017 | T | 2.16 | 3.48 | 2.94 | 2.80 | 7.73 | 0.93 |
| [CNN-GAN](http://www.apsipa.org/proceedings/2018/pdfs/0001246.pdf) | APSIPA 2018 | F | 2.34 | 3.55 | 2.95 | 2.92 | -- | 0.93 |
| [WaveUnet](https://arxiv.org/pdf/1811.11307.pdf) | arxiv 2018 | T| 2.40 | 3.52 | 3.24 | 2.96 | 9.97 | -- |
| [WaveNet](https://arxiv.org/pdf/1706.07162.pdf) | ICASSP 2018 | T | -- | 3.62 | 3.24 | 2.98 | -- | -- |
| [U-net](https://ejhumphrey.com/assets/pdf/jansson2017singing.pdf) | ISMIR 2017 | F | 2.48 | 3.65 | 3.21 | 3.05 | 9.34 | -- |
| [MSE-GAN](http://150.162.46.34:8080/icassp2018/ICASSP18_USB/pdfs/0005039.pdf) | ICASSP 2018 | F | 2.53 | 3.80 | 3.12 | 3.14 | -- | 0.93 |
| [DFL](https://arxiv.org/pdf/1806.10522.pdf) | INTERSPEECH 2019 | T | -- | 3.86 | 3.33 | 3.22 | -- | -- |
| [DFL reimplemented](https://openreview.net/pdf?id=SkeRTsAcYm) | ICLR 2019 | T | 2.51 | 3.79 | 3.27 | 3.14 | 9.86 |-- |
| [TasNet](https://arxiv.org/pdf/1809.07454.pdf) | TASLP 2019 | T | 2.57 | 3.80 | 3.29 | 3.18 | 9.65 | -- |
| [MDPhD](https://arxiv.org/pdf/1812.08914.pdf) | arxiv 2018 | T&F | 2.70 | 3.85 | 3.39 | 3.27 | 10.22 | -- |
| [Complex U-net](https://openreview.net/pdf?id=SkeRTsAcYm) | INTERSPEECH 2019 | F | 3.24 | 4.34 | 4.10 | 3.81 | 16.85 | -- |
| [Complex U-net reimplemented](https://arxiv.org/pdf/1901.09146.pdf) | arxiv 2019 | F | 2.87 | 4.12 | 3.47 | 3.51 | 9.96 | -- |
| [SDR-PRSQ](https://arxiv.org/pdf/1901.09146.pdf) | arxiv 2019 | F | 3.01 | 4.09 | 3.54 | 3.55 | 10.44 |
| [RHRnet](https://arxiv.org/pdf/1904.07294.pdf) | ICASSP 2020 | T | 3.20 | 4.37 | 4.02 | 3.82 | 14.71 | 0.98 |

## Learning materials
#### Book or thesis
  * A Study on WaveNet, GANs and General CNNRNN Architectures, 2019 [[link]](http://www.diva-portal.org/smash/get/diva2:1355369/FULLTEXT01.pdf)
  * Deep learning: method and applications, 2016 [[link]](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/DeepLearning-NowPublishing-Vol7-SIG-039.pdf)
  * Deep learning by Ian Goodfellow and Yoshua Bengio and Aaron Courville, 2016 [[link]](https://www.deeplearningbook.org/)
  * Robust automatic speech recognition by Jinyu Li and Li Deng, 2015 [[link]](https://www.sciencedirect.com/book/9780128023983/robust-automatic-speech-recognition)

#### Video
  * CCF speech seminar 2020 [[link]](https://www.bilibili.com/video/BV1MV411k7iJ)
  * Real-time Single-channel Speech Enhancement with Recurrent Neural Networks by Microsoft Research, 2019 [[link]](https://www.youtube.com/watch?v=r6Ijqo5E3I4)
  * Deep learning in speech by Hongyi Li, 2019 [[link]](https://www.youtube.com/playlist?list=PLJV_el3uVTsOK_ZK5L0Iv_EQoL1JefRL4)
  * High-Accuracy Neural-Network Models for Speech Enhancement, 2017 [[link]](https://www.microsoft.com/en-us/research/video/high-accuracy-neural-network-models-speech-enhancement/)
  * DNN-Based Online Speech Enhancement Using Multitask Learning and Suppression Rule Estimation, 2015 [[link]](https://www.microsoft.com/en-us/research/video/dnn-based-online-speech-enhancement-using-multitask-learning-and-suppression-rule-estimation/)
  * Microphone array signal processing: beyond the beamformer,2011 [[link]](https://www.microsoft.com/en-us/research/video/microphone-array-signal-processing-beyond-the-beamformer/)

#### Slides
  * Deep learning in speech by Hongyi Li, 2019 [[link]](http://speech.ee.ntu.edu.tw/~tlkagk/courses_ML19.html)
  * Learning-based approach to speech enhancement and separation (INTERSPEECH tutorial, 2016) [[link]](https://github.com/nanahou/Awesome-Speech-Enhancement/blob/master/learning-materials/2016-interspeech-tutorial.pdf)
  * Deep learning for speech/language processing (INTERSPEECH tutorial by Li Deng, 2015) [[link]](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/07/interspeech-tutorial-2015-lideng-sept6a.pdf)
  * Speech enhancement algorithms (Stanford University, 2013) [[link]](https://ccrma.stanford.edu/~njb/teaching/sstutorial/part1.pdf)
