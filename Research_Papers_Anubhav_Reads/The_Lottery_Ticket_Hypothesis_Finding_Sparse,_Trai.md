# The Lottery Ticket Hypothesis: Finding Sparse, Trainable Neural Networks
Author: Jonathan Frankle, Michael Carbin

Category: Optimization-No. of params, Tips & Tricks

Conference: ICLR

Link: https://arxiv.org/abs/1803.03635

Status: Read

Summary: Lottery ticket hypothesis: dense, randomly-initialized, feed-forward networks contain subnetworks (winning tickets) that—when trained in isolation— reach test accuracy comparable to the original network in a similar number of iterations.

Topic: NN Initialization, NNs

Year: 2019

# Questions

### What did authors try to accomplish?

- Authors proposed the Lottery ticket hypothesis: dense, randomly-initialized, feed-forward networks contain subnetworks (winning tickets) that—when trained in isolation— reach test accuracy comparable to the original network in a similar number of iterations.
- They showed that this subnetwork if initialized by its original network weights can achieve same or even better performance that the original network in same or smaller training iterations.
- Comparing the hypothesis on both Dense networks as well as CNNs.

### What were the key elements of the approach?

- Identifying winning tickets:
    1. Randomly initialize a neural network f (x; θ0) (where θ0 ∼ Dθ ).
    2. Train the network for j iterations, arriving at parameters θj .
    3. Prune p% of the parameters in θj , creating a mask m.
    4. Reset the remaining parameters to their values in θ0, creating the winning ticket f (x; m*θ0).
- This can be done in oneshot fashion but iterative pruning and training showed to achieve better results.
- Pruned network randomly underperformed as compared to when initialized by the original network initial weights.

### What can you use yourself from this paper?

- Network pruning to get smaller networks with similar performance.

### What other references to follow?

- [Youtube video explanation](https://youtu.be/ZVVnvZdUMUk)
- Follow up work on different masking strategies: [Deconstructing Lottery Tickets: Zeros, Signs, and the Supermask](https://arxiv.org/abs/1905.01067)
    - Database link: [Deconstructing Lottery Tickets: Zeros, Signs, and the Supermask](Deconstructing%20Lottery%20Tickets%20Zeros,%20Signs,%20and%20t%201479cb3c504642c99041fb329c2fe53c.md)
- There can be bias in pruned models where it underperforms for minority classes: [Characterising Bias in Compressed Models](https://arxiv.org/abs/2010.03058)

---