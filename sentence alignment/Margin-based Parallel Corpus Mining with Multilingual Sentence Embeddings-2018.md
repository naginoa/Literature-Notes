# Margin-based Parallel Corpus Mining with Multilingual Sentence Embeddings

## Architecture

embedding  encoder  decoder

encoder：

embedding -> biLSTM -> max pooling -> result:sentence embeddings

decoder:

1:embeddings from encoder liner tranform then to initialize LSTM.

2:embeddings from encoder concatenated to the input embeddings.
