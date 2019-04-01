## Co-Regularized Deep Multi-Network Embedding
### Summary
  * 提出了一个DMNE的框架， 即Deep Multi-Network Embedding。该模型可以视作为一个AutoEncoder
  * 框架结构：
    * 采用RWR方法，为每一个节点计算到达其他所有结点的k-step概率，得到矩阵A，将矩阵A作为该模型的输入 。  
    * 采用了两种损失函数，ED AND PD. 
      * ED 最小化两个网络间向量表示的相似度误差。通过两个网络的关系权重S，从j网络乘以S得到新的向量表示j',比较j’ 与 i之间的相似度误差，适用于矩阵维度相等的情况。
      * PD ii网络相似的节点x，y在 j网络映射后的j'也应该相似，因为构建了一个相似度误差。即x，y向量的点乘-j’网络映射下x'，y'向量的点乘。适用于维度不同的网络。
### Strength
 * 引入了一个矩阵U，替代H，便于计算。并且这个U就当作网络表示
### Weakness
