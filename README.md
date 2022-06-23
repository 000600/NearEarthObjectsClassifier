# Near Earth Objects Classifier

## The Neural Network

This network predicts whether or not an asteroid or object in space near to earth (an NEO) is hazardous. The model will predict a value close to 0 if the asteroid is safe and a 1 if the asteroid is considered to be dangerous. Since the model only predicts binary categorical values, the model uses a binary crossentropy loss function and has 1 output neuron. The model uses a standard Adam optimizer with a learning rate of 0.001, dropout layers to prevent overfitting, and contains an architecture consisting of:
- 1 Batch Normalization layer
- 1 Input layer (with 32 input neurons and a ReLU activation function)
- 2 Hidden layers (each with 32 neurons and a ReLU activation function)
- 3 Dropout layers (one after each hidden layer and input layer)
- 1 Output layer (with 1 output neuron and a sigmoid activation function)

Feel free to further tune the hyperparameters or build upon the model!

## The Dataset
The dataset can be found at this link: https://www.kaggle.com/datasets/sameepvani/nasa-nearest-earth-objects. Credit for the dataset collection goes to **Sameep Vani**, **Shakir Ai**, **Chris X**, and others on *Kaggle* and at *NASA*. It describes the hazardousness (0 or 1) of an object in space based on multiple factors, inluding:
- Minimum estimated diameter
- Maximum estimated diameter
- Relative velocity
- Absolute magnitude

## Libraries
This neural network was created with the help of the Tensorflow and Scikit-Learn libraries.
- Tensorflow's Website: https://www.tensorflow.org/
- Tensorflow Installation Instructions: https://www.tensorflow.org/install
- Scikit Learn's Website: https://scikit-learn.org/stable/
- Scikit Learn's Installation Instructions: https://scikit-learn.org/stable/install.html
