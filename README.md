# Simple Two-Layer Neural Network for MNIST Classification

This project demonstrates a two-layer neural network built from scratch using Python and NumPy, designed to classify handwritten digits from the MNIST dataset. The neural network consists of ReLU and Softmax activations and is trained using backpropagation and gradient descent.

## Sample Iamges

![Screenshot 2024-11-04 124428](https://github.com/user-attachments/assets/1e84594d-d1c0-4399-9eb5-712ed470ba70) ![Screenshot 2024-11-04 124455](https://github.com/user-attachments/assets/925232de-72d4-4712-a140-e8aa41ecfcbe)


## Table of Contents

- [Project Overview](#project-overview)
- [Code Structure](#code-structure)
- [Examples](#examples)
- [License](#license)

## Project Overview

This project aims to implement a simple, fully-connected neural network from scratch without using any high-level deep learning libraries. It includes:
- Loading and preprocessing the MNIST dataset
- Building a neural network with two layers
- Training the model using gradient descent
- Testing the model’s performance on unseen data
- Visualizing predictions for sample images

## Code Structure

mnist-neural-network/
│
├── neural_network_mnist.py  
├── README.md                
├── images/                  
└── LICENSE                  

## Examples

# After running the model, you should see output like this:

  Cost after iteration 0: 0.230267 | Accuracy: 9.28%
  Cost after iteration 10: 0.229518 | Accuracy: 12.83%
  Cost after iteration 20: 0.223094 | Accuracy: 31.83%
  Cost after iteration 30: 0.185379 | Accuracy: 52.04%
  Cost after iteration 40: 0.123359 | Accuracy: 67.94%
  Cost after iteration 50: 0.089636 | Accuracy: 76.24%
  Cost after iteration 60: 0.071945 | Accuracy: 81.13%
  Cost after iteration 70: 0.061373 | Accuracy: 83.74%
  Cost after iteration 80: 0.056556 | Accuracy: 83.74%
  Cost after iteration 90: 0.056280 | Accuracy: 81.99%
  Cost after iteration 100: 0.047166 | Accuracy: 86.86%
  Cost after iteration 110: 0.044446 | Accuracy: 87.67%
  Cost after iteration 120: 0.042518 | Accuracy: 88.22%
  Cost after iteration 130: 0.041001 | Accuracy: 88.57%
  Cost after iteration 140: 0.039766 | Accuracy: 88.89%
  Cost after iteration 150: 0.038738 | Accuracy: 89.13%
  Cost after iteration 160: 0.037867 | Accuracy: 89.40%
  Cost after iteration 170: 0.037117 | Accuracy: 89.60%
  Cost after iteration 180: 0.036461 | Accuracy: 89.80%
  Cost after iteration 190: 0.035882 | Accuracy: 89.91%
  Cost after iteration 200: 0.035363 | Accuracy: 90.01%

# To visualize a prediction for a sample image, you can use:

  sample_img = X_test[:, 2319]
  cache, A2 = forward_propagation(sample_img.reshape(-1, 1), trained_params)
  predicted_label = np.argmax(A2, axis=0)
  visualize_prediction(sample_img, predicted_label)


## License 

This project is licensed under the MIT License. See the LICENSE file for details.

