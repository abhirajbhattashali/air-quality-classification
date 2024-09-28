# Air Quality Classification

This project focuses on building and evaluating a classification model to predict air quality categories using machine learning techniques.

## Introduction
The goal of this project is to classify air quality based on various pollutant levels. The model is built using TensorFlow and Keras, and it is evaluated using metrics like accuracy and F1-score.

## Dataset
The dataset used in this project consists of air quality measurements. It includes features such as PM2.5, PM10, NO, NO2, NOx, NH3, CO, SO2, O3, Benzene, Toluene, Xylene, and AQI.


## Model Architecture
The model consists of:
- An input layer that expects 13 features (pollutant levels).
- A hidden Dense layer with 10 neurons using ReLU activation.
- An output Dense layer with 6 neurons using softmax activation.

Here is the model architecture from the script:

```python
# Design the model
model = Sequential()
# Add the input layer
model.add(InputLayer(input_shape=(x_train.shape[1],)))
# Add a hidden layer
model.add(Dense(10, activation='relu'))
# Add an output layer 
model.add(Dense(6, activation='softmax'))
```

## Evaluation
The model is evaluated using the classification report, which includes metrics like precision, recall, and F1-score.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

