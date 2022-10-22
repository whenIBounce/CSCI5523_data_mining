# ANN

1. Perceptron
   - What is a perceptron?
   - What are two type of nodes in a perceptron?
   - The iterative **weight update formula** for $i^{th}$ training instance's $j^{th}$ attribute after the $k^{th}$ iteration?
     - $w_j^{(k+1)} = w_j^{(k)} + \lambda (y_i -\widehat{ y_i}^{(k)})x_{ij}$
   - Perceptron learning algorithm
   - The perceptron model is design to learn *linear* or *non-linear* decision boundaries in the attribute space?
   - What is a major limitation of perceptrons in real-world classification problems?
2. Multi-layer Neural Network
   - What is a feedforward neural network?
   - At layer $l$, the $i^{th}$ node's activation value $a_i^l$ can be expressed as?
   - The model parameters $(w, b)$ is choosing to minimize what function?
   - Why we use **backpropagation** ?
   - Learning ANN using backpropagation and gradient descent. 
3. Characteristics of ANN
   - ANN can easily handle irrelevant attributes, by using zero weights for attributes that do not help in improving the training loss.
   - Redundant attributes receive similar weights and do not degrade the quality of the classifier. However, if the number of irrelevant or redundant attributes is large, the learning of the ANN model may suffer from overfitting, leading to poor generalization performance.