# Deconstructing Lottery Tickets: Zeros, Signs, and the Supermask
Author: Hattie Zhou, Janice Lan, Jason Yosinski, Rosanne Liu

Category: Comparison, Optimization-No. of params, Tips & Tricks

Conference: NeurIPS

Link: https://arxiv.org/abs/1905.01067

Status: Read

Summary: Follow up on Lottery Ticket Hypothesis exploring the effects of different Masking criteria as well as Mask-1 and Mask-0 actions.

Topic: NN Initialization, NNs

Year: 2019

# Questions

### What did authors try to accomplish?

- The authors further explore the [The Lottery Ticket Hypothesis: Finding Sparse, Trainable Neural Networks](The%20Lottery%20Ticket%20Hypothesis%20Finding%20Sparse,%20Trai%20f3a7b3e3c81448cd9e2f016bc099e57f.md) by exploring the effects of different Masking criteria as well as Mask-1 and Mask-0 actions.
- They also show the effects of using the learned mask without training the model at all also gives improvement in accuracy.

### What were the key elements of the approach?

- Using different thresholding criteria for pruning weights
- Using different Mask-1 actions such as reshuffling the weights, replacing with a constant value.
- Using different Mask-0 actions such as replacing with original init, replacing only the weights which improved in magnitude, etc.
- Use of masks learned by the lottery ticket on top of the untrained model to observe improvement in accuracy more than random.
- Training these learned masks (called Supermasks) to achieve even further improvement in accuracy without training the network weights.

### What can you use yourself from this paper?

- Pruning the n/w weights to reduce model training time and parameters.

### What other references to follow?

- [Youtube video](https://www.youtube.com/watch?v=jhCInVFE2sc)

---