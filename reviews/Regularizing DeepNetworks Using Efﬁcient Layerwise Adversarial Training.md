## Regularizing DeepNetworks Using Efﬁcient Layerwise Adversarial Training 
### Summary
* Generating adversarial perturbations from intermediate layersrather than just using the input layer
* Using the gradients from the previous batch to generate adversarial perturbations for the activations of the current batch
* VGG模型上逐层增加perturbations时，效果越来越好
* 作者提出一个观点：正则性和鲁棒性之间有一个平衡。他提出的方法在正则性上更优于FGS但是鲁棒性上不及FGS
### Strengths / Novelties
* 速度相比于FGS更快，并且多层添加perturbations，虽然是前一批次的但实验表明相比于FGS只在input layer 添加perturbations 更具有adverarial。不过仅在第一层添加前一批次的perturbations效果就不如FGS。
* better capture data variations that are relevant for classifying original test data hence providing improved performance
* 在AlexNet模型，大数据集上测试accuracies 提升3.1%
* 相比于使用dropout的模型效果也更好
* 对deep model也有很好的效果
### Weaknesses / Notes
* 略低于FGS的鲁棒性
* 是否可以运用在非images模型上，作者只是提出这个观点，未实验。
* 好像没有提及同时使用dropout和自身方法的实验。
