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
      - [RNN \& LSTM \& GRU](#rnn--lstm--gru)
      - [CRNN](#crnn)
      - [Attention](#attention)
      - [Encoder-decoder neural networks](#encoder-decoder-neural-networks)
    - [Learning strategy](#learning-strategy)
      - [Loss function](#loss-function)
        - [MSE](#mse)
        - [Cross entropy](#cross-entropy)
      - [Multi-task learning](#multi-task-learning)
      - [Semi-supervised learning](#semi-supervised-learning)
    - [Other improvements](#other-improvements)
    - [SSL+](#ssl)
      - [SSL + Separation](#ssl--separation)
      - [Speech Enhancement + SSL](#speech-enhancement--ssl)
      - [SSL + Speaker Recognition](#ssl--speaker-recognition)
  - [Tools](#tools)
      - [Framework](#framework)
      - [Audio feature extraction](#audio-feature-extraction)
      - [Audio data augmentation](#audio-data-augmentation)
  - [Datasets](#datasets)
      - [Sound source localization datasets (in no particular order)](#sound-source-localization-datasets-in-no-particular-order)
      - [Augmentation noise sources (sorted by usage frequency in paper)](#augmentation-noise-sources-sorted-by-usage-frequency-in-paper)
  - [Learning materials](#learning-materials)
      - [Book or thesis](#book-or-thesis)
      - [Video](#video)
      - [Slides](#slides)

## Overview

This is a curated list of Awesome Sound Source Localization tutorials, papers, libraries, datasets, tools, scripts and results. The purpose of this repo is to organize the world’s resources for Sound Source Localization, and make them universally accessible and useful.

To add items to this page, you are welcomed to simply issue a Pull Request.

## Publications

### Survey
* A Survey of Sound Source Localization with Deep Learning Methods, The Journal of the Acoustical Society of America, 2022 [[paper]](https://arxiv.org/abs/2109.03465)

### Databases
* SLoClas: A Database for Joint Sound Localization and Classification, 2021 [[paper]](https://arxiv.org/abs/2108.02539) [[note]](https://zhuanlan.zhihu.com/p/433298840)
* The LOCATA Challenge: Acoustic Source Localization and Tracking, TASLP 2020 [[paper]](https://arxiv.org/abs/1909.01008)

### Network design
#### MLP
  * Deep Neural Networks for Multiple Speaker Detection and Localization [[paper]](https://arxiv.org/pdf/1711.11565.pdf) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm) [[note]](https://zhuanlan.zhihu.com/p/413083178)

#### CNN
  * Deep Neural Networks for Multiple Speaker Detection and Localization, ICRA 2018 [[paper]](https://arxiv.org/pdf/1711.11565.pdf) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm) [[note]](https://zhuanlan.zhihu.com/p/413083178)
  * Joint Localization and Classification of Multiple Sound Sources Using a Multi-task Neural Network, Interspeech2018 [[paper]](https://www.isca-speech.org/archive_v0/Interspeech_2018/pdfs/1269.pdf)
  * Adaptation of Multiple Sound Source Localization Neural Networks with Weak Supervision and Domain-adversarial Training, ICASSP 2019 [[paper]](https://ieeexplore.ieee.org/document/8682655) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm)
  * Neural Network Adaptation and Data Augmentation for Multi-Speaker Direction-of-Arrival Estimation, TASLP 2021 [[paper]](https://ieeexplore.ieee.org/document/9357962) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm) [[note]](https://zhuanlan.zhihu.com/p/426644156)
  * Broadband DOA estimation using Convolutional neural networks trained with noise signals, 2017 [[paper]](https://arxiv.org/abs/1705.00919) [[note]](https://zhuanlan.zhihu.com/p/427013456)
  * Multi-Speaker DOA Estimation Using Deep Convolutional Networks Trained with Noise Signals, JSTSP 2019 [[paper]](https://arxiv.org/abs/1807.11722) [[note]](https://zhuanlan.zhihu.com/p/429217156)
  * Robust Source Counting and DOA Estimation Using Spatial Pseudo-Spectrum and Convolutional Neural Network, TASLP 2020 [[paper]](https://ieeexplore.ieee.org/document/9178434) [[note]](https://zhuanlan.zhihu.com/p/447494486)

#### RNN & LSTM & GRU
  * Time Difference of Arrival Estimation of Speech Signals Using Deep Neural Networks with Integrated Time-frequency Masking, ICASSP 2019 [[paper]](https://ieeexplore.ieee.org/document/8682574) [[note]](https://zhuanlan.zhihu.com/p/407709624)
  
#### CRNN
  * Direction of arrival estimation for multiple sound sources using convolutional recurrent neural network, EUSIPCO 2018 [[paper]](https://arxiv.org/abs/1710.10059) [[note]](https://zhuanlan.zhihu.com/p/447493389)
  * Sound Event Localization and Detection of Overlapping Sources Using Convolutional Recurrent Neural Networks, JSTSP 2018 [[paper]](https://ieeexplore.ieee.org/document/8567942) [[note]](https://zhuanlan.zhihu.com/p/447495306) [[code]](https://github.com/sharathadavanne/seld-net)
  * CRNN-Based Multiple DoA Estimation Using Acoustic Intensity Features for Ambisonics Recordings, 2019 [[paper]](https://hal.inria.fr/hal-01839883/file/Perotin-2019-CRNN-based_multiple_DoA_estimation.pdf) [[note]](https://zhuanlan.zhihu.com/p/447506072)

#### Attention

  * A combination of various neural networks for sound event localization and detection, DCASE 2021 Challenge 
  * Sound event localization and detection using cross-modal attention and parameter sharing, DCASE 2021 Challenge

#### Encoder-decoder neural networks
  * PILOT: introducing Transformers for probabilistic sound event localization, Interspeech 2021 [[paper]](https://www.isca-speech.org/archive/pdfs/interspeech_2021/schymura21_interspeech.pdf) 

### Learning strategy
#### Loss function
##### MSE
  * Deep Neural Networks for Multiple Speaker Detection and Localization, ICRA 2018 [[paper]](https://arxiv.org/pdf/1711.11565.pdf) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm) [[note]](https://zhuanlan.zhihu.com/p/413083178)
  * Joint Localization and Classification of Multiple Sound Sources Using a Multi-task Neural Network, Interspeech2018 [[paper]](https://www.isca-speech.org/archive_v0/Interspeech_2018/pdfs/1269.pdf)
  * Adaptation of Multiple Sound Source Localization Neural Networks with Weak Supervision and Domain-adversarial Training, ICASSP 2019 [[paper]](https://ieeexplore.ieee.org/document/8682655) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm)
  * Neural Network Adaptation and Data Augmentation for Multi-Speaker Direction-of-Arrival Estimation, TASLP 2021 [[paper]](https://ieeexplore.ieee.org/document/9357962) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm) [[note]](https://zhuanlan.zhihu.com/p/426644156)
  * Robust Source Counting and DOA Estimation Using Spatial Pseudo-Spectrum and Convolutional Neural Network, TASLP 2020 [[paper]](https://ieeexplore.ieee.org/document/9178434) [[note]](https://zhuanlan.zhihu.com/p/447494486)
##### Cross entropy
  * Broadband DOA estimation using Convolutional neural networks trained with noise signals, 2017 [[paper]](https://arxiv.org/abs/1705.00919) [[note]](https://zhuanlan.zhihu.com/p/427013456)
  * Multi-Speaker DOA Estimation Using Deep Convolutional Networks Trained with Noise Signals, JSTSP 2019 [[paper]](https://arxiv.org/abs/1807.11722) [[note]](https://zhuanlan.zhihu.com/p/429217156)
  * SLoClas: A Database for Joint Sound Localization and Classification, 2021 [[paper]](https://arxiv.org/abs/2108.02539) [[note]](https://zhuanlan.zhihu.com/p/433298840)
#### Multi-task learning
  * Joint Localization and Classification of Multiple Sound Sources Using a Multi-task Neural Network [[paper]](https://www.isca-speech.org/archive_v0/Interspeech_2018/pdfs/1269.pdf)
  * Robust Source Counting and DOA Estimation Using Spatial Pseudo-Spectrum and Convolutional Neural Network, TASLP 2020 [[paper]](https://ieeexplore.ieee.org/document/9178434) [[note]](https://zhuanlan.zhihu.com/p/447494486)
#### Semi-supervised learning
  * Adaptation of Multiple Sound Source Localization Neural Networks with Weak Supervision and Domain-adversarial Training, ICASSP 2019 [[paper]](https://ieeexplore.ieee.org/document/8682655) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm)
  * Neural Network Adaptation and Data Augmentation for Multi-Speaker Direction-of-Arrival Estimation, TASLP 2021 [[paper]](https://ieeexplore.ieee.org/document/9357962) [[code]](https://github.com/FYJNEVERFOLLOWS/nnsslm) [[note]](https://zhuanlan.zhihu.com/p/426644156)
### Other improvements
* MIMO-DoAnet: Multi-channel Input and Multiple Outputs DoA Network with Unknown Number of Sound Sources, Interspeech 2022 [[paper]](https://www.isca-speech.org/archive/interspeech_2022/yin22b_interspeech.html) [[code]](https://github.com/TJU-haoran/VCTK-16k-simulated)
* Iterative Sound Source Localization for Unknown Number of Sources, Interspeech 2022 [[paper]](https://www.isca-speech.org/archive/interspeech_2022/fu22c_interspeech.html) [[code]](https://github.com/FYJNEVERFOLLOWS/ISSL)

### SSL+
#### SSL + Separation
  * Multi-Microphone Speaker Separation based on Deep DOA Estimation, EUSIPCO 2019 [[paper]](https://ieeexplore.ieee.org/document/8903121) [[note]](https://zhuanlan.zhihu.com/p/465365146)
  * An End-to-End Deep Learning Framework For Multiple Audio Source Separation And Localization, ICASSP 2022 [[paper]](https://ieeexplore.ieee.org/document/9746950) [[note]](https://zhuanlan.zhihu.com/p/518440711)
  * DBnet: Doa-Driven Beamforming Network for end-to-end Reverberant Sound Source Separation, ICASSP 2021 [[paper]](https://ieeexplore.ieee.org/document/9414187)
  * Blind Speech Separation Through Direction of Arrival Estimation Using Deep Neural Networks with a Flexibility on the Number of Speakers, MMSP 2022 [[paper]](https://ieeexplore.ieee.org/document/9949050)


#### Speech Enhancement + SSL
  * Time Difference of Arrival Estimation of Speech Signals Using Deep Neural Networks with Integrated Time-frequency Masking, ICASSP 2019 [[paper]](https://ieeexplore.ieee.org/document/8682574) [[note]](https://zhuanlan.zhihu.com/p/407709624)
  * Robust DOA Estimation Based on Convolutional Neural Network and Time-Frequency Masking, Interspeech 2019 [[paper]](https://www.isca-speech.org/archive/pdfs/interspeech_2019/zhang19j_interspeech.pdf) [[note]](https://zhuanlan.zhihu.com/p/497216650)
#### SSL + Speaker Recognition
  * Multi-task Neural Network for Robust Multiple Speaker Embedding Extraction, Interspeech 2021 [[paper]](https://www.isca-speech.org/archive/pdfs/interspeech_2021/he21_interspeech.pdf) [[note]](https://zhuanlan.zhihu.com/p/500993159)

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
| [GCC & GCC-Fbank](https://github.com/idiap/nnsslm) | Python | Python code to extract features: GCC coefficients and GCCFB. |

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

| Name | Language | Pricing | Additional information |
| ---- | -------- | ------- | ---------------------- |
| [SSLR](https://www.idiap.ch/en/dataset/sslr) (2018) | English | Free |  A collection of real robot audio recordings for the development and evaluation of sound source localization methods. |
| [LOCATA](https://www.locata.lms.tf.fau.de/datasets/) (2018) | English | Free |  |
| [SLoClas](https://bidishasharma.github.io/SLoClass/) (2021) | English | Free |  |

#### Augmentation noise sources (sorted by usage frequency in paper)

| Name | Noise types | Pricing | Additional information |
| ---- | ----------- | ------- | ---------------------- |
| [DEMAND](https://zenodo.org/record/1227121#.Xv2VsZP7RhE) (2013) | 18 | Free | Diverse Environments Multichannel Acoustic Noise Database provides a set of recordings that allow testing of algorithms using real-world noise in a variety of settings. |
| [115 Noise](http://staff.ustc.edu.cn/~jundu/The%20team/yongxu/demo/115noises.html) (2015)| 115 | Free | The noise bank for simulate noisy data with clean speech. For N1-N100 noises, they were collected by Guoning Hu and the other 15 home-made noise types by USTC.|
| [NoiseX-92](http://www.speech.cs.cmu.edu/comp.speech/Section1/Data/noisex.html) (1996)| 15 | Free | Database of recording of various noises available on 2 CDROMs. |
<!-- 
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
| [RHRnet](https://arxiv.org/pdf/1904.07294.pdf) | ICASSP 2020 | T | 3.20 | 4.37 | 4.02 | 3.82 | 14.71 | 0.98 | -->

## Learning materials
#### Book or thesis
  * Deep learning: method and applications, 2016 [[link]](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/DeepLearning-NowPublishing-Vol7-SIG-039.pdf)
  * Deep learning by Ian Goodfellow and Yoshua Bengio and Aaron Courville, 2016 [[link]](https://www.deeplearningbook.org/)

#### Video
  * CCF speech seminar 2020 [[link]](https://www.bilibili.com/video/BV1MV411k7iJ)
  * Deep learning in speech by Hongyi Li, 2019 [[link]](https://www.youtube.com/playlist?list=PLJV_el3uVTsOK_ZK5L0Iv_EQoL1JefRL4)

#### Slides
  * Deep learning in speech by Hongyi Li, 2019 [[link]](http://speech.ee.ntu.edu.tw/~tlkagk/courses_ML19.html)
