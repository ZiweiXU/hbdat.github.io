---
layout: post
title:  "Paper requirement"
date:   2020-01-18 17:40:38 -0500
---

# **A Shared Multi-Attention Framework for Multi-Label Zero-Shot Learning**
<u>Abstract:</u><br>
_In this work, we develop a shared multi-attention model for multi-label zero-shot learning. We argue that designing attention mechanism for recognizing multiple seen and unseen labels in an image is a non-trivial task as there is no training signal to localize unseen labels and an image only contains a few present labels that need attentions out of thousands of possible labels. Therefore, instead of generating attentions for unseen labels which have unknown behaviors and could focus on irrelevant regions due to the lack of any training sample, we let the unseen labels select among a set of shared attentions which are trained to be label-agnostic and to focus on only relevant/foreground regions through our novel loss. Finally, we learn a compatibility function to distinguish labels based on the selected attention. We further propose a novel loss function that consists of three components guiding the attention to focus on diverse and relevant image regions while utilizing all attention features. By extensive experiments, we show that our method improves the state of the art by 3.3% and 1.4% F1 score on the NUS-WIDE and the large scale Open Images datasets, respectively._

<div style="text-align:center"><img src="/img/attentionZSL.png" width="500"/></div>

- [Main Paper](https://drive.google.com/file/d/1vgPO_n1TW8IwEcXLK5w-4MfEjc73gO3t/view?usp=sharing) 
- [Supplementary Material](https://drive.google.com/file/d/1CIeMjWfi49IbB7fh1yy9e3GfB9mxxjMM/view?usp=sharing)

#### Statement from [Prof. Ehsan Elhamifar](https://www.ccs.neu.edu/home/eelhami/):
>Dat Huynh is in his 3rd year of PhD studies and has 3 papers in CVPR 2020, which is the top computer vision conference. Dat's research revolves around development of new algorithms for large-scale recognition and learning with less/no labeled data. 
>
>In particular, in his paper "A Shared Multi-Attention Framework for Multi-Label Zero-Shot Learning", he proposed a novel algorithm for multi-label zero-shot learning based on deep attention models. Multi-label learning refers to the problem of finding all existing labels in an image and in contrast to the multi-class classification, which finds only the dominant label in an image, is a much harder problem to address, due to conflicting information from different labels, which makes feature learning a very hard task in multi-label settings. The problem becomes much more challenging when many labels do not have any training annotations, which is referred to as zero-shot learning. Dat developed a new method for multi-label zero-shot learning by making the interesting observation that in order to classify all labels, the system has to focus on relevant regions in an image. However, existing attention models cannot generalize to unseen labels. Dat proposed a shared multi-attention model where different attention mechanisms learn to automatically focus on relevant labels, while each attention autonomously becomes an expert for recognizing a subset of relevant labels. He proposed a new learning mechanism in order to train these attention mechanism to be effectively used, be diverse and can find label-relevant regions without any ground-truth bounding-box annotations. Dat performed extensive experiments on two large image datasets, including the Open Images dataset, with more than 5000 classes and 10 Millions images, showing his methods outperform the few existing work on this challenging problem. 
>
>The paper was accepted in CVPR 2020 with acceptance ratings from all reviewers. 
