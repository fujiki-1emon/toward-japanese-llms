# Resources toward Japanese LLMs

## Table of Contents
- [Pre-training datasets](#pre-training-datasets)
- [Downsteam tasks](#donwstream-tasks)
- [Tokenization](#tokenization)
- [Models](#models)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)

## General
- A Survey of Large Language Models [[arXiv]](https://arxiv.org/abs/2303.18223)

## Pre-training datasets
### The Pile
- The Pile: An 800GB Dataset of Diverse Text for Language Modeling [[arXiv]](https://arxiv.org/abs/2101.00027)
  - noted: Pile-CC
- The Pile has 0.07%（approx. 900 M chars）of Japanese texts based on the types of the characters.
  - cf. [The Pileの構成（なぜCerebras-GPTで日本語が使えるのか？）](https://staka.jp/wordpress/?p=854)

### The ROOTS
- [The BigScience ROOTS Corpus: A 1.6TB Composite Multilingual Dataset](https://openreview.net/forum?id=UoEw6KigkUn)

## Donwstream tasks
### Question Answering
- Better Question-Answering Models on a Budget [[ArXiv]](https://arxiv.org/abs/2304.12370v1)
  - Having briefly checked it, it looks interesting, but only compared their models to OPTs?


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
- Performance report of rinna/japanese-gpt-1b fine-tuned on Japanese version (translation) of Dolly dataset [[tweet]](https://twitter.com/kun1em0n/status/1651849601505464320?s=20)
  - <img width="477" alt="スクリーンショット 2023-04-29 11 19 01" src="https://user-images.githubusercontent.com/8359397/235279258-1c28d56e-dd6d-4eda-82b5-a0ab02555439.png">

### Alignment
- Learning to summarize from human feedback [[arXiv]](https://arxiv.org/abs/2009.01325)
- Training language models to follow instructions with human feedback [[arXiv]](https://arxiv.org/abs/2203.02155)

### RLHF
- RLHF works because it's rating full sentences
  -  https://twitter.com/savvyRL/status/1651255588813443073?s=20
  -  https://twitter.com/mr_bay_area/status/1651594421551644678?s=20
      -  Sequence Level Training with Recurrent Neural Networks [[arXiv]](https://arxiv.org/abs/1511.06732)


## Evaluation
- [EleutherAI/lm-evaluation-harness: v0.3.0](https://zenodo.org/record/7413426)
- [japanese-toxic-dataset](https://github.com/inspection-ai/japanese-toxic-dataset)


## Practical
- Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond [[ArXiv]](https://arxiv.org/abs/2304.13712)

# What I've developed
- [t5-efficient-xl-nl6-japanese](https://huggingface.co/JapaNLP/t5-efficient-xl-nl6-japanese)
- [ul2-base-japanese](https://huggingface.co/JapaNLP/ul2-base-japanese)
- [ul2-large-japanese](https://huggingface.co/JapaNLP/ul2-large-japanese)
