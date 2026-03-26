# CMPE 258 Assignment 3 – Neural Network Implementations for Nonlinear Regression

This repository contains my work for CMPE 258 Assignment 3.  
In this assignment, I implemented the same nonlinear regression problem using different approaches across NumPy, PyTorch, PyTorch Lightning, and TensorFlow.

The main goal of this assignment was to understand how a 3-layer neural network can be built at different abstraction levels, starting from fully manual implementations and then moving toward higher-level deep learning frameworks.

I used a synthetic dataset with 3 input variables and a nonlinear target equation. Across the notebooks, I trained models, tracked loss over epochs, and compared actual vs predicted outputs to see how well each version learned the pattern in the data.

---

## Repository Contents

### 1. Colab A – NumPy / From Scratch
In this notebook, I built a 3-layer neural network for nonlinear regression from scratch using NumPy-style logic.  
I manually implemented:
- forward propagation
- backpropagation
- chain rule based gradient updates
- loss calculation
- parameter updates

I also used `tensorflow.einsum` in the layer computations as required.  
This notebook helped me understand what is happening internally inside a neural network instead of relying on built-in layers.

**Notebook:** `CMPE258_NumpyPytorch_Colab1.ipynb`  
**Video Walkthrough:** *Add your link here*

---

### 2. Colab B – PyTorch From Scratch
In this notebook, I implemented the same 3-layer nonlinear regression model in PyTorch, but without using built-in layer modules like `nn.Linear`.  
I manually handled:
- weight initialization
- forward pass
- loss computation
- backpropagation logic
- parameter updates

This version shows how PyTorch tensors can still be used in a low-level way while keeping more control over the model structure.

**Notebook:** `CMPE258_NumpyPytorch_Colab2.ipynb`  
**Video Walkthrough:** *Add your link here*

---

### 3. Colab C – PyTorch Using Built-in Modules
In this notebook, I built the same nonlinear regression model using PyTorch’s built-in `nn.Module` and `nn.Linear` functionality.  
Compared to the from-scratch version, this one is much cleaner and shorter because PyTorch handles a lot of the layer setup and automatic differentiation for us.

This notebook helped me see the difference between low-level implementation and using framework-supported modules.

**Notebook:** `CMPE258_NumpyPytorch_Colab3.ipynb`  
**Video Walkthrough:** *Add your link here*

---

### 4. Colab D – PyTorch Lightning Version
In this notebook, I implemented the same regression problem using PyTorch Lightning.  
The main purpose here was to see how Lightning reduces boilerplate by organizing the model, training step, validation step, and optimizer configuration in a more structured way.

This version is useful because it keeps the code cleaner and makes the training workflow easier to manage.

**Notebook:** `CMPE258_NumpyPytorch_Colab4.ipynb`  
**Video Walkthrough:** *Add your link here*

---

### 5. Colab E – TensorFlow Variants
In this notebook, I implemented the same nonlinear regression problem in multiple TensorFlow styles:

- low-level TensorFlow
- TensorFlow Sequential API
- TensorFlow Functional API
- TensorFlow subclassed model

This notebook helped me compare how the same problem can be solved at different levels of abstraction in TensorFlow.  
The low-level version gave more control, while the higher-level versions made the code shorter and easier to manage.

**Notebook:** `CMPE258_NumpyPytorch_Colab5.ipynb`  
**Video Walkthrough:** *Add your link here*

---

## Dataset / Problem Setup

For this assignment, I used a synthetic nonlinear regression dataset created using 3 input variables.  
The target values were generated using a nonlinear equation along with a small amount of noise to make the problem more realistic.

This allowed me to use the same regression setup across all frameworks and compare how each implementation performed.

---

## What is shown in each notebook

Each notebook includes:
- data generation
- model building
- training process
- loss tracking across epochs
- final predictions
- output visualizations
- comparison of actual vs predicted values

Some notebooks also include additional metrics like MAE along with MSE.

---

## Main Learning Outcome

This assignment helped me understand the difference between:
- building a neural network completely from scratch
- using framework-level tensor operations
- using built-in modules and APIs
- using higher-level training abstractions like PyTorch Lightning

Doing the same problem in multiple ways made it easier to understand what the frameworks are doing behind the scenes.

---

## How to Run

1. Open any notebook in Google Colab or Jupyter Notebook
2. Run all cells in order
3. Make sure the required libraries are installed
4. View the training output, loss plots, and prediction plots

---

## Submission Notes

- All notebooks were executed and saved with outputs
- Video walkthroughs were recorded for each notebook
- Each video explains the main code sections and final outputs

---

## Files in this Repository

- `CMPE_258_NumpyPytorch_Colab1.ipynb`
- `CMPE_258_NumpyPytorch_Colab2.ipynb`
- `CMPE_258_NumpyPytorch_Colab3.ipynb`
- `CMPE_258_NumpyPytorch_Colab4.ipynb`
- `CMPE_258_NumpyPytorch_Colab5.ipynb`

---

## Author
Nikita Memane
