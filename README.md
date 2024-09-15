# Presentation
This Python project uses the PyTorch library to predict the value of a digit represented by an image (28x28x3). These digit images have different colorations.

# Installation
- Install Python libraries
```sh
pip install -r requirements.txt
```
When the program is run, the following files are downloaded locally into the cloned directory: 
- __MACOSX
- customX_test
- customX_train.NPY
- customY_train.NPY
- dataset

These represent training and test data. They don't weigh much more than 50MB. They can be easily deleted.

# Algorithm configuration
The internal values used for the algorithm can be modified in the `Automaton_CNN_figures.py` file.
To name just a few important ones:

```
python
BATCH_SIZE = 64
EPOCHS = 10
lr=1e-4
```

|argument|type|description|
|-|-|-|
|BATCH_SIZE|int|The size of the data batch used for training|
|EPOCHS|int|The number of epochs used to train the model|
|lr|float|The learning rate of the optimizer (“Adam” here)|


**Notes**: All values must be modified with full knowledge of the facts. No check is made on the consistency of the values.
The last part “Interacion with the model” can only be executed in google colab. It allows you to draw figures interactively and see the associated model prediction.