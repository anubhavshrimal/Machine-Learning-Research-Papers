# Evaluation of neural network architectures for embedded systems
Status: Read

Author: Adam Paszke, Alfredo Canziani, Eugenio Culurciello

Topic: CNNs, CV , Image 

Category: Comparison

Conference: IEEE ISCAS

Year: 2017

Link: https://ieeexplore.ieee.org/abstract/document/8050276

Summary: Compare CNN classification architectures on accuracy, memory footprint, parameters, operations count, inference time and power consumption.

# Questions

### What did authors try to accomplish?

- Compare 14 different CNN architectures in past 4 years (from publish date) on accuracy, memory footprint, parameters, operations count, inference time and power consumption.
- The idea is that even though CNN architectures have improved over time in terms of prediction accuracy, they may be inefficient in the resources they consume and very huge in number of parameters the possess.

### What were the key elements of the approach?

- N/A

### What can you use yourself from this paper?

- The model's resource utilization / number of params should also be a key aspect of consideration when showing SOTA results.
- Many models now a days utilize huge GPUs to train for long hours and are not feasible to run for inference on usual machines.

### What other references to follow?

- N/A

---