# Reformer: The Efficient Transformer
Author: Anselm Levskaya, Lukasz Kaiser, Nikita Kitaev

Category: Architecture, Optimization-Memory, Optimization-No. of params

Conference: arXiv

Link: https://arxiv.org/abs/2001.04451

Status: Read

Summary: Overcome time and memory complexity of Transformers by bucketing Query, Keys and using Reversible residual connections.

Topic: Attention, Text , Transformers

Year: 2020

# Questions

### What did authors try to accomplish?

- Reduce the Transformer’s time complexity of O(L^2) to O(L log L) where L is the sequence length.
- Reduce the memory requirements of transformers by using Reversible residual connections to avoid saving activations for all layers in the network.

### What were the key elements of the approach?

- Introduced Locality Sensitive Hashing which maps Query and Key vectors into similar buckets such that similar vectors are mapped to the same bucket.
- These buckets are then sorted and chunked into equal sizes to avoid having a single large bucket.
- Now, instead of looking at the complete sequence length to find the query key mappings, relations are found only from within the bucket and also from adjacent bucket to prevent loss of information due to chunking. (Ref. Fig 2 in paper)
- They use Reversible residual networks to allow model to recompute activations for backpropagation without the need to store the activations during the forward pass.
- This allowed the Reformers to be used for sequence length of 64k tokens with just 16GB RAM in comparison to just 512 tokens in BERT transformer.

### What can you use yourself from this paper?

- Locality sensitive hashing for grouping similar vectors together to avoid large time complexity overheads.
- Reversible Residual Networks to save memory by avoiding to save activations.

### What other references to follow?

---