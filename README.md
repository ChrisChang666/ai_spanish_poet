# AI Spanish Poet
## Deep learning model to generate spanish love poems

This a  mini-project developed for a "Sant Jordi" poem contest hosted at my company.

The idea is to train a deep learning model to write spanish love poems
First, the model will be tranined with thousands of famous spanish poems
Then, train it to write love theme poems trough transfer learning technique


## First at all, What is Sant Jordi?

## What is the contest about?


## AI Poet submission
> Here will be the final poem generated by the model



## How the AI poet was trained?
General description of the project structure

## Data
webscraping and data insights

## Training with general theme
model iteration and final network

```python
model = Sequential()
# Mask parts of the lookback period that are all zeros (i.e., unobserved) so they don't skew the model
model.add(Masking(mask_value=-1., input_shape=(train_x.shape[1], train_x.shape[2])))
# layer 1
model.add(LSTM(HIDDEN_NEURONS, return_sequences=True))
model.add(Dropout(0.2))
# layer 2
model.add(LSTM(HIDDEN_NEURONS, return_sequences=True)))
model.add(Dropout(0.2))
# layer 3
model.add(LSTM(HIDDEN_NEURONS))
model.add(Dropout(0.2))
# Final layer
model.add(Dense(train_y.shape[1], activation='softmax'))
# compile
model.compile(loss='categorical_crossentropy',
              optimizer='adam',
              metrics=['accuracy'])
```

## Transfer Learning with love poems
improvements comparison of baseline model vs love model