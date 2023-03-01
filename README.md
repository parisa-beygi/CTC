# CTC

CTC loss (Connectionist Temporal Classification loss) is an algorithm used in machine learning for sequence labelling tasks, such as speech recognition or optical character recognition. The problem in sequence labeling is that we do not know the how the tokens in the output align to the input tokens. The CTC loss function is designed to enable the training of neural networks to make predictions about sequences where the alignment between the input and output sequences is not known in advance.

The CTC loss function involves summing over all possible paths through the output sequence that could produce the observed input sequence, and then normalizing by the total number of such paths. The goal of training the neural network is to minimize this loss function, which encourages the network to learn to predict the correct output sequence given the input sequence.

In this repository, we revisit the task of image recognition in the form of sequences of MNIST digits, where digits tend to overlap, making it challenging to establish bounding boxes for each digit. In such cases, the Connectionist Temporal Classification (CTC) algorithm treats the complete sequence as a unit and employs the forward-backward algorithm to assign the suitable labeling. The code accepts input sequences in a similar manner to the following example. The dataset could be found under dataset

```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```
