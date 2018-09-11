## Single-stroke Language-Agnostic Keylogging using Stereo-Microphones and Domain Specific Machine Learning
Sashank Narain, Amirali Sanatinia and Guevara Noubir College of Computer and Information Science Northeastern University, Boston, MA
### Summary
* 基于Android OS结合stereo-microphones and gyroscopes，exceed 90% accuracy
* 结合两种方法记录声音：（1）the amplitude of audio signals at the two microphones （2）the other that uses the time delay between signals reaching
the two microphones。number of samples = （distance（T，M1）- distance（T，M2））*samples rate/speed of sound
* 采用Cubic Spline Interpolation方法对data进行resample
* 实验时算法使用了DT，k-NN,NB,但效果均不好，并未提及采用NN时的效果，只是提及nn过于笨重。
* 采用ensemble learning
### Strengths / Novelties
* 作者将keyboard划分多个区域，考虑到靠近gyroscopes区域的数据效果不好，将模型又分为只有microphone和microphone+gyroscopes的
### Weaknesses / Notes
* 轻触屏幕，或者非常吵闹的环境，或是抖动之下，效果都不会很好。
