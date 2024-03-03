# Language-Agnostic BERT Sentence Embedding
Status: Read

Author: Fangxiaoyu Feng, Yinfei Yang

Topic: Attention, Siamese Network, Text , Transformers

Category: Embeddings

Conference: arXiv

Year: 2020

Link: https://arxiv.org/abs/2007.01852

Summary: A BERT model with multilingual sentence embeddings learned over 112 languages and Zero-shot learning over unseen languages.

# Questions

### What did authors try to accomplish?

- The authors introduce a training scheme which allows BERT transformer model to learn multilingual embeddings over 112 languges.

### What were the key elements of the approach?

- Use of Monolingual data to pre-train the model for different languages. This approach has shown to give decent results in the past papers.
- Use of Paired language data for fine-tuning model for learning multilingual embeddings.
- Use of Dual encoder BERT model with shared parameters initialized by the pre-trained model on monolingual data. One encodes source language text and other encodes the target language text.
- The source and target CLS token embeddings are treated as sentence embeddings and `Additive Margin loss` is applied to bring the similar embeddings close to each other.

### What can you use yourself from this paper?

- Additive Margin loss can be used in Siamese based networks.
- Use the multilingual embeddings for models where multiple languages are possible.
- Good embedding model for low/no resource languages.

### What other references to follow?

- [Google AI Blog](https://ai.googleblog.com/2020/08/language-agnostic-bert-sentence.html)

---