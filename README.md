# Machine Learning: Advice for Applying Machine Learning (Practice Lab)

This repository contains the practical lab exercises and code for the **Advice for Applying Machine Learning** module from the DeepLearning.AI Machine Learning Specialization (**Advanced Learning Algorithms** course).

##  Exercises Completed

The following 5 core functions and neural network models were successfully implemented and tested:

### 1. Mean Squared Error (MSE) for Linear Regression
* **Function:** `eval_mse(y, yhat)`
* **Description:** Calculates the mean squared error between target values (`y`) and predicted values (`yhat`) for a linear regression model.

### 2. Categorization Error Calculation
* **Function:** `eval_cat_err(y, yhat)`
* **Description:** Calculates the fraction of incorrect predictions (categorization error) for multi-class classification models.

### 3. Complex Neural Network Model
* **Model:** `model`
* **Description:** A 3-layer neural network architecture designed for complex classification:
  * Dense layer with 120 units (`relu` activation)
  * Dense layer with 40 units (`relu` activation)
  * Output dense layer with 6 units (`linear` activation)
* **Compilation:** `SparseCategoricalCrossentropy(from_logits=True)` loss function and `Adam` optimizer (learning rate = 0.01).

### 4. Simple Neural Network Model
* **Model:** `model_s`
* **Description:** A 2-layer simple neural network architecture:
  * Dense layer with 6 units (`relu` activation)
  * Output dense layer with 6 units (`linear` activation)
* **Compilation:** `SparseCategoricalCrossentropy(from_logits=True)` loss and `Adam` optimizer (learning rate = 0.01).

### 5. Regularized Neural Network Model
* **Model:** `model_r`
* **Description:** A 3-layer neural network implementing L2 regularization to prevent overfitting:
  * Uses `kernel_regularizer=tf.keras.regularizers.l2(0.1)` on hidden layers.
  * Output dense layer with 6 units (`linear` activation).
* **Compilation:** `SparseCategoricalCrossentropy(from_logits=True)` loss and `Adam` optimizer (learning rate = 0.01).

##  Technologies Used
* **Python**
* **TensorFlow / Keras**
* **NumPy**
* **Scikit-Learn**
* **Matplotlib**

