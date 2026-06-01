Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np
arr = np.array([[1, 2, 3],[4, 5, 6],[7, 8, 9]])
new_col = np.array([10, 11, 12])
arr_deleted = np.delete(arr, 1, axis=1)
updated_arr = np.insert(arr_deleted, 1, new_col, axis=1)
print("Original Array:\n", arr)
print("\nUpdated Array (Second column replaced):\n", updated_arr)
```

## Output
<img width="1919" height="686" alt="Screenshot 2026-06-01 233850" src="https://github.com/user-attachments/assets/780ab105-8a2a-46a1-a839-107080ca4423" />

## Result
The program successfully deletes the second column of the array and inserts a new column in its place.
