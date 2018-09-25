## Yet Another Text Captcha Solver:A Generative Adversarial Network Based Approach
Guixin Ye,Zhanyong Tang,Dingyi Fang,Zhanxing Zhu,Yansong Feng,Pengfei Xu
### Summary
* 利用GAN创建了一个captchas solver，结果显示效果很好，优于目前最先进的几个solver，并且还能用于这些solver不能使用的地方。  
* step
  * step1.训练一个GAN，用于生成captchas,其中有一个CNN层用于生成干扰
  * step2.pre-processing 基于pix2pix训练一个GAN用于去掉干扰
  * step3.用based on aclassical CNN called （LeNet-5） 训练没有干扰的captchas，输出字符
  * step4.采用转移学习精炼slover
### Strengths / Novelties
* significantly reduces the number of real captchas needed. paper中表示仅使用500张即可
* 整体训练速度快，标签训练数据使用少，人工消耗也远远减少
* pre-processing methods 效果很好，能够很好地移除干扰，这个方法应该还可以运用到其他地方。

### Weaknesses / Notes
* 对于非常复杂captchas，还是难以生成相似的captchas，比如谷歌的captchas
