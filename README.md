
# Day 15 – NumPy Statistical Analysis

## Overview

This project is part of the **VEDA AI & ML Internship – 45 Day AI & ML Track**.

In this task, a numerical student performance dataset is analyzed using **NumPy statistical functions**. The analysis focuses on calculating basic statistical measures and identifying important patterns, including high and low values in the dataset.

## Objective

Analyze a numerical dataset using NumPy statistical functions and identify important patterns in the data.

## Tools Used

- Python
- NumPy
- Jupyter Notebook

## Dataset

A student performance dataset containing the following marks was used:

```python
[65, 72, 88, 91, 56, 78, 84, 95, 67, 73, 89, 45, 82, 76, 93]
````

The dataset contains **15 student marks**.

## Statistical Measures

The following statistical measures were calculated using NumPy:

* Mean
* Median
* Standard Deviation
* Minimum
* Maximum
* Range

## NumPy Functions Used

```python
np.mean()
np.median()
np.std()
np.min()
np.max()
```

## Implementation

### Import NumPy

```python
import numpy as np
```

### Create the Dataset

```python
marks = np.array([65, 72, 88, 91, 56, 78, 84, 95, 67, 73, 89, 45, 82, 76, 93])

marks
```

### Calculate Mean

```python
mean_marks = np.mean(marks)

print("Mean:", mean_marks)
```

### Calculate Median

```python
median_marks = np.median(marks)

print("Median:", median_marks)
```

### Calculate Standard Deviation

```python
std_marks = np.std(marks)

print("Standard Deviation:", std_marks)
```

### Calculate Minimum and Maximum

```python
minimum_marks = np.min(marks)
maximum_marks = np.max(marks)

print("Minimum:", minimum_marks)
print("Maximum:", maximum_marks)
```

### Combined Statistical Analysis

```python
print("Statistical Analysis")
print("--------------------")
print("Mean:", np.mean(marks))
print("Median:", np.median(marks))
print("Standard Deviation:", np.std(marks))
print("Minimum:", np.min(marks))
print("Maximum:", np.max(marks))
```

### Compare Mean and Median

```python
if mean_marks > median_marks:
    print("Mean is greater than the median.")
elif mean_marks < median_marks:
    print("Mean is less than the median.")
else:
    print("Mean and median are equal.")
```

### Identify High and Low Values

For this analysis:

* Marks of **90 or above** are considered high values.
* Marks **below 50** are considered low values.

```python
high_values = marks[marks >= 90]
low_values = marks[marks < 50]

print("High values (90 and above):", high_values)
print("Low values (below 50):", low_values)
```

### Find Highest and Lowest Marks

```python
highest_mark = np.max(marks)
lowest_mark = np.min(marks)

print("Highest mark:", highest_mark)
print("Lowest mark:", lowest_mark)
```

### Calculate Range

```python
data_range = np.max(marks) - np.min(marks)

print("Range:", data_range)
```

## Results

| Statistical Measure | Result |
| ------------------- | -----: |
| Mean                |  76.27 |
| Median              |  78.00 |
| Standard Deviation  |  13.91 |
| Minimum             |     45 |
| Maximum             |     95 |
| Range               |     50 |

## High and Low Values

### High Values

Students scoring **90 or above**:

```text
91, 95, 93
```

There are **3 high values**.

### Low Values

Students scoring **below 50**:

```text
45
```

There is **1 low value**.

## Observations

1. The mean mark is approximately **76.27**, while the median is **78**, showing that the average and middle value are relatively close.
2. The highest mark is **95** and the lowest mark is **45**, resulting in a range of **50 marks**.
3. Three students scored **90 or above**, while one student scored **below 50**.
4. The standard deviation of approximately **13.91** indicates a moderate spread of marks around the mean.
5. Since the mean is slightly lower than the median, the lower marks have a small influence on the average.

## Mean vs Median

The **mean** is calculated by adding all the values and dividing the total by the number of values.

The **median** is the middle value when the dataset is arranged in ascending or descending order.

For this dataset:

```text
Mean   = 76.27
Median = 78.00
```

The median is slightly higher than the mean because the lower values in the dataset reduce the average.

## Understanding Standard Deviation

Standard deviation measures the amount of variation or dispersion in a dataset.

For this dataset:

```text
Standard Deviation ≈ 13.91
```

This indicates that the student marks have a moderate amount of variation around the mean.

A lower standard deviation means that the values are closer to the mean, while a higher standard deviation indicates greater spread.

## Learning Outcomes

Through this task, I learned how to:

* Create numerical datasets using NumPy.
* Calculate mean and median.
* Calculate standard deviation.
* Find minimum and maximum values.
* Calculate the range of a dataset.
* Compare mean and median.
* Identify unusually high and low values.
* Interpret basic statistical patterns.
* Use NumPy statistical functions for numerical data analysis.

## Interview Questions

### 1. What is the difference between mean and median?

The mean is the average of all values in a dataset. The median is the middle value after arranging the data in order.

### 2. When can median be more useful than mean?

The median can be more useful when the dataset contains extreme values or outliers because the median is less affected by unusually high or low values.

### 3. What does standard deviation tell us?

Standard deviation tells us how widely the values are spread around the mean. A lower standard deviation indicates that the values are closer to the mean, while a higher standard deviation indicates greater variation.

## Project Structure

```text
Day-15-NumPy-Statistical-Analysis/
│
├── Day_15_NumPy_Statistical_Analysis.ipynb
└── README.md
```

## Conclusion

This task demonstrated how NumPy can be used for basic statistical analysis of numerical data. By calculating the mean, median, standard deviation, minimum, maximum, and range, useful patterns in the student performance dataset were identified. The analysis also demonstrated how statistical measures can help understand the distribution and variation of numerical data.

## Internship

**VEDA AI & ML Internship – 45 Day AI & ML Track**

**Day 15: NumPy Statistical Analysis**

```
```
