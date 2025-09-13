Transformer input:

Each record → 1 numerical embedding + 3 categorical embeddings → 4 tokens.

Self-attention captures feature interactions.

Classifier:

Simple MLP on top of the pooled transformer output (context vector).

Sample size is small (NSL-KDD dataset):

Training: 2,000

Testing: 500

Fast for Colab demo.
