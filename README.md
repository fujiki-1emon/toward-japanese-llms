# japanese-llms-resources

## Table of Contents
- [Pre-training datasets](#pre-training-datasets)
- [Downsteam tasks](#donwstream-tasks)
- [Tokenization](#tokenization)
- [Models](#models)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)

## Pre-training datasets
### The Pile
- The Pile has 0.07%（approx. 900 M chars）of Japanese texts based on the types of the characters.
  - cf. [The Pileの構成（なぜCerebras-GPTで日本語が使えるのか？）](https://staka.jp/wordpress/?p=854)


## Donwstream tasks
### Question Answering
- Better Question-Answering Models on a Budget [[ArXiv]](https://arxiv.org/abs/2304.12370v1)
  - Looks interesting, but only compared their models to OPTs?


## Tokenization
### [LINE Distill BERT](https://github.com/line/LINE-DistilBERT-Japanese)
- Word segmentation by MeCab+UniDic + subword tokenization by SentencePiece


## Models
### [abeja/gpt-neox-japanese-2.7b](https://huggingface.co/abeja/gpt-neox-japanese-2.7b)
- [ABEJAで作った大規模GPTモデルとその道のり](https://tech-blog.abeja.asia/entry/abeja-gpt-project-202207)


## Model Architecture
- [ABEJA GPTモデルにおけるアーキテクチャの工夫](https://tech-blog.abeja.asia/entry/abeja-gpt-model-202208)


## Training
- [GPT-neoxの学習用にマルチノード並列学習環境を整えた with DeepSpeed](https://tech-blog.abeja.asia/entry/abeja-gpt-neox-infra-202208)


## Fine-tuning
- [【インターンレポート】6.7B日本語モデルに対するLoRAチューニング](https://engineering.linecorp.com/ja/blog/lora-tuning-for-japanese-model)
- Self-Instruct: Aligning Language Model with Self Generated Instructions [arXiv](https://arxiv.org/abs/2212.10560)
  - https://twitter.com/rasbt/status/1650866140892069892?s=20


## Evaluation
- [EleutherAI/lm-evaluation-harness: v0.3.0](https://zenodo.org/record/7413426)
- [japanese-toxic-dataset](https://github.com/inspection-ai/japanese-toxic-dataset)


## Practical
- Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond [[ArXiv]](https://arxiv.org/abs/2304.13712)
