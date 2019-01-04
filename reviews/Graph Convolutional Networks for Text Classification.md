## Graph Convolutional Networks for Text Classification
### Summary
>* 不同于一般的分类方法是在词嵌入学习之后再进行的分类，文中的方法是词嵌入与分类同时进行学习。
>* 特征向量取单位向量，所有的边基于单词、文档之间出现的情况作为连接，WORD-DOC采用TF-IDF做边的权值,WORD-WORD采用PMI做边的权值。
### Weakness
>* MR数据集上在sentiment classification方面效果不如LSTM\CNN，作者分析原因之一就是没有考虑单词顺序,因此是否可以采用GGNN或者采用有向图来做？
