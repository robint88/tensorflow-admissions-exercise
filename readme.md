# Graduate Admissions Regression Model

This project predicts graduate school admission chances using a neural network implemented in TensorFlow/Keras. It is my first introduction to TensorFlow/Neural Networks.

## Project Overview

- Dataset: `admissions_data.csv` (not included in this repo)
- Task: Regression to predict admission chance
- Features: GRE Score, TOEFL Score, University Rating, SOP, LOR, CGPA, Research
- Label: Chance of Admit

## Steps Taken

1. Loaded and explored the data.
2. Split data into training and test sets.
3. Scaled features using `StandardScaler`.
4. Built a neural network model with Keras:
   - 1 hidden layer with 16 neurons (ReLU)
   - Output layer with 1 neuron (linear activation)
   - Adam optimizer, MSE loss, MAE metric
5. Used EarlyStopping to avoid overfitting.
6. Evaluated performance on the test set using MAE and R².
7. Performed hyperparameter tuning (batch size, learning rate) to improve accuracy.

## Results

- Test MAE: 0.049
- Test MSE: 0.0047
- R² Score: 0.756

> Note: Results may vary depending on random initialization and train/test split.

## Usage

1. Place `admissions_data.csv` in the same directory as the notebook or script.
2. Run the Jupyter notebook or Python script to train and test the model.
3. Modify hyperparameters as desired to explore model performance.

## Files

- `admissions_model.ipynb` – Main notebook with code and plots
- `.gitignore` – Ensures CSV file is not tracked by Git
- `README.md` – Project description
