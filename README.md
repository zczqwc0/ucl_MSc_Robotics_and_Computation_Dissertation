# Integrating Learned Motion Predictions into Factor Graph Optimization for Robot Pose Estimation

## Description
This study focuses on exploring the integration of deep learning techniques with factor graphs for robot state estimation. By learning the information regarding the estimation of relative transformation, observation, and noise covariance from a neural network, these predictions are then fed into a factor graph for final graphical optimization to localize the global robot trajectory.

##  Preparation: Setting up a Python Virtual Environment

Before installing the required packages, it's recommended to create a Python virtual environment. This helps avoid conflicts with other installed packages and allows for a clean workspace. To create a virtual environment

To set up the environment for this project, follow these steps:
1. Create a Python virtual environment:
```bash
python -m venv venv
source venv/bin/activate # Linux
```

## Installation
```bash
pip install pandas tensorflow keras scikit-learn numpy matplotlib
```

## Usage
Follow these steps to run the project:
1. Run the simulation script `simu.py` to collect datasets:
- 60,000 training samples with Gaussian noise distribution in the process and measurement model.
- 12,000 non-Gaussian noise samples for the test set.
- 12,000 Gaussian noise samples for the baseline test set.
2. Train the model using `train_nn.py`
3. Test the model using `test_nn.py`:

