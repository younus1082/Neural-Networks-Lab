# Single Layer Perceptron (From Scratch)

**Course:** CSE 422 - Neural Networks (Spring 2026)
**Assignment:** Lab Assignment 1
**Language:** Python 3 (Pure)

## Project Overview
This repository contains a **Single Layer Perceptron** implemented entirely from scratch using standard Python. It solves a binary classification problem to predict whether a student will **Pass (1)** or **Fail (0)**.

Per the assignment strict constraints, this project **does not use** any machine learning libraries (NumPy, Pandas, Scikit-Learn, PyTorch, or TensorFlow). It relies solely on Python's built-in lists, loops, and math operations.

## Problem Statement
The model predicts a student's result based on two input features:
1.  **Study Hours per Day**
2.  **Class Attendance Percentage**

### Dataset Logic
A custom dataset was generated using the following rule:
> A student **Passes (1)** if: `(Study Hours * 8) + Attendance > 120`
> Otherwise, the student **Fails (0)**.

This creates a linearly separable dataset suitable for a single-layer perceptron.

## Features
* **Zero Dependencies:** No `pip install` required for ML libraries.
* **Manual Backpropagation:** Implements the Perceptron Learning Rule to update weights and bias manually.
* **Step Activation Function:** Uses a simple threshold activation.
* **Interactive Testing:** Allows users to input their own data after training to see predictions.
* **Training Metrics:** Tracks loss and accuracy per epoch (Bonus Task) 

## How to Run
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/younus1082/Neural-Networks-Lab
    cd https://github.com/younus1082/Neural-Networks-Lab
    ```

2.  **Run the script:**
    ```bash
    python Younus_1082_A2_la1.py
    ```

## Usage Example
Once the training converges (usually within 100 epochs), the program will ask for input.

**Input Format:** `[Study Hours], [Attendance %]`

```text
--- System Ready for User Input ---

Enter [Hours, Attendance] (or 'q' to quit): 8, 90
>> Result: PASS. (Model predicts student will pass)

Enter [Hours, Attendance] (or 'q' to quit): 2, 50
>> Result: FAIL. (Model predicts student will fail)
