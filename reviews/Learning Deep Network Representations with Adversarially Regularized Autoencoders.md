## Learning Deep Network Representations with Adversarially Regularized Autoencoders
### Summary
* 提出了一个network representations模型，用以更好的嵌入表现。能以保存网络的结构信息，提高泛化能力
* 基本结构：encoder采用lstm捕获点与点之间的信息，将嵌入的向量作为正样本输入GAN进行学习，通过gan反馈回的梯度，更新encoder。最终实现encoder生成的向量分布更加
区分。
### Strength/Noveties
### Weakness/Notes
