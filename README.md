# Tried to fine-tune a pretrained bert model for text classification
using a public quora dataset which predict if the given text input is told in a positive(sincere) way or in a negative(insincere) way./

The code uses the TensorFlow Hub module to load the pre-trained BERT model, and a tokenizer to convert the text data into tokenized input sequences that can be fed into the BERT model. The tokenized data is then transformed into numerical tensors using to_feature_map() and fed into the model using tf.data.Dataset for efficient input pipeline creation.

Finally, the code defines a function create_model() which builds a model that consists of the pre-trained BERT layer followed by a trainable dense layer with a single output unit and a sigmoid activation function, used to perform binary classification.( will try multiclassification in future(notcertain))

this project was guided by Snehan Kekre.
