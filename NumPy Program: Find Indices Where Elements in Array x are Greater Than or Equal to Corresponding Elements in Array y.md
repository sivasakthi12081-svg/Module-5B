# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
```
import numpy as np
x = np.array([5, 10, 15, 20])
y = np.array([3, 10, 18, 15])
indices = np.where(x >= y)
print("Array x:", x)
print("Array y:", y)
print("Indices where x >= y:", indices)
```

## Output
<img width="1919" height="712" alt="Screenshot 2026-06-01 233601" src="https://github.com/user-attachments/assets/dec8b91c-e868-4b1a-aee3-ae996330a2b6" />

## Result
The program successfully identified the indices where elements of array x are greater than or equal to those in array y.
The correct index positions were displayed using np.where().
