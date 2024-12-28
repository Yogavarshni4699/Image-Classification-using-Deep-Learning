# Image-Classification-using-Deep-Learning

## Data Set: https://www.kaggle.com/datasets/sidharkal/sports-image-classification/data
This dataset consists of labeled images belonging to the following sports classes:
cricket, wrestling, tennis, badminton, soccer, swimming, and karate.

I have tried 11 experiments in this task with various deep learning techniques

Model, Layers / Neurons, Activation, Batch Size, Epochs, Loss Function, Optimizer, Regularization, Trainable parameter, Explanation

1
512 → 256
ReLU
32
20
CrossEntropyLoss
Adam
Dropout (0.3)
77203975
Simple architecture with fast learning and overfitting prevention.

2
512 → 256
ReLU
64
20
CrossEntropyLoss
RMSprop
L2 Regularization
77205511
Simple model with weight control and fast convergence.

3
1024 → 512 → 256
Tanh
64
50
CrossEntropyLoss
SGD
Batch Normalization
154803207
Deeper network with fast convergence and better generalization.

4
1024 → 512 → 256 → 128
Leaky ReLU
16
25
CrossEntropyLoss
RMSprop
L2 Regularization
154831623
Prevents dead neurons with dynamic learning and weight control.

5
512 → 256
Leaky ReLU
16
10
CrossEntropyLoss
SGD
L2 Regularization
77203975
Small batch size with generalization and weight control.

6
512 → 256
Tanh
32
20
Focal Loss
Adam
Dropout (0.3)
77203975
Focal Loss handles class imbalance with fast learning.

7
1024 → 512 → 256 → 128
Tanh
64
50
Focal Loss
SGD
Dropout (0.3)
154831623
Balances learning with Dropout and SGD generalizes well.

8
1024 → 512 → 256
ReLU
32
20
CrossEntropyLoss
Adam
Batch Normalization
77212807
Adam improves performance with stable learning.

9
1024 → 512 → 256
Tanh
16
50
CrossEntropyLoss
SGD
Dropout (0.3)
154799623
Tanh with Dropout balances learning and avoids overfitting.

10
1024 → 512 → 256 → 128
ReLU
32
50
CrossEntropyLoss
Adam
L2 Regularization
154831623
Deep model with efficient optimization and weight control.


