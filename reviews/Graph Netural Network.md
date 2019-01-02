## Graph Netural Network
### Summary
* Neighborhood Aggregation 节点嵌入方法
  >1.搜索计算求得目标节点的所有邻接节点，根据层数可以求得邻接节点的邻接节点  
  >2.每一层可以根据自己设定的方法，比如平均节点值的方法，计算每一层的嵌入  
  >3.损失函数自己设定，比如分类就可以通过输出的嵌入向量作为计算交叉熵。  
  >#### 
* Graph Convolutional Networks 方法
  >1.
* GraphSAGE Idea 方法
  >1.将邻接节点向量映射为一个单一向量（将这个过程称为AGG），然后与目标向量链接作为这一层的输入，通过激活函数输出  
  >2.AGG可以是mean方法、Pool、LSTM方法  
  >#### 感觉有点像CGAN中的条件
* Gated Graph Neural Networks方法
  >1.采用GRU网络更新
  >2.适用于深层次的网络结构
* Subgraph Embeddings  子图嵌入不同于以上三种方法的节点嵌入
  >1.简单的将子图中每个节点向量相加
  >2.将子图用一个虚拟的节点表示，然后将这些虚拟节点当作一个graph计算
* attention 方法
  >1.引入注意力机制，顶点对（i,j） ，通过权值W ,计算  WHi||WHj  ，再通过一个权值向量a，将矩阵变为 1\*F' 的矩阵,进行softmax求得每个节点的注意力。可以同时采用多个注意力机制。
