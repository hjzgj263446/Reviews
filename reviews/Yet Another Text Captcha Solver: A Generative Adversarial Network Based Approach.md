## Yet Another Text Captcha Solver:
A Generative Adversarial Network Based Approach
Guixin Ye,Zhanyong Tang,Dingyi Fang,Zhanxing Zhu,Yansong Feng,Pengfei Xu
### Summary
* 利用GAN创建了一个captchas solver，结果显示效果很好，优于目前最先进的几个solver，并且还能用于这些solver不能使用的地方。
* step1.训练一个GAN，用于生成captchas.
  step2.基于pix2pix训练一个GAN用于去掉干扰
  step3.用CNN训练之前产生的数据，输出字符，
  step4.采用转移学习精炼slover
### Strengths / Novelties
* significantly reduces the number of real captchas needed. paper中表示仅使用500张即可
### Weaknesses / Notes
