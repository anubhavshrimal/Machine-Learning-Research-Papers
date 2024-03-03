# Bag of Tricks for Image Classification with Convolutional Neural Networks
Status: Read

Author: Tong He, Zhi Zhang

Topic: CV , Image 

Category: Optimizations, Tips & Tricks

Conference: arXiv

Year: 2018

Link: https://arxiv.org/abs/1812.01187

Summary: Shows a dozen tricks (mixup, label smoothing, etc.) to improve CNN accuracy and training time.

# Questions

### What did authors try to accomplish?

- The authors show different tricks which when applied to CNN training can help improve the accuracy of models such as ResNet, Inception V3, MobileNet, etc.
- They show that these tricks are consistent across different models and datasets and also helps in improving downstream task performance using these models.

### What were the key elements of the approach?

- **Efficient Training using:**
    - Large batch
    - Linear scaling learning rate
    - Learning rate warmup
    - Zero gamma for batch normalization
    - No bias decay
- **Training Refinements using:**
    - Cosine learning rate decay
    - Label smoothing
    - Knowledge distillation
    - Mixup training

### What can you use yourself from this paper?

- The tricks discussed in the paper are general and can be applied in other works to help improve the model performance.

### What other references to follow?

- N/A

---