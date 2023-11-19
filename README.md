# Neural Networks Classification Projects
This repository contains a few projects where Neural Networks were used to solve classification problems.

## Heart Failure Project

### Overview
The [dataset](https://github.com/sergiobaezlugo/Neural_Networks_Classification_Projects/blob/main/heart_failure.csv) was used to predict the survival ('death_event' column) of patients with heart failure from serum creatinine, ejection fraction, age, anemia, diabetes, etc. The dataset is from Kaggle. Here's a preview: 

|index|age|anaemia|creatinine\_phosphokinase|diabetes|ejection\_fraction|high\_blood\_pressure|platelets|serum\_creatinine|serum\_sodium|sex|smoking|time|death\_event|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|0|75\.0|no|582|no|20|yes|265000\.0|1\.9|130|yes|no|4|yes|
|1|55\.0|no|7861|no|38|no|263358\.03|1\.1|136|yes|no|6|yes|
|2|65\.0|no|146|no|20|no|162000\.0|1\.3|129|yes|yes|7|yes|
|3|50\.0|yes|111|no|20|no|210000\.0|1\.9|137|yes|no|7|yes|
|4|65\.0|yes|160|yes|20|no|327000\.0|2\.7|116|no|no|8|yes|


### NN Architecture and Hyperparameters
A simple Feedforward Neural Network with one hidden layer (12 units and ReLu activation function) and output layer with 2 units (Softmax activation function) was used.

Adam optimization was used with batch_size = 16, loss = sparse_categorical_crossentropy, and epochs = 100.

[Code](https://github.com/sergiobaezlugo/Neural_Networks_Classification_Projects/blob/main/heart_failure.ipynb)

### Performance
The model achieved accuracy = 0.7666666507720947 and F1_score = 0.7666666666666667 on the test data.
