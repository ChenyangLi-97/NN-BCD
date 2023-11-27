# On Model Compression for Neural Networks: Framework, Algorithm, and Convergence Guarantee

This is the code implementation of NN-BCD algorithm in _On Model Compression for Neural Networks: Framework, Algorithm, and Convergence Guarantee_

# Abstract
Model compression is a crucial part of deploying neural networks, especially when the memory of computing devices is limited in many applications. This paper focuses on two model compression techniques: low-rank approximation and weight pruning in neural networks, which are very popular nowadays. However, training NN with low-rank approximation and weight pruning always suffers significant accuracy loss and convergence issues. In this paper, a holistic framework is proposed for model compression from a novel perspective of nonconvex optimization by designing an appropriate objective function. Then, we introduce NN-BCD, a block coordinate descent (BCD) algorithm to solve the nonconvex optimization. One advantage of our algorithm is that an efficient iteration scheme can be derived, which is gradient-free. With the Kurdyka-Lojasiewicz (K\L) property of our objective function, we show that our algorithm globally converges to a critical point at the rate of O(1/k), where k denotes the number of iterations. Lastly, extensive experiments with tensor train decomposition and weight pruning demonstrate the efficiency and superior performance of our training framework.  


# Code Folder Structure
`CNN`:1 convolution layer and 2 fully-connected layers structure, TTD+BCD algorithm, MNIST dataset <br>
`MLP`: 3 & 4 layers MLP structure, TTD+BCD algorithm, UCI-HAR dataset <br>
`Weight Pruning`: LeNet300-100 structure, Pruning+BCD algorithm, Solar Flare dataset <br>
  - `NN-BCD`: main implementation of NN-BCD
  - `different hyperparameters`: effect of different hyperparameters of NN-BCD
  - `weight init`: Stability of different weight initialization methods of NN-BCD

     
     
