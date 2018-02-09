# Video-Recognition-using-LSTM

Trained an LSTM model for action recognition in a video dataset. The project is implemented in TensorFlow Framework..

## Dataset
The dataset contains 588 videos each of 4 to 6 seconds in length.
Each video consist of 50 frames of 2048 pixels each.
The videos were divided in 5 categories:
1. Cricket Bowling : Consist of bowling videos from cricket matches.
2. Cricket Shot: Consist of videos of batsman hitting balls in cricket games.
3. Pizza Tossing: Consist of videos of persons tossing pizzas in the air.
4. Playing Cello: Consists of videos of people playing cello.
5. Playing Sitar: Consists of videos of people playing sitar.

## Preprocessing
All the videos were divided into frames and were passed through a Convolutional Neural Network (VGG16) and features were stored as sequential data in a npz file. The data was divided into training set and validation set.

## Model
Model consist of a basic LSTM cell with 128 neurons along with a dynamic rnn layer.
The whole model was implemented in TensorFlow framework.

## Training
Training was done on batches of size 32. Adam Optimizer was used with learning rate = 1e-4, beta1 = 0.9 beta2 = 0.999 and epsilon = 1e-8.
Training was successful with approximately 90% accuracy on the validation set
Softmax classification was used with cross entropy loss.


