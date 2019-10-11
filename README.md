# Programming-a-Neural-Network
## Modifications to NN hyper-parameters and functions

In this example, I modify the neural network `original-network.py` as follows (note changes in `new-network.py`):

1. Add hyper-parameters:
   + **Cost functions**, each implemented as a class with two functions: `fn()` (to compute the cost during evaluation) and `derivative()` (to compute error during learning)
      - Quadratic cost
      - Cross entropy
      - Log Likelihood
   + **Activation functions**, each implemented as a class with two functions: `fn()` (to compute the node acitivation value) and `derivative()` (to compute the error during learning)
      - Sigmoid
      - Tanh
      - ReLU
      - Softmax
   + **Regularization**, implemented as if-else conditionals
      - L1
      - L2
   + **Dropout rate**, implemented by scaling the activation values of all hidden layers during the training phase, and using the same dropout nodes during one mini-batch
2. Modify the following functions:
   + `feedforward()`
   + `update_mini_batch()`
   + `total_cost()`
  
  You can watch a 5-minute video which quickly goes over these changes below:
  
  <a href="http://www.youtube.com/watch?feature=player_embedded&v=VAZY6IwcwKI
" target="_blank"><img src="http://img.youtube.com/vi/VAZY6IwcwKI/0.jpg" 
alt="YouTube video which explains code changes" width="240" height="180" border="10" /></a>
  
  
