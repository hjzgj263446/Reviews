## PassGAN: A Deep Learning Approach for Password Guessing
Briland Hitaj, Paolo Gasti, Giuseppe Ateniese and Fernando Perez-Cruz
### Summary
* 提出passgan用于password guessing，自动学习密码的分布，效果优于一般的ML方法，主要是能自动习得特别的密码规则，进而提出密码
* passgan基于IWGAN
* using 5 residual layers for both the generator and the discriminator
### Strengths / Novelties
* 能生成超过基于密码规则的方法的密码数，并且与FLA结合，效果更好
* 能非常有效的学得高频密码的分布
* 即使训练、测试时数据来自不同分布，依然展现较好的效果
### Weaknesses / Notes
* 但是对低频密码的分布习得效果较差
