# DeeperForensics-1.0: A Large-Scale Dataset for Real-World Face Forgery Detection

![firstfigure](supports/first_figure.png)

This repository will provide code, model and data for the following paper：

**DeeperForensics-1.0: A Large-Scale Dataset for Real-World Face Forgery Detection**<br>
[Liming Jiang](https://liming-jiang.com/),  [Wayne Wu](http://wywu.github.io), [Ren Li](https://liren2515.github.io/page/), [Chen Qian](https://scholar.google.com/citations?user=AerkT0YAAAAJ&hl=en)  and [Chen Change Loy](http://personal.ie.cuhk.edu.hk/~ccloy/)<br>
To appear on arXiv.<br>
[**Project Page**](https://liming-jiang.com/projects/DrF1/DrF1.html) |   [**Paper**]() | [**YouTube Demo**](https://www.youtube.com/watch?v=b6iKqkJht38)
> **Abstract:** *In this paper, we present our on-going effort of constructing a large-scale benchmark, DeeperForensics-1.0, for face forgery detection. Our benchmark represents the largest face forgery detection dataset by far, with 60,000 videos constituted by a total of 17.6 million frames, 10 times larger than existing datasets of the same kind. Extensive real-world perturbations are applied to obtain a more challenging benchmark of larger scale and higher diversity. All source videos in DeeperForensics-1.0 are carefully collected, and fake videos are generated by a newly proposed end-to-end face swapping framework. The quality of generated videos outperforms those in existing datasets, validated by user studies. The benchmark features a hidden test set, which contains manipulated videos that successfully deceived human eyes. We further contribute a comprehensive study that evaluates five representative detection baselines and make a thorough analysis of different settings. We believe this dataset will contribute to real-world face forgery detection research.*

![comparison](supports/comparison.png)

## Overview

### Data Collection
We invited 100 paid actors from 26 countries to record the source videos. Our high-quality collected data vary in identities, poses, expressions, emotions, lighting conditions, and 3DMM blendshapes.
<p align="center">
  <img height="320" src="supports/source.gif">
</p>

### Face Manipulation
We also propose a new learning-based **many-to-many** face swapping method,
 **DeepFake Variational Auto-Encoder (DF-VAE)**. DF-VAE improves *scalability*,
  *style matching*, and *temporal continuity* to ensure face swapping **quality**.
<p align="center">
  <img src="supports/DF-VAE.png">
</p>

Several face manipulation results:
<p align="center">
  <img src="supports/manipulation.gif">
</p>

Many-to-many (three-to-three) face swapping by a **single** model:
<p align="center">
  <img src="supports/m2m.png">
</p>

### Real-World Perturbation
We apply 7 types (transmission errors, compression, *etc.*) of distortions 
at 5 intensity levels. Some videos are subjected to a mixture of more than 
one distortion. These perturbations make DeeperForensics-1.0 better simulate
real-world scenarios.
<p align="center">
  <img src="supports/perturbations.png">
</p>

### Benchmark
We benchmark five representative open-source forgery detection methods 
using our DeeperForensics-1.0 dataset. Please refer to our [paper]() 
for more information.

## Installation
The **code** of our face manipulation method, DF-VAE, will be open-source. 
Please stay tuned.

## Downloads
DeeperForensics-1.0 **dataset** and the **models** will be made publicly available 
for non-commercial research purposes. Please stay tuned.

## Citation
If you find this work useful for your research, please cite our paper:
```
```
## Acknowledgments
We gratefully acknowledge the exceptional help from Hao Zhu and Keqiang Sun for source data collection and coordination.