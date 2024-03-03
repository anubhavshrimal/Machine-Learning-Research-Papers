# SpanBERT: Improving Pre-training by Representing and Predicting Spans
Status: Read

Author: Danqi Chen, Mandar Joshi

Topic: Question-Answering, Text , Transformers

Category: Pre-Training

Conference: TACL

Year: 2020

Link: https://www.aclweb.org/anthology/2020.tacl-1.5/

Summary: A different pre-training strategy for BERT model to improve performance for Question Answering task.

# Questions

### What did authors try to accomplish?

- Introduce a new pre-training strategy for BERT model for improved performance on Question Answering task.

### What were the key elements of the approach?

- **Span Masking:** Instead of the conventional masking of random tokens in BERT, the authors mask a contiguous span of text.
- **Span Boundary Objective:** Predicting each token of the masked span using only the representations of the observed tokens at the boundaries.

### What can you use yourself from this paper?

- Using a different pre-training objective relevant to your task can help in improving model performance.

### What other references to follow?

- N/A

---