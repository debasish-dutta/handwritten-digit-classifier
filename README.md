# Handwritten-Digit-Classifier

## Problem

In this I tend to create a neural network model to classify handwritten digits.
![nn]

## Data

The data is taken from MINST dataset and then is divided into training, validation and test datasets of about 50k, 10k and 10k subsecuently.
The data are greyscale images of 28 by 28 px. These are then flattened into about 784px.

## Model Creatiion

The model is created withh 3 laters - the input layer with 2 hidden layer and the output layer with a learning rate of le-3. The first hidden layer consists of 512 nodes and the 2nd hidden layer with 64 nodes. The model is then trained in batched of 1000 and total of 50 epochs.
![graph]

## Evaluation

The model is evaluated on 2 metrices - accuracy and loss. It uses the Adam optimizer.
![graph_acc]
![graph_cost]

---

The histogram chart of the model on different layers are
layer1_biases
[layer1_biases]
layer1_weights_train
![layer1_weights_train]
out_biases
![out_biases]
out_weigts
![out_weigts]

## Saving

The model is saved using the tf.v1 Saved Model method.

### Accuracy on test set is 97.92%.

[nn]: "tensorboard_mnist_digit_logs/graphs_models/graph.png"
[graph]: "tensorboard_mnist_digit_logs\graphs_models\graph.png"
[graph_acc]: "tensorboard_mnist_digit_logs\graphs_models\graph_acc.png"
[graph_cost]: "tensorboard_mnist_digit_logs\graphs_models\graph_cost.png"
[layer1_biases]: "tensorboard_mnist_digit_logs\graphs_models\layer1_biases.png"
[layer1_weights_train]: "tensorboard_mnist_digit_logs\graphs_models\layer1_weights_train.png"
[out_biases]: "tensorboard_mnist_digit_logs\graphs_models\out_biases.png"
[out_weigts]: "tensorboard_mnist_digit_logs\graphs_models\out_weigts.png"
