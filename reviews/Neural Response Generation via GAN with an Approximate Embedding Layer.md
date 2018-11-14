## Neural Response Generation via GAN with an Approximate Embedding Layer
### Summary
* 用GAN处理query问题。
* 将query嵌入为向量h，h通过GRU生成h',G 输入（z，h'），通过全连接层softmax再与向量矩阵相乘得到一个词向量w，D：采用cnn处理G生成的r'和真实的response,r，另外一个CNN
处理query，再将query分别与r,r'连接，通过全连接层sigmoid。
### Strengths/Noveties
### Weakness/
