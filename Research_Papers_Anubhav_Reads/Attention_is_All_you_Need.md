# Attention is All you Need
Status: Read

Author: Ashish Vaswani, Illia Polosukhin, Noam Shazeer, Łukasz Kaiser

Topic: Attention, Text , Transformers

Category: Architecture

Conference: NIPS

Year: 2017

Link: http://papers.nips.cc/paper/7181-attention-is-all-you-need

Summary: Talks about Transformer architecture which brings SOTA performance for different tasks in NLP

# Questions

### What did authors try to accomplish?

The authors propose a new architecture for NLP tasks which alleviates the sequential processing issue of RNNs. They propose the use of only Attention network to combine and find relations between the words.

### What were the key elements of the approach?

- Use of only attention layers and feed forward neural networks
- Introduction to positional embeddings to induce sense of sequence
- Multi headed attention to attend the embeddings in different feature space

### What can you use yourself from this paper?

- Transformers are powerful models giving SOTA performance in various tasks in machine learning
- They have now become a default go to option whenever a problem needs to be solved

### What other references to follow?

- [http://jalammar.github.io/illustrated-transformer/](http://jalammar.github.io/illustrated-transformer/)
- BERT, T5, GPT2, GPT3, etc. are all transformer based models
- Hugging face is a good open source github repo which gives implementations of different transformer models and tasks

---