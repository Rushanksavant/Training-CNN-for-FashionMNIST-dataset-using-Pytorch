## Context:

Fashion-MNIST is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000
examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes. Zalando intends Fashion-MNIST to 
serve as a direct drop-in replacement for the original MNIST dataset for benchmarking machine learning algorithms. I
t shares the same image size and structure of training and testing splits.
The original MNIST dataset contains a lot of handwritten digits. Members of the AI/ML/Data Science community love this dataset 
and use it as a benchmark to validate their algorithms. In fact, MNIST is often the first dataset researchers try. "If it 
doesn't work on MNIST, it won't work at all", they said. "Well, if it does work on MNIST, it may still fail on others."

Zalando seeks to replace the original MNIST dataset


## Labels

Each training and test example is assigned to one of the following labels:

0-T-shirt/top;
 1-Trouser;
 2-Pullover;
 3-Dress;
 4-Coat;
 5-Sandal;
 6-Shirt;
 7-Sneaker;
 8-Bag;
 9-Ankle boot


## About the Algorithm

PyTorch is an open source machine learning library based on the Torch library, used for applications such as computer vision 
and natural language processing, primarily developed by Facebook's AI Research lab. It is free and open-source software 
released under the Modified BSD license.

Pytorch has been used to train the CNN for FashionMNIST dataset.
A class 'Network' is created containing the architecture for the CNN which includes, two convolution layers and three 
fully connected/linear layers. Onto which forward propogation is applied followed by calculation of loss function(cross-entropy)
and back propogation to reduce it as well as gradient by updating the randomly initialized weights.
The batchs of dataset (with a definite batch size) are passed to the 'network' to complete a single epoch. And the accuracy is
calculated by dividing the correct predictions by length of training set. The number of correct predictions are calculated by
a pre-defined function. 
This process is repeated until 10 epochs and finally the accuracy of model is calculated (above 88%).
To visualize the training results the confusion matrix is created for the predicted results of the model, followed by the
plotting of heatmap.


## License

The MIT License (MIT) Copyright © [2017] Zalando SE, https://tech.zalando.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation 
files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, 
modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the 
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS 
BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT 
OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
