# ResNet (Deep Residual Learning for Image Recognition)
Author: Kaiming He, Xiangyu Zhang

Category: Architecture

Conference: CVPR

Link: https://openaccess.thecvf.com/content_cvpr_2016/html/He_Deep_Residual_Learning_CVPR_2016_paper.html

Status: Read

Summary: Introduces Residual or Skip Connections to allow increase in the depth of a DNN

Topic: CNNs, CV , Image 

Year: 2016

# Questions

### What did authors try to accomplish?

- Authors try to increase the depth of a DNN while resolving the issues of vanishing gradients due to depth.

### What were the key elements of the approach?

- Introduces Residual / Skip connections between layers to propagate gradients from higher layers directly to lower layers.

### What can you use yourself from this paper?

- Residual connections generally give better performance in many different models especially when the model is deep.
- Such connections are also made between encoder-decoder models to propagate features learned from earlier layers directly to higher layers. Eg. see U-Net model.

### What other references to follow?

---