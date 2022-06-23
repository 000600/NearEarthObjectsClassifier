# Near Earth Objects Classifier

## The Neural Network

This network predicts whether or not an asteroid or object in space near to earth (an NEO) is hazardous. The model will predict a value close to 0 if the asteroid is safe and a 1 if the asteroid is considered to be dangerous. Since the model only predicts binary categorical values, the model uses a binary crossentropy loss function and has 1 output neuron. The model uses a standard Adam optimizer with a learning rate of 0.001 and contains an architecture consisting of:
- 1 Batch Normalization Layer
- 1 Input Layer (with 512 input neurons)
- 3 Hidden Layers (2 with 256 neurons and 1 with 512; each with a ReLU activation function)
- 3 Batch Normalization Layers (one after each hidden layer)
- 1 Output Layer (with 1 output neuron and a sigmoid activation function)

Feel free to further tune the hyperparameters or build upon the model!

## The Dataset
The dataset can be found at this link: https://www.kaggle.com/andrewmvd/heart-failure-clinical-data. Credit for the dataset collection goes to **Larxel** on *Kaggle*. It describes the death event (0 or 1) of a patient based on 11 factors, inluding:
- Age
- Anaemia
- Creatinine Phosphokinase
- Diabetes
- Blood Pressure
- Platelets

## Libraries
This neural network was created with the help of the Tensorflow and Scikit-Learn libraries.
- Tensorflow's Website: https://www.tensorflow.org/
- Tensorflow Installation Instructions: https://www.tensorflow.org/install
- Scikit Learn's Website: https://scikit-learn.org/stable/
- Scikit Learn's Installation Instructions: https://scikit-learn.org/stable/install.html
