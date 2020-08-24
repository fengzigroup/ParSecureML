# ParSecureML

 A Parallel Secure Machine Learning Framework on GPUs 

## Introduction

This is a source code of paper entitled "ParSecureML: An Efficient Parallel Secure Machine Learning Framework on GPUs" by Zheng Chen, Feng Zhang, Amelie Chi Zhou, Jidong Zhai, Chenyang Zhang, Xiaoyong Du,2020.

We implement a parallel secure machine learning framework on GPUS using secure multi-party computing.

## Abstract

Machine learning has been widely used in our daily lives. Large amounts of data have been continuously produced and transmitted to the cloud for model training and data processing, which raises a problem: how to preserve the security of the data. Recently, a secure machine learning system named SecureML has been proposed to solve this issue using two-party computation. However, due to the excessive computation expenses of two-party computation, the secure machine learning is about 2x slower than the original machine learning methods. Previous work on secure machine learning mostly focused on novel protocols or improving accuracy, while the performance metric has been ignored. In this paper, we propose a GPU-based framework ParSecureML to improve the performance of secure machine learning algorithms based on two-party computation. The main challenges of developing ParSecureML lie in the complex computation patterns, frequent intra-node data transmission between CPU and GPU, and complicated inter-node data dependence. To handle these challenges, we propose a series of novel solutions, including profiling-guided adaptive GPU utilization, finegrained double pipeline for intra-node CPU-GPU cooperation, and compressed transmission for inter-node communication. As far as we know, this is the first GPU-based secure machine learning framework. Compared to the state-of-the-art framework, ParSecureML achieves an average of 32.2x speedup. ParSecureML can be downloaded from https://github.com/ZhengChenCS/ParSecureML.

## Execution

1.Set CUDA path, MPI path in Makefile.

2.run ``make``.

3.run ``bin/run.sh``

## Acknowledgement

ParSecureML  is developed by Renmin University of China, Shenzhen University, Tsinghua University.

Zheng Chen, Feng Zhang, Chenyang Zhang and Xiaoyong Du are with the Key Laboratory of Data Engineering and Knowledge Engineering (MOE), and School of Information, Renmin University of China. 

Amelie Chi Zhou is with the Guangdong Province Engineering Center of China-made High Performance Data Computing System, Shenzhen University.

Jidong Zhai is with the Department of Computer Science and Technology, Tsinghua University, BNRist

If you have any questions,  please contact us (chenzheng123@ruc.edu.cn)

## Citation

 If you use our code, please cite our paper: 

```
@inproceedings{chen2020parsecureml,
author = {Zheng Chen and Feng Zhang and Amelie Chi Zhou Jidong Zhai Chenyang Zhang Xiaoyong Du},
title = {{ParSecureML: An Efficient Parallel Secure Machine Learning Framework on GPUs}},
year = {2020},
booktitle = {Proceedings of the 49th International Conference on Parallel Processing},
series = {ICPP '20}
}
```





