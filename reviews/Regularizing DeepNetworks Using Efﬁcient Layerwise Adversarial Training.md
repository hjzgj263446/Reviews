## Regularizing DeepNetworks Using Efﬁcient Layerwise Adversarial Training 
### Summary
* Generating adversarial perturbations from intermediate layersrather than just using the input layer
* Using the gradients from the previous batch to generate adversarial perturbations for the activations of the current batch

### Strengths / Novelties
* 计算量相比于FGS低
* better capture data variations that are relevant for classifying original test data hence providing improved performance
*
### Weaknesses / Notes
* 略低于FGS的鲁棒性
