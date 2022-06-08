---
layout: page
permalink: /allen/
title: AllenNLP Tips
description: AllenNLP tips. Last update: 9th June 2022. 
nav: false
nav_order: 2
---



## Some notes for AllenNLP's upgrade from 1.0 to 2.0



It's common practice to load a pretrained model into AllenNLP's `Predictor` class. 



In AllenNLP 1.x, we use:

```python
predictor = Predictor.from_path(
    "https://storage.googleapis.com/allennlp-public-models/structured-prediction-srl-bert.2020.12.15.tar.gz",
    cuda_device=3)
```



But this command is buggy in AllenNLP 2.x.

I have done search and trial for a few rounds, here is the solution:

```python
predictor = pretrained.load_predictor("structured-prediction-srl")
```



2.x is indeed more elegant than 1.x, but the change of syntax can be made more explicit to users. 



