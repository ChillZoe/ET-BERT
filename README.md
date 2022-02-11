# ET-BERT

[![codebeat badge](https://codebeat.co/badges/f75fab90-6d00-44b4-bb42-d19067400243)](https://codebeat.co/projects/github-com-linwhitehat-et-bert-main)
![](https://img.shields.io/badge/license-MIT-000000.svg)
[![arXiv](https://img.shields.io/badge/arXiv-1909.05658-<color>.svg)](https://arxiv.org/abs/1909.05658)

**The repository of ET-BERT, a network traffic classification model on encrypted traffic.**

ET-BERT is a method for learning datagram contextual relationships from encrypted traffic, which could be **directly applied to different encrypted traffic scenarios and accurately identify classes of traffic**. First, ET-BERT employs multi-layer attention in large scale unlabelled traffic to learn both inter-datagram contextual and inter-traffic transport relationships. Second, ET-BERT could be applied to a specific scenario to identify traffic types by fine-tuning the labeled encrypted traffic on a small scale.

![The framework of ET-BERT](images/etbert.png)

The work is introduced in the 31st The Web Conference:
> Xinjie Lin, Gang Xiong, Gaopeng Gou, Zhen Li, Junzheng Shi and Jing Yu. 2022. ET-BERT: A Contextualized Datagram Representation with Pre-training Transformers for Encrypted Traffic Classification. In Proceedings of The Web Conference (WWW) 2022, Lyon, France. Association for Computing Machinery. 

Note: this code is based on [UER-py](https://github.com/dbiir/UER-py). Many thanks to the authors.
<br/>

Table of Contents
=================
  * [Requirements](#requirements)
  * [Datasets](#datasets)
  * [Download ET-BERT](#download-et-bert)
  * [Using ET-BERT](#using-et-bert)
  * [Reproduce ET-BERT](#reproduce-et-bert)
  * [Citation](#citation)
  * [Contact](#contact)

<br/>

## Requirements
* Python >= 3.6
* torch >= 1.1
* six >= 1.12.0
* scapy == 2.4.4
* numpy == 1.19.2
* argparse
* packaging
* [scikit-learn](https://scikit-learn.org/stable/)
* For the mixed precision training you will need apex from NVIDIA
* For the pre-trained model conversion (related with TensorFlow) you will need TensorFlow
* For the tokenization with wordpiece model you will need [WordPiece](https://github.com/huggingface/tokenizers)
* For the use of CRF in sequence labeling downstream task you will need [pytorch-crf](https://github.com/kmkurn/pytorch-crf)
<br/>

## Datasets
The real-world TLS 1.3 dataset is collected from March to July 2021 on China Science and Technology Network (CSTNET). For privacy considerations, we only release part of the anonymous data. Other datasets are publicly available.

If you want to use your own data, please check if the data format is the same as `datasets/cstnet-tls1.3.zip` and specify the data path in `dataloader.py`.
<br/>

## Download ET-BERT

<br/>

## Using ET-BERT

<br/>

## Reproduce ET-BERT

<br/>

## Citation
#### If you are using the work (e.g. pre-trained model) in ET-BERT for academic work, please cite the [paper](https://arxiv.org/pdf/1909.05658.pdf) published in WWW 2022:

```
@inproceedings{Lin2022etbert,
  author        = {Lin, Xinjie and Xiong, Gang and Gou, Gaopeng and Li, Zhen and Shi, Junzheng and Yu, Jing.},
  title         = {ET-BERT: A Contextualized Datagram Representation with Pre-training Transformers for Encrypted Traffic Classification},
  year          = {2022},
  month         = apr,
  isbn          = {9781450390965},
  publisher     = {Association for Computing Machinery},
  booktitle     = {Proceedings of The Web Conference 2022},
  numpages      = {10},
}
```

<br/>

## Contact
Please post a Github issue if you have any questions.
