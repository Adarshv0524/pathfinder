# Pathfinder 

This project implements a machine learning model designed to find the optimized route for mail or parcel delivery. It takes into account various factors, including the amount, time, date, and location of the delivery.



## Prerequisites

Before you get started, ensure you have the following installed:
- **Python** (version 3.6 or higher). You can download it from the [official Python website](https://www.python.org/downloads/).
- **pip**, which comes bundled with Python, for managing Python packages.

## Installation and Setup

Follow the steps below to set up the project and create a virtual environment for managing dependencies.

### Command Prompt
1. Open **Command Prompt**.
2. Navigate to your project directory:
   ```bash
   cd path\to\your\pathfinder
   ```
3. Create a virtual environment named `pathfinder-venv`:
   ```bash
   virtualenv pathfinder-venv
   ```
4. Activate the virtual environment:
   ```bash
   pathfinder-venv\Scripts\activate
   ```

### PowerShell
1. Open **PowerShell**.
2. Navigate to your project directory:
   ```powershell
   cd path\to\your\pathfinder
   ```
3. Create the virtual environment:
   ```powershell
   virtualenv pathfinder-venv
   ```
4. Activate the virtual environment:
   ```powershell
   pathfinder-venv\Scripts\Activate.ps1
   ```

### Git Bash
1. Open **Git Bash**.
2. Navigate to your project directory:
   ```bash
   cd /d/sih/pathfinder
   ```
3. Create the virtual environment:
   ```bash
   virtualenv pathfinder-venv
   ```
4. Activate the virtual environment:
   ```bash
   source pathfinder-venv/Scripts/activate
   ```

## Deactivating the Virtual Environment

To exit the virtual environment at any time, simply run:
```bash
deactivate
```



# Build model to be consider


## Best Choices

### 1 . Random Forest
construct multible decision trees during training and outputs 
- Accuracy 80-90 percentage
- Robustness to overfitting makes it suitable for datasets with complex feature interactions and high dimensionality
- Ideal for capturing the non-linear relationships between features such as transit times, costs, and distances due to its multiple tree structure.

### 2. XGBoost 
XGBoost( Extreme Gradint Boosting) is implementation of gradient boosting that improves on traditional boosting methods with regularization and tree pruning.
- Accuracy : around 90% 
- Well-suited for optimizing routes where precise prediction of delivery times and costs is essential, leveraging its ability to handle various types of data, including missing value.

### 3. GBM (Gradient Boosting Machine)
Construct decision trees sequentially , where each tree corrects error made by the previous ones
- Accuracy : around 80-90%


## Avoid 

K-NN 
Linear Regression