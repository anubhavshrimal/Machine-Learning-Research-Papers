# Pix2Pix: Image-to-Image Translation with Conditional Adversarial Nets
Author: Alexei A. Efros, Jun-Yan Zhu, Phillip Isola, Tinghui Zhou

Conference: CVPR

Link: https://arxiv.org/abs/1611.07004

Status: Read

Summary: Image to image translation using Conditional GANs and dataset of image pairs from one domain to another.

Topic: GANs, Image 

Year: 2017

# Questions

### What did authors try to accomplish?

- A Conditional GAN architecture that can perform many different image to image translation given a labelled dataset of image pairs.

### What were the key elements of the approach?

- Show that the loss functions need not be hand engineered for different Image to Image translation tasks.
- Use of Encoder-Decoder (U-Net) architecture as Generator for better quality outputs.
- Use of Patch GAN Discriminator to speed up the inference time .
- Show the ability to train model on small images (286x286) while being able to apply on larger images convolutionally in patches.
- Experiments to compare normal GAN with Conditional GAN.
- Show effects of L1 loss on image sharpness.

### What can you use yourself from this paper?

- Conditional GANs understanding.
- Effects of using losses such as L1 for image generation tasks.
- Use of Image Patch based Discriminator for low parameters and faster training/inference.

### What other references to follow?

- [https://phillipi.github.io/pix2pix](https://phillipi.github.io/pix2pix/)/

---