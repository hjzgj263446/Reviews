## Data-Driven Proactive Policy Assurance of Post Quality in Community Q&A Sites
CHUNYANG CHEN, Monash University, Australia,
XI CHEN, JIAMOU SUN, and ZHENCHANG XING, Australian National University, Australia,
GUOQIANG LI, Shanghai Jiao Tong University, China
### summary
* 作者提出了一种基于CNN的审查并对提出不符合规定的帖子的机制
* 将问题转化为分类问题。
* 采用了Latent Dirichlet Allocation (LDA) model分析编辑过的评论用于提取主题
* 测试数据对< origional −post, post −body −edit −type >,CNN 嵌入矩阵为n*m（n为单词嵌入维度，m为句子单词数），的 filter高度等于单词维度n，max-pooling宽度为m，高度为1，利用反卷积提取key phrases
### Strengths / Novelties
* 相比于之前的研究，本文研究成果更加复杂，之前研究更多是minor revisions，处于sentence-level，本文更是post-level
* 本文不同于使用RNN采用的是CNN
### Weaknesses / Notes
