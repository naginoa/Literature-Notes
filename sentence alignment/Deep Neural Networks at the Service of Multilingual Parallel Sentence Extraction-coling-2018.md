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


Mohammadi and GhasemAghaee, 2010 基于 Gale and Church, 1993 的长度对齐算法减少了算法复杂度。

对于大规模数据，Barbosa et al.， 2012 使用双语词典和在线翻译服务。 Zhang et al.， 2006 提出在候选并行web页面中使用对齐器进行内容相似度估计。

S¸ tef˘anescu and Ion, 2013，使用文档中嵌入的跨语言Wikipedia链接和一个可培训的模型来生成平行句子标识的相似性评分

interwiki links

## evaluation

概率最大的句子为句对，为了验证该句对是否正确，需要一个阈值。

1.设置threshold，超过它的概率的句对即可evaluation为是真。

2.问评价的人哪些是平行的来验证阈值。

### step 1

通过正确的句对的概率，建立概率的正态分布
