# Implementing RNNs and Analyzing Gradients

## Overview
This notebook implements a simple Recurrent Neural Network (RNN) layer from scratch using PyTorch, builds an RNN-based regression model, and explores gradient flow dynamics. It includes:
- Custom `RNNLayer` class with forward pass logic
- `RecurrentRegressionModel` for sequence prediction
- Synthetic dataset generation for training/testing
- Gradient analysis tools to inspect RNN behavior


## Usage
1. **RNN Layer Implementation**  
   - Core RNN logic with `nn.Linear` layers
   - Hidden state retention for gradient tracking

2. **Regression Model**  
   - Wrapper model for sequence-to-sequence prediction
   - Linear output layer for regression tasks

3. **Synthetic Data Generation**  
   - `generate_batch()` creates sequences with cumulative averages
   - Interactive visualization of generated sequences

4. **Gradient Analysis**  
   - Retain gradients through hidden states
   - Tools for visualizing gradient flow patterns


## Test Cases
Validation includes:
- Shape checks for outputs
- Numerical stability tests
- Parameter count verification
- Forward pass consistency checks


## Notes
- Gradient analysis helps identify vanishing/exploding gradient issues common in RNNs
- The synthetic dataset tests the model's ability to track temporal dependencies
- Test cases validate numerical implementation correctness
