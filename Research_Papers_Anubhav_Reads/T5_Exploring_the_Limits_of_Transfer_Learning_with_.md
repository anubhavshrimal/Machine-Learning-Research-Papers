# T5: Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer
Author: Colin Raffel, Noam Shazeer, Peter J. Liu, Wei Liu, Yanqi Zhou

Conference: JMLR

Link: https://arxiv.org/abs/1910.10683

Status: Read

Summary: Presents a Text-to-Text transformer model with multi-task learning capabilities, simultaneously solving problems such as machine translation, document summarization, question answering, and classification tasks.

Topic: Attention, Text , Transformers

Year: 2020

# Questions

### What did authors try to accomplish?

- Presents a Text-to-Text transformer model with multi-task learning capabilities, simultaneously solving problems such as machine translation, document summarization, question answering, and classification tasks.
- They also present a large-scale empirical survey to determine which transfer learning techniques work best.

### What were the key elements of the approach?

- Presents a Text-To-Text framework for transformers.
- Introduce a new large unlabelled corpus named Colossal Clean Crawled Corpus (C4), a cleaned version of Common Crawl that is two orders of magnitude larger than Wikipedia.
- Paper explores:
    - *model architectures*, where they found that encoder-decoder models generally outperformed "decoder-only" language models;
    - *pre-training objectives*, where they confirmed that fill-in-the-blank-style denoising objectives (where the model is trained to recover missing words in the input) worked best and that the most important factor was the computational cost;
    - *unlabelled datasets*, where they showed that training on in-domain data can be beneficial but that pre-training on smaller datasets can lead to detrimental overfitting;
    - *training strategies*, where they found that multitask learning could be close to competitive with a pre-train-then-fine-tune approach but requires carefully choosing how often the model is trained on each task;

### What can you use yourself from this paper?

- Using the model in Text-to-Text generation tasks.

### What other references to follow?

- [Google AI Blog](https://ai.googleblog.com/2020/02/exploring-transfer-learning-with-t5.html)

---