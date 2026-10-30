# News Text Classification (Course Lab)

Classifies Reuters newswires into 46 topics with a multilayer perceptron.

**Context:** deep learning course lab. The notebook is based on code provided in the course, adapted from the Reuters example in *Deep Learning with Python* by François Chollet.

## Model
- Bag-of-words input (top 10,000 words, multi-hot encoded).
- Dense 128 (ReLU, L2) → Dropout 0.5 → Dense 64 (ReLU, L2) → Dropout 0.3 → Dense 46 (softmax).
- RMSprop, categorical cross-entropy, 30 epochs, 1,000 samples held out for validation.

## Result
Validation accuracy of **78.6%** after 30 epochs.

**Tools:** Python · TensorFlow / Keras · NumPy · matplotlib
