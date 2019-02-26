# Deep Neural Networks at the Service of Multilingual Parallel Sentence Extraction

2018 coling

## abstract

维基有大量有价值的多语言语料，所以创建了一个基于维基的模型去提取平行语料。并且人工评估的方式表现还不错。

## introduction

以前的句子对齐如基于长度的等必须是按照顺序来的(same order),该模型在给定每一对句子的情况下会估计其全局概率分布。

评估方式是两层的人工评估方式。

只有句子语义相同时才算一对平行句。

翻译者都是英语母语的人。

## related work

Adafre and de Rijke, 2006 是第一个使用维基百度来做相关工作的人。他从30个维基网页中生成了源语言和目标语言的笛卡尔积，然后利用一个MT系统都翻译为英文，计算词重叠。
