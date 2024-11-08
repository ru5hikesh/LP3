Here's a simpler overview of the key concepts in this assignment:

### 1. **Artificial Neural Network (ANN) Basics**
   - **Input Layer**: Takes data (e.g., customer data) and passes it through the network.
   - **Hidden Layer**: The part of the network where calculations are done to identify patterns in the data. Multiple layers of neurons help the model learn complex relationships.
   - **Output Layer**: Produces the final output (prediction), such as whether the customer will leave or stay.

### 2. **Activation Functions**
   - Activation functions decide if a neuron should activate (or "fire"). They add non-linearity, allowing the model to learn complex patterns.
   - Common activation functions include **ReLU** (Rectified Linear Unit) and **Sigmoid**. For binary classification (like predicting if a customer will leave), **Sigmoid** is often used in the output layer.

### 3. **Keras**
   - **Keras** is a user-friendly, high-level library for building neural networks. It’s widely used because it simplifies complex coding by acting as a wrapper for low-level libraries like **TensorFlow**.
   - **TensorFlow** is a library that performs calculations on CPUs and GPUs, supporting Keras in running deep learning models effectively.

### 4. **Normalization and Standardization**
   - **Normalization**: Scales data between 0 and 1. Useful when features have different ranges (like age and salary) to prevent any single feature from dominating the model.
   - **Standardization**: Centers data around 0 with a standard deviation of 1. Often used if the data follows a normal (bell curve) distribution. 

   - **Which to use?**: Use normalization if you don’t know the distribution; it’s often helpful in neural networks. Use standardization if the data distribution is known and is normal.

### 5. **Confusion Matrix**
   - A **confusion matrix** helps evaluate a classification model's performance by comparing the predicted and actual values.
     - **True Positive (TP)**: Predicted “yes” and actual “yes”.
     - **True Negative (TN)**: Predicted “no” and actual “no”.
     - **False Positive (FP)**: Predicted “yes” but actual “no” (Type I error).
     - **False Negative (FN)**: Predicted “no” but actual “yes” (Type II error).
   - Metrics calculated from the confusion matrix include:
     - **Accuracy**: (TP + TN) / Total predictions.
     - **Error Rate**: The rate of incorrect predictions, calculated as (FP + FN) / Total predictions.

By using Keras and TensorFlow with techniques like normalization, this ANN model can predict customer retention effectively. Metrics from the confusion matrix will allow you to evaluate and improve the model's performance, ensuring it accurately identifies patterns to make reliable predictions.
