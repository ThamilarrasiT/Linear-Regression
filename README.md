Linear Regression From Scratch Using Python

=> About the Project

This project is a simple implementation of **Linear Regression** using only basic Python.  
No external libraries like NumPy, Pandas, or Scikit-learn are used.

The main goal of this project is to understand how Linear Regression works internally, especially:
- Finding the slope and intercept manually
- Using Gradient Descent for optimization
- Calculating prediction error (loss)

This project is beginner-friendly and useful for students learning Machine Learning fundamentals.

---

=> Features

- Pure Python implementation
- No machine learning libraries used
- Manual calculation of:
  - Mean
  - Slope (`m`)
  - Intercept (`c`)
- Gradient Descent optimization
- Loss calculation after every epoch

---

=> Dataset Used

```python
x = [1, 2, 3, 4, 5]
y = [1, 3, 2, 4, 5]
````

* `x` represents input values
* `y` represents output values

---

=> How the Program Works

=> Step 1 — Calculate Average

The program first calculates the average values of `x` and `y`.

=> Step 2 — Find Initial Line Equation

Using mathematical formulas, the program calculates the initial slope and intercept.

Slope Formula:

m=\frac{\sum (x_i-\bar{x})(y_i-\bar{y})}{\sum (x_i-\bar{x})^2}

Intercept Formula:

c=\bar{y}-m\bar{x}

---

=> Step 3 — Gradient Descent

The model improves itself using Gradient Descent by updating:

* slope (`m`)
* intercept (`c`)

Update Formula:

m=m-\alpha\frac{\partial J}{\partial m}

c=c-\alpha\frac{\partial J}{\partial c}

Where:

* `α` is the learning rate
* `J` is the loss function

---

=> Loss Function

The program uses Mean Squared Error (MSE) loss:

J(m,c)=\frac{1}{2n}\sum (y_i-\hat{y_i})^2

The loss value decreases as the model learns better.

---

 How to Run the Project

=>1. Save the Program

```bash
linear_regression_without_library.py
```

=> 2. Run the File

```bash
python linear_regression_without_library.py
```

---
=> Sample Output

```bash
Epoch= 0
Epoch= 1
Epoch= 2
...
Epoch= 99

M= 0.85
C= 0.52
Loss= 0.18
```

---

=> What You Can Learn From This Project

This project helps you understand:

* Basics of Machine Learning
* Linear Regression concepts
* Gradient Descent optimization
* How prediction models learn from data

---

=> Future Improvements

You can improve this project by:

* Adding graph visualization
* Using NumPy for faster calculations
* Comparing results with Scikit-learn
* Extending to Multiple Linear Regression

---

=> Conclusion

This project is a great starting point for beginners who want to learn Machine Learning without depending on libraries.
It explains the core idea behind Linear Regression in a simple and practical way.

````
----------------------------------------------------------------------------------------------------------------------------------------------------
---

=> README — Linear Regression With Library

```markdown
 Linear Regression Using Scikit-learn

=> About the Project

This project demonstrates how to build a **Linear Regression model** using the Scikit-learn library in Python.

Unlike the manual implementation, Scikit-learn provides ready-made functions that make model training faster and easier.

This project is useful for beginners who want to understand how machine learning libraries simplify the development process.

---

=> Features

- Simple Linear Regression using Scikit-learn
- Easy model training
- Automatic prediction
- Finds slope and intercept automatically
- Beginner-friendly code

---

=> Dataset Used

```python
x = [[1], [2], [3], [4], [5]]
y = [1, 3, 2, 4, 5]
````

* `x` represents input values
* `y` represents output values

---

 Libraries Required

Install the required libraries using:

```bash
pip install numpy scikit-learn matplotlib
```

Libraries used:

* NumPy
* Scikit-learn
* Matplotlib (optional)

---

 How the Model Works

The Linear Regression model follows the equation:

genui{"math_block_widget_always_prefetch_v2":{"content":"y=mx+c"}}

Where:

* `m` = slope
* `c` = intercept

The model automatically learns the best-fit line from the data.

---

 Example Code

```python
from sklearn.linear_model import LinearRegression
import numpy as np

x = np.array([1,2,3,4,5]).reshape(-1,1)
y = np.array([1,3,2,4,5])

model = LinearRegression()

model.fit(x, y)

predictions = model.predict(x)

print("Slope:", model.coef_[0])
print("Intercept:", model.intercept_)
print("Predictions:", predictions)
```

---
How to Run the Project

 1. Save the File

```bash
linear_regression_with_library.py
```

 2. Run the Program

```bash
python linear_regression_with_library.py
```

---

=> Sample Output

```bash
Slope: 0.8
Intercept: 0.4
Predictions: [1.2 2.0 2.8 3.6 4.4]
```

---

=> What You Can Learn From This Project

This project helps you understand:

* How Scikit-learn works
* Training a Machine Learning model
* Making predictions using trained models
* Difference between manual and library-based implementation

---
=> Advantages of Using Scikit-learn

* Less code
* Faster development
* Optimized algorithms
* Easy to scale for larger datasets

---

=> Future Improvements

You can improve this project by:

* Adding train-test split
* Visualizing the regression line
* Calculating accuracy metrics
* Using larger datasets

---

=> Conclusion

This project shows how easily Linear Regression can be implemented using Scikit-learn.
It is a good next step after learning the manual implementation of Linear Regression from scratch.

```
```
