# SqueezeNet
Status: Read

Author: Forrest N. Iandola, Song Han

Topic: CNNs, CV , Image 

Category: Architecture, Optimization-No. of params

Conference: arXiv

Year: 2016

Link: https://arxiv.org/abs/1602.07360

Summary: Explores model compression by using 1x1 convolutions called fire modules.

# Questions

### What did authors try to accomplish?

- The authors try to reduce the model size/parameters while preserving the model accuracy.
- They were able to get 50x smaller model as compared to AlexNet while having the same accuracy.
- By applying other model compression accuracy got 500x smaller model.

### What were the key elements of the approach?

- The authors use 3 major strategies:
    - Replace 3x3 filters with 1x1 filters
    - Decrease the number of input channels to 3x3 filters
    - Downsample late in the network so that convolution layers have large activation maps
- They introduce a Fire module which comprises of only 1x1 conv followed by a Expand module with 1x1 and 3x3 convs.
- They also explore effects of using Residual connections between Fire modules.
- They also explore effect of increasing or decreasing number of 3x3 convs in Expand module.

### What can you use yourself from this paper?

- Use of 1x1 conv to decrease the model parameters and other strategies to preserve the model accuracy.

### What other references to follow?

---