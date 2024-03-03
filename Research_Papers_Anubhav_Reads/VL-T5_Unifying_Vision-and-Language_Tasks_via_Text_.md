# VL-T5: Unifying Vision-and-Language Tasks via Text Generation
Status: Read

Author: Hao Tan, Jaemin Cho, Jie Le, Mohit Bansal

Topic: CNNs, CV , Generative, Image , Large-Language-Models, Question-Answering, Text , Transformers

Category: Architecture, Embeddings, Multimodal, Pre-Training

Conference: arXiv

Year: 2021

Link: https://arxiv.org/pdf/2102.02779.pdf

Summary: Unifying two modalities (image and text) together in a single transformer model to solve multiple tasks in a single architecture using text prefixes similar to T5.

# Questions

### What did authors try to accomplish?

- Unifying two modalities (image and text) together in a single transformer model.
- Solving multiple tasks (QnA, Summarization, VQA, etc.) in a single architecture.
- Pre-training the model to solve multiple tasks at once using Task specific prefixes.

### What were the key elements of the approach?

- Mapping the image features in the text space using `<vis_1>` type tokens whose embedding is a combination of ROI features of FasterRCNN model.
- Mapping visual embeddings of each region to region_ids for each region using `<vis_1>` in pretraining.
- Using T5/BART as backbones to show the efficacy of their approach.
- Allowing 2 images also added to the model using `image_ids`.
- Using a generative decoder based method contrary to the existing soltuions which are classification based methods.

### What can you use yourself from this paper?

- Use this architecture to train multimodal multitask models for solving various problems by fine-tuning on task specific dataset.
- How to embed different modalities together in a transformer network.

### What other references to follow?

- Faster RCNN paper: [https://arxiv.org/abs/1506.01497](https://arxiv.org/abs/1506.01497)
- T5 paper: [https://arxiv.org/abs/1910.10683](https://arxiv.org/abs/1910.10683)

---