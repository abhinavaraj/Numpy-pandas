# NumPy & Pandas Learning Repository 📊🐍

This repository contains examples, notes, and practice code for learning **NumPy** and **Pandas**, two of the most powerful Python libraries for data analysis and manipulation.  

---

## 🚀 About the Project
- **NumPy** provides fast mathematical operations on arrays and matrices.  
- **Pandas** offers easy-to-use data structures like `Series` and `DataFrame` for handling structured data.  

This repo is aimed at beginners and intermediate learners who want to strengthen their Python data analysis skills.

---

## 📂 Repository Structure
├── numpy/
│ ├── basics.py # Array creation, indexing, slicing
│ ├── operations.py # Arithmetic, broadcasting, functions
│ └── matrix.py # Linear algebra, dot product, transpose
│
├── pandas/
│ ├── series.py # Pandas Series basics
│ ├── dataframe.py # DataFrame creation & manipulation
│ ├── cleaning.py # Handling missing data, duplicates
│ └── analysis.py # GroupBy, merge, join, pivot
│
└── README.md

markdown
Copy code

---

## 📖 Topics Covered

### 🔹 NumPy
- Array creation (`np.array`, `np.zeros`, `np.ones`, `np.arange`, `np.linspace`)
- Indexing & slicing
- Broadcasting
- Universal functions (ufuncs)
- Aggregations (`sum`, `mean`, `std`, etc.)
- Linear algebra (`dot`, `transpose`, `inverse`)

#### ✅ Sample Code
```python
import numpy as np

# Create arrays
arr = np.array([1, 2, 3, 4, 5])
zeros = np.zeros((2, 3))
ones = np.ones((3, 3))

# Operations
print("Array:", arr)
print("Mean:", arr.mean())
print("Sum:", arr.sum())

# Matrix multiplication
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])
print("Dot product:\n", np.dot(A, B))
🔹 Pandas
Series & DataFrame creation

Importing & exporting data (CSV, Excel, JSON)

Indexing & selection (loc, iloc)

Data cleaning (missing values, duplicates)

Filtering & sorting

GroupBy operations

Merging & joining datasets

Pivot tables

✅ Sample Code
python
Copy code
import pandas as pd

# Create DataFrame
data = {
    "Name": ["Alice", "Bob", "Charlie"],
    "Age": [25, 30, 35],
    "Score": [85, 90, 95]
}
df = pd.DataFrame(data)

# Display
print(df)

# Selection
print(df["Name"])
print(df.loc[0, "Age"])

# Filtering
print(df[df["Score"] > 85])

# GroupBy example
grouped = df.groupby("Age")["Score"].mean()
print(grouped)
🛠️ Installation
Make sure you have Python installed (>=3.8). Then install the required libraries:

bash
Copy code
pip install numpy pandas
📘 Usage
Run Python files directly, for example:

bash
Copy code
python numpy/basics.py
python pandas/dataframe.py
Or open Jupyter Notebook for interactive learning:

bash
Copy code
jupyter notebook
🎯 Learning Resources
NumPy Documentation

Pandas Documentation

Kaggle Learn Pandas

🤝 Contributing
Contributions are welcome! Feel free to:

Add new examples

Fix bugs

Improve explanations

