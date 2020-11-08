# BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding
Author: Jacob Devlin, Ming-Wei Chang

Category: Embeddings

Conference: NAACL

Link: https://arxiv.org/abs/1810.04805

Status: Read

Summary: BERT is an extension to Transformer based architecture which introduces a masked word pretraining and next sentence prediction task to pretrain the model for a wide variety of tasks.

Topic: Text , Transformers

Year: 2018

# Questions

### What did authors try to accomplish?

- The authors propose a way to pre-train a model through both directions instead of just left to right or right to left fashion by masking intermediate words.
- They also introduce next sentence prediction task by giving two sentences as input to the model.
- These pretrainings allows the model to train on a varied number of tasks in a semi-supervised fashion and then be fine tuned for many different tasks giving SOTA results.

### What were the key elements of the approach?

- Bidirectional embedding learning
- Next sentence prediction as pretraining task

### What can you use yourself from this paper?

- Bert provides pretrained models on large corpus which can then be finetuned for many down stream tasks.

### What other references to follow?

---