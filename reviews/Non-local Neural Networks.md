## Non-local Neural Networks
### Summary
* 简单来说就是可以在训练模型中增加一个Non-local block，少量的增加了计算量，换取获得更远位置的关系信息。提升模型性能。
### Strengths / Novelties
* capture long-range dependencies directly by computing interactions between any two positions, regardless of their positional distance
* efficient and achieve their best results even with only a few layers
* maintain the variable input sizes and can be easily combined with other operations
### Weaknesses / Notes
