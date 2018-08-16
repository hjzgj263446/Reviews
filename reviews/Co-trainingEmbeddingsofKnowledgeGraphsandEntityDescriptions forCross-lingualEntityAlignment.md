## Co-training Embeddings of Knowledge Graphsand Entity Descriptions forCross-lingual Entity Alignment
MuhaoChen,YingtaoTian,Kai-WeiChang,StevenSkiena and CarloZaniolo,18 Jun 2018
### Summary
* 因为现有的KGs大多数并未完全entity alignment从而影响了一些应用，为此本篇提出了一个新方法KDCoE，基于一个multilingual KG embedding model（KGEM）和一个multilingual literal description embedding model(DEM)的Co-training用于改善semi-supervised learning。结果显示在entity alignment这方面效果很好，并且在zero-shot entity alignment和cross-lingual KG completion方面也很有前景。
* KGEM 基于TransE，类似于改进版的MTransE-LT，
* DEM，采用了两层36个输入的AGRU单元作为encoder
### Strengths / Novelties
* entity alignment，zero-shot alignment， KG completion方面效果显著
* 基于co-training
### Weaknesses / Notes
* 
* 
