# Text Classification



## CNN usage in text classification

Convolutional Neural Networks (CNNs) excel in extracting hierarchical features from fixed-size windows. In text classification, CNNs excel at local feature extraction, offering complementary strengths for comprehensive analysis and accurate predictions.



## CNN layers

In this case, we use a neuron network including the following layers:

1. **Input Layer:**
   - Accepts word embeddings or one-hot encoded vectors representing words in the input text.
2. **Convolutional Layer (Conv1D):**
   - Convolutional filters slide over the input to detect local patterns.
   - The number of filters represents different learned features.
   - Filter size determines the span of the local patterns.
3. **ReLU Activation Layer:**
   - Introduces non-linearity by applying the Rectified Linear Unit (ReLU) activation function to the output of the convolutional layer.
4. **Pooling Layer (Max Pooling):**
   - Reduces spatial dimensions by selecting the maximum value from a set of values within a local region.
   - Helps in capturing the most relevant features and reducing computation.
5. **Fully Connected Layer:**
   - Flattens the output from the pooling layer and connects every neuron to each other, capturing global patterns.
   - Typically followed by ReLU activation.
6. **Output Layer:**
   - Produces the final output, representing class probabilities for text classification tasks.
   - Sigmoid activation for binary classification or softmax for multiclass classification.



