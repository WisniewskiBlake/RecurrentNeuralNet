# RecurrentNeuralNet
The model I used is LSTM(Long Short Term Memory) in order to stop the vanishing gradient prob. which is a problem that arises when I'm propagating the error back through the network. Specifically, the error has to go through the unraveled temporal loop and as it does that, it goes through a layer of connected neurons. The neurons are connected through a weight called "Wrec".  Because the weight is applied many many times on itself, that causes the gradient to decline rapidly; meaning the first layer of neurons is updated much slower than the last layer. So using an LSTM fixed this problem. On top of the LSTM, I used drop-out regularization to avoid over-fitting.

![](images/ml9.png)

![](images/rnn1.png)

![](images/rnn2.png)

![](images/rnn3.png)

![](images/rnn4.png)
