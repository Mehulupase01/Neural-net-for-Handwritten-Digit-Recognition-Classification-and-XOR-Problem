# Neural net for Handwritten Digit Recognition, Classification and XOR Problem
 This project covers the implementation of distance-based classifiers, multi-class perceptrons, and neural networks for the MNIST dataset (handwritten digit recognition) and the XOR problem. Tasks include dimensionality reduction, nearest mean classification, K-Nearest Neighbor (KNN) classification, multi-class perceptron training, and building a neural network from scratch using gradient descent.

# Classification and Neural Network Implementation for Handwritten Digit Recognition and XOR Problem

This project implements various machine learning algorithms for classifying handwritten digits from the **MNIST dataset** and solving the **XOR problem**. The tasks involve distance-based classifiers, multi-class perceptron training, and the development of a neural network using gradient descent.

## Overview

The project is split into three main tasks:

1. **Data Dimensionality and Distance-Based Classifiers**:
   - Apply dimensionality reduction techniques (PCA, UMAP, t-SNE) to visualize the **MNIST dataset**.
   - Implement a **Nearest Mean Classifier** and a **K-Nearest Neighbor (KNN)** classifier for handwritten digit recognition.
   - Compare the performance of both classifiers using confusion matrices.

2. **Multi-Class Perceptron**:
   - Implement a multi-class perceptron from scratch to classify the **MNIST dataset**.
   - Train the perceptron on the training set and evaluate its performance on the test set.
   - Experiment with different weight initializations and learning rates.

3. **Neural Network for XOR Problem**:
   - Implement a neural network from scratch to solve the **XOR problem** using gradient descent.
   - Train the network with sigmoid activation functions and experiment with different initializations and learning rates.

### Key Tasks:
1. **Task 1**: Data dimensionality reduction and distance-based classification for MNIST.
   - Visualize the data using **PCA**, **UMAP**, and **t-SNE**.
   - Implement **Nearest Mean Classifier** and **KNN** and evaluate performance using confusion matrices.

2. **Task 2**: Multi-class perceptron implementation for the **MNIST dataset**.
   - Train the perceptron and evaluate accuracy on both training and test sets.
   - Tune hyperparameters (learning rates, weight initialization) and plot loss/accuracy.

3. **Task 3**: Implement a neural network to solve the **XOR problem** using **gradient descent**.
   - Implement a simple 3-layer neural network with sigmoid activation.
   - Experiment with learning rates and weight initialization strategies.

## Code Structure

**`Group32_IDL_Assignment0.ipynb`**: A Jupyter notebook for experimenting with data dimensionality, classifier training, and visualizations.

### Libraries Used:
- **numpy**: For mathematical operations.
- **scikit-learn**: For KNN classification, PCA, and t-SNE.
- **matplotlib**: For plotting visualizations.
- **pandas**: For data handling and manipulation.

## Output

- **Task 1 Output**: Visualizations of the MNIST dataset using PCA, UMAP, and t-SNE. Classifier performance shown through confusion matrices for both **Nearest Mean** and **KNN** classifiers.
  
Example output for KNN confusion matrix:
 ```
Confusion Matrix for KNN: 0 1 2 3 4 5 6 7 8 9 0 318 0 1 0 0 0 0 0 0 0 1 0 252 0 0 0 0 0 0 0 0 2 2 4 189 1 1 0 0 4 0 1 ...

 ```

- **Task 2 Output**: Accuracy and loss values for the multi-class perceptron on both the **train** and **test** datasets.

Example output for perceptron accuracy:

```
Epoch 10: Training Accuracy = 97%, Test Accuracy = 86%
```

- **Task 3 Output**: The loss and accuracy of the XOR neural network across multiple training epochs.

## Results & Discussion

- **Task 1**: Visualizations with **PCA**, **UMAP**, and **t-SNE** provided insight into how the digits are distributed in high-dimensional space. The **KNN classifier** performed better than the **Nearest Mean Classifier** with a higher accuracy on both the training and test sets.
  
- **Task 2**: The multi-class perceptron achieved an accuracy of 97% on the training set and 86% on the test set after 10 epochs. Hyperparameter tuning was performed to optimize the learning rate and weight initialization.

- **Task 3**: The XOR neural network achieved convergence using **sigmoid** activation functions. The network was most stable with **sigmoid** and **tanh**, and the best learning rate was found to be 0.15.

## Conclusion

This project demonstrates the implementation and evaluation of various machine learning techniques, including distance-based classification, multi-class perceptron, and neural networks. The results highlight the power of **KNN** and **perceptron** for classification tasks, and the **neural network** was successfully implemented to solve the XOR problem.

## References

1. **MNIST Dataset**: http://yann.lecun.com/exdb/mnist/
2. **Perceptron**: Rosenblatt, F. (1958). The Perceptron: A Perceiving and Recognizing Automaton. Report 85-460-1, Cornell Aeronautical Laboratory.
3. **Backpropagation**: Rumelhart, D. E., Hinton, G. E., & Williams, R. J. (1986). Learning Representations by Backpropagating Errors. Nature.