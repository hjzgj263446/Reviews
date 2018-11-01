## A simple neural network module for relational reasoning
### Summary
* 提出一个RNs（relation networks）feature maps作为object
* 一个CNN层卷积提取feature maps,LSTM用于解析问题为一个向量q，每两个object链接一个q通过gθ，求和
### Strengths / Novelties
* 模型简单，并且性能相比之前的模型都有提升，甚至性能超过人类。
* 也能学到复杂的关系
* 对于某些可能存在关系的问题，使用这个方法可以较大提升性能
### Weaknesses / Notes
* 
