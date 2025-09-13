Transformer input:

Each record → 1 numerical embedding + 3 categorical embeddings → 4 tokens.

Self-attention captures feature interactions.

Classifier:

Simple MLP on top of the pooled transformer output (context vector).

Sample size is small (NSL-KDD dataset):

Training: 2,000

Testing: 500

Fast for Colab demo.

Working Process at a glance:
4. Intuition

Q (query) = what the feature “wants to know.”

K (key) = what identity/info the feature exposes.

V (value)= the actual information it contributes when chosen.

So in NSL-KDD:

src_bytes (Q) “asks”: Am I normal in this protocol?

protocol (K) responds: I’m ICMP, which makes your size suspicious.

protocol (V) passes this info into the updated src_bytes'.
