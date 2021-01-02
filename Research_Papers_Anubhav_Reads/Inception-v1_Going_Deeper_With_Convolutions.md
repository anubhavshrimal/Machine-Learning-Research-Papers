# Inception-v1 (Going Deeper With Convolutions)
Author: Christian Szegedy, Wei Liu

Category: Architecture

Conference: CVPR

Link: https://arxiv.org/abs/1409.4842

Status: Read

Summary: Propose the use of 1x1 conv operations to reduce the number of parameters in a deep and wide CNN 

Topic: CNNs, CV , Image 

Year: 2015

# Questions

### What did authors try to accomplish?

- The authors try to reduce the number of parameters in a deep CNN whilte still increasing the depth and width of the network

### What were the key elements of the approach?

- Use of 1x1 convolutions to reduce the number of parameters
- Stacking of inception modules which combines max pooling, 3x3, 5x5 and 1x1 conv operations together
- Adding intermediate softmax layers to propogate error in earlier layers.

### What can you use yourself from this paper?

- Use of 1x1 conv operations to reduce the number of filters and dense connections in a model

### What other references to follow?

---