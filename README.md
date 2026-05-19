# 📊 Pandas Library — Complete Beginner Friendly Guide

![Pandas Banner](https://pandas.pydata.org/static/img/pandas_mark.svg)

## 🚀 Introduction

**Pandas** is one of the most powerful and popular Python libraries used for:

* Data Analysis
* Data Cleaning
* Data Manipulation
* Data Visualization Preparation
* Machine Learning Preprocessing

It provides easy-to-use data structures like:

* **Series** → 1D data
* **DataFrame** → 2D tabular data

Pandas is widely used in:

* Data Science
* Machine Learning
* Artificial Intelligence
* Business Analytics
* Research

---

# 📦 Installation

Install Pandas using pip:

```bash
pip install pandas
```

Check version:

```python
import pandas as pd

print(pd.__version__)
```

---

# 📚 Import Pandas

```python
import pandas as pd
```

---

# 🏗️ Creating Data Structures

## 1️⃣ Series

```python
import pandas as pd

data = [10, 20, 30, 40]

s = pd.Series(data)

print(s)
```

---

## 2️⃣ DataFrame

```python
import pandas as pd

data = {
    "Name": ["Om", "Rahul", "Aman"],
    "Age": [19, 20, 21],
    "City": ["Bhopal", "Delhi", "Mumbai"]
}

df = pd.DataFrame(data)

print(df)
```

---

# 📖 Reading Files

## Read CSV File

```python
df = pd.read_csv("data.csv")
```

## Read Excel File

```python
df = pd.read_excel("data.xlsx")
```

## Read JSON File

```python
df = pd.read_json("data.json")
```

---

# 💾 Saving Files

```python
df.to_csv("output.csv", index=False)
```

```python
df.to_excel("output.xlsx", index=False)
```

---

# 🔍 Viewing Data

## First 5 Rows

```python
df.head()
```

## Last 5 Rows

```python
df.tail()
```

## Shape of Dataset

```python
df.shape
```

## Information About Dataset

```python
df.info()
```

## Statistical Summary

```python
df.describe()
```

---

# 🧹 Data Cleaning

## Check Missing Values

```python
df.isnull().sum()
```

## Remove Missing Values

```python
df.dropna()
```

## Fill Missing Values

```python
df.fillna(0)
```

---

# 🎯 Selecting Data

## Select Single Column

```python
df["Name"]
```

## Select Multiple Columns

```python
df[["Name", "Age"]]
```

## Select Rows Using loc

```python
df.loc[0]
```

## Select Rows Using iloc

```python
df.iloc[0:3]
```

---

# 🔄 Filtering Data

```python
df[df["Age"] > 20]
```

---

# ➕ Adding New Column

```python
df["Salary"] = [25000, 30000, 40000]
```

---

# ❌ Deleting Column

```python
df.drop("Salary", axis=1)
```

---

# 📊 GroupBy Operation

```python
df.groupby("City")["Age"].mean()
```

---

# 🔃 Sorting Data

## Ascending Order

```python
df.sort_values("Age")
```

## Descending Order

```python
df.sort_values("Age", ascending=False)
```

---

# 🔗 Merging DataFrames

```python
pd.merge(df1, df2, on="ID")
```

---

# 📈 Pandas With Matplotlib

```python
import matplotlib.pyplot as plt

df["Age"].plot(kind="hist")

plt.show()
```

---

# 🤖 Why Pandas is Important in Machine Learning?

Pandas helps in:

* Cleaning datasets
* Handling missing values
* Feature engineering
* Data preprocessing
* Data analysis
* Preparing data for ML models

---

# ⚡ Advantages of Pandas

✅ Easy to learn
✅ Fast and powerful
✅ Excellent for large datasets
✅ Supports multiple file formats
✅ Works well with NumPy and Matplotlib
✅ Essential for Data Science

---

# 🛠️ Commonly Used Functions

| Function        | Description         |
| --------------- | ------------------- |
| `head()`        | Show first rows     |
| `tail()`        | Show last rows      |
| `info()`        | Dataset information |
| `describe()`    | Statistical summary |
| `shape`         | Dataset dimensions  |
| `dropna()`      | Remove null values  |
| `fillna()`      | Fill null values    |
| `groupby()`     | Group data          |
| `sort_values()` | Sort dataset        |

---

# 📌 Example Mini Project

```python
import pandas as pd

df = pd.read_csv("students.csv")

print(df.head())

print(df.isnull().sum())

df = df.dropna()

average_marks = df["Marks"].mean()

print("Average Marks:", average_marks)
```

---

# 📚 Official Documentation

📖 Pandas Documentation:
[Pandas Official Documentation](https://pandas.pydata.org/docs/?utm_source=chatgpt.com)

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch
3. Make changes
4. Commit your code
5. Submit a Pull Request

---

# ⭐ Support

If you found this project helpful:

⭐ Star the repository
🍴 Fork the project
📢 Share with others

---

# 👨‍💻 Author

Made with ❤️ using Python and Pandas

---

# 🏷️ Hashtags

`#Python` `#Pandas` `#DataScience` `#MachineLearning` `#AI` `#DataAnalysis`

Is there any other problem?
