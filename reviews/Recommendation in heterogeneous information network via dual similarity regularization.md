### Recommendation in heterogeneous information network via dual similarity regularization
## Summary
  * 目前推荐系统的不足：
    * 整合用户信息不完善。
    * 用户的信息可能是稀疏的，例如cold-start
    * 训练时可能会导致本来不相似的user，迫使他们相似
  * 利用HIN构造了 dual similarity regularization-based recommendation method，which imposes constraints on users and items with high and low
similarities simultaneously
  * based on the basic matrix factorization framework
  
## Strength
  * can constrain the latent features of users and items with arbitrary similarity simultaneously 
  * achieve the best performance for cold-start users and items
## Weakness
  * 代价函数既然想要考虑最大化相似度和最小化不相似，那么采用交叉熵作为代价函数呢
