##
### Summary
* In practice unregularized embedding approaches often learn a degenerate identity mapping where the latent code space is free of any structure and can easily result in poor representation in dealing with real-world sparse and noisy graph data
* An encoder and a decoder ，an adjacency matrix A(structure of G) and matrix X (content features) 经过endcoder 生成Z，再将高斯分布的Z'作为正向样本经过一个discriminator进行区分。
### Strengths / Novelties
* handle both topological and content information for graph data
*
### Weaknesses / Notes
