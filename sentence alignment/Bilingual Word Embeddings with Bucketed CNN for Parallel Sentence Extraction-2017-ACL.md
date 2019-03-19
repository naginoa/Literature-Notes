# Bilingual Word Embeddings with Bucketed CNN for Parallel Sentence Extraction

## model

### 1.双语embedding

### 2.相似矩阵  行代表S1,列代表s2.   S(i, j) 表示s1的wi和s2的wj的相似性度量。

### 3.Bucketing and Dynamic Poling
### 要把相似矩阵池化为固定维度的矩阵，但是这样很短的句子和很长的句子有一样的维度。所以将句子按照不同的长度范围进行分组。
### 如果len < dim 就复制元素直到满足条件， 如果有剩余就放到最后一行。

### 4.CNN
### 使用CNN可以既包含相似分数，还可以知道单词顺序。
