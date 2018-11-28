## Adversarial Feature Matching for Text Generation
### Summry
* 利用一个encoder-decoder模型加上一个Gan生成文本。
* G利用LSTM模型，通过z生成S^,与真实句子s，然后输入一个CNN的D，产生的中间特征向量f^,f.f^与f求MMD，f^与f进行D鉴别。f^最后再经过decoder生成z^进行重构误差。
### Strength/Novties
* 将D中的cnn层的特征层真实样本与假样本进行MMD比较，是否可以扩充至其他领域。
### weakeness/
* decoder重构的为什么不能是s，通过s^,重构出的句子再与s比较。
