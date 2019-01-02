## Graph Netural Network
### Summary
* Neighborhood Aggregation 节点嵌入方法
  >1.搜索计算求得目标节点的所有邻接节点，根据层数可以求得邻接节点的邻接节点  
  >2.每一层可以根据自己设定的方法，比如平均节点值的方法，计算每一层的嵌入  
  >3.损失函数自己设定，比如分类就可以通过输出的嵌入向量作为计算交叉熵。  
  * 
* Graph Convolutional Networks 方法
  >1.
* GraphSAGE Idea 方法
  >1.将邻接节点向量映射为一个单一向量（将这个过程称为AGG），然后与目标向量链接作为这一层的输入，通过激活函数输出  
  >2.AGG可以是mean方法、Pool、LSTM方法  
  >#### 感觉有点像CGAN中的条件
* Gated Graph Neural Networks方法
  >1.e
  >2.e
