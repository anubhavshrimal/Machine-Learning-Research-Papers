# Learning to Extract Attribute Value from Product via Question
Status: Read

Author: Li Yang, Qifan Wang

Topic: Question-Answering, Text , Transformers

Category: Zero-shot-learning

Conference: KDD

Year: 2020

Link: https://dl.acm.org/doi/pdf/10.1145/3394486.3403047

Summary: Question Answering BERT model used to extract attributes from products. Introduce further No Answer loss and distillation to promote zero shot learning.

# Questions

### What did authors try to accomplish?

- Instead of using traditional Named Entity Recognition (NER) architectures such as [BiLSTM-CNN-Softmax](https://arxiv.org/abs/1806.01264) models, the authors propose the use of Question and Answering approach using BERT.
- Given a `product description` as `context` and a `question` Eg. `What is the brand?` . The objective is to find the span of the answer from the context.

### What were the key elements of the approach?

- Use of BERT QnA architecture to solve Attribute extraction.
- Use of No Answer (NA) loss to make the model to predict when there is no answer present for a question.
- Use of distillation loss over a pre-trained BERT to retain general model knowledge so as to promote Zero-shot answers for unseen attributes.

### What can you use yourself from this paper?

- NA-loss & Distillation loss to promote zero-shot.
- Use of QnA model to scale for NER tasks as the prediction labels are just (start, end) of the span and the prediction labels do not grow as the number of labels grow (Eg. IOBES tagging in NER architecture).

### What other references to follow?

- [OpenTag NER model](https://arxiv.org/abs/1806.01264)

---