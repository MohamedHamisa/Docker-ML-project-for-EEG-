
The goal is to quickly and easily build a Docker container to run a machine learning model. We'll use three key files for this setup:

Dockerfile
train.py
inference.py
In the train.py script, EEG data from a CSV file (train.csv) will be ingested and normalized. The script will train two machine learning models using scikit-learn: a Linear Discriminant Analysis (LDA) model (clf_lda) and a Neural Networks Multi-layer Perceptron model (clf_NN). After training, the models will be saved.

The inference.py script will then load these saved models to perform batch inference on new EEG data from a CSV file (test.csv). The script will normalize the test data, make predictions using both models, and output the classification accuracy and the predicted results.
