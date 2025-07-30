# Perceptron Interactive Demo

An interactive web-based visualization of how a perceptron (single-layer neural network) learns to classify data points into two classes. This educational tool demonstrates the fundamental concepts of machine learning through hands-on interaction.

## What is a Perceptron?

A perceptron is the simplest form of a neural network, consisting of a single neuron that can learn to classify data into two categories. It was one of the first machine learning algorithms and forms the foundation for understanding more complex neural networks.

## Features

### Interactive Training
- **Click to Add Points**: Select a class (Blue or Red) and click on the canvas to add training data
- **Real-time Visualization**: Watch the decision boundary form and adjust as the perceptron learns
- **Training Controls**: Train step-by-step or clear all data to start over

### Visual Feedback
- **Decision Boundary**: See the line that separates the two classes
- **Background Coloring**: Visual regions show how the perceptron classifies different areas
- **Training Statistics**: Monitor epochs, accuracy, and point count in real-time

### Testing Mode
- **Test New Points**: Switch to test mode to evaluate how well the trained perceptron classifies new data
- **Immediate Feedback**: See predictions instantly with visual indicators

### Educational Display
- **Weight Visualization**: View the current weights (w₁, w₂) and bias values
- **Training Log**: Follow the learning process with detailed epoch-by-epoch progress
- **Mathematical Formula**: See the decision function: `output = sign(w₁×x + w₂×y + bias)`

## How to Use

1. **Open `index.html`** in a web browser
2. **Add Training Data**:
   - Select "Class 0 (Blue)" or "Class 1 (Red)"
   - Click on the canvas to add points of that class
   - Add several points of each class in different areas
3. **Train the Perceptron**:
   - Click "Train Perceptron" to start the learning process
   - Watch the training log to see convergence progress
   - Observe how the decision boundary adjusts to separate the classes
4. **Test the Model**:
   - Click "Test Mode" after training
   - Click anywhere on the canvas to see how the perceptron classifies new points
5. **Experiment**:
   - Try different data distributions
   - See how the perceptron handles linearly separable vs. non-separable data
   - Use "Clear All" to start with new data

## Technical Details

### Algorithm
- **Learning Rule**: Classic perceptron learning algorithm
- **Learning Rate**: 0.1 (fixed)
- **Activation Function**: Sign function (step function)
- **Coordinate System**: Normalized to [-1, 1] range for training

### Decision Function
```
output = sign(w₁ × x + w₂ × y + bias)
```
Where:
- `w₁, w₂` are the learned weights
- `x, y` are the input coordinates
- `bias` is the learned bias term
- `sign()` returns 1 for positive values, 0 for negative

### Implementation
- **Pure JavaScript**: No external dependencies
- **HTML5 Canvas**: For interactive visualization
- **Responsive Design**: Works on desktop and mobile devices
- **Real-time Updates**: Immediate visual feedback during training

## Educational Value

This demo helps you understand:
- How perceptrons learn through iterative weight updates
- The concept of linear separability in machine learning
- The relationship between weights, bias, and decision boundaries
- Why some data patterns can't be learned by a single perceptron
- The foundation concepts that lead to multi-layer neural networks

## Browser Compatibility

Works in all modern web browsers that support HTML5 Canvas and ES6 JavaScript features.

## Getting Started

Simply download the repository and open `index.html` in your web browser. No installation or build process required!
