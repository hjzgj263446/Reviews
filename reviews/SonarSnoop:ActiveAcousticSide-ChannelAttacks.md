## SonarSnoop:Active Acoustic Side-Channel Attacks 
PengCheng,Ibrahim Ethem Bagci,Utz Rozdig,Jeff Yan,May9,2018
### summary
* 第一个提出了active acoustic side-channel attack，提出了SonarSnoop Framework
* 在 Unlock Pattern Stealing方面，把备选项数量减少70%
* 通过speaker发出inaudible OFDM sound signal，microphones接受echoes，通过手指在屏幕上的移动，echo的改变进行观察
* 实验测试12个常见patterns，ml使用的是svm；D1（考虑angle and range）效果一般，D2（仅考虑angle）效果好于D1，D3（先考虑angle的基础上在进行angle和range的ml分类）在降低candidates上优于D2
### Strengths / Novelties
* 相较于大多数的side channel的passive，本文的acoustic signals是attcker主动发出的。
* sonarsnoop可以无视environment nosie
* sonarsnoop不仅可以运用于pattern，还可以扩展至，gestures，typing等
* sonarsnoop也可以实现远距离观察用户行为，即使用户操作远离屏幕，即用户操作一个ATM机时，也可能实现对用户操作的识别读取
* 不光是可以使用speaker和microphone，还可以结合使用类似于gyroscope之类的
### Weaknesses / Notes
* 因为不同手机型号的speakers and microphones不同，也即需要不同的model
* 作者实验时似乎对手机握姿有要求，不知如果对microphone有稍些遮挡，有何影响
* 用户的 interaction speed会影响性能，不过实际上大多数用户使用习惯基本保持较快速度，因此可能影响不会太大
* 实验时在每个strokes之间均有停止间隙，而实际中用户使用时并未太多pause，如何准确区分每一个strokes，作者提到可以使用单独的connected component改进。
