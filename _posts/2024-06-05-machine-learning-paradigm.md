---
layout: default
title: 机器学习的范式
---

# {{ page.title }}
---
## 传统模式
1. Training(specific) 
    - <center> $$ y = \mathfrak{F}(x, \theta)$$ </center>
    - 为特定的具体任务设计，如手写字符识别/广告点击率预估
    - 我们要做的是设计一个拟合函数$$\mathfrak{F}$$，在训练样本$$\{x_i, y_i\}_i^n$$上学习$$\theta$$
    - 使得在未见过的测试样本上，取得比较好的效果

2. Prediction(specific)
    - 利用专用模型$$\mathfrak{F}$$，在特定任务上做预估

## 新的模式
1. Pretraining(General 通用大模型)
    - 如bert/gpt2/grok/clip
    - 一个规模巨大的$$\theta$$
2. Finetuning(General/Specific)
    - 在厂商开源前，做的FT一般认为是General Task，可以提升模型基础能力。
    - 进入具体的业务场景后，再做的FT，一般是为终端的具体业务服务，比较难再给其他业务使用。
3. InContextPrompt(Specific)
    - 具体业务的prompt

<div style="text-align: center;">
</div>

---
{{ page.date | date_to_string }}
