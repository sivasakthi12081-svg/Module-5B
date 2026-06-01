# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd
student_data1 = {
    'name': ['Arun', 'Bala'],
    'marks': [85, 90]
}
student_data2 = {
    'name': ['Cathy', 'David'],
    'marks': [88, 92]
}
df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)
result = pd.concat([df1, df2], axis=0)
print(result)
```

## Output
<img width="1919" height="773" alt="Screenshot 2026-06-01 234423" src="https://github.com/user-attachments/assets/2588bdcc-494f-4131-a7a3-66c9dc8f6672" />

## Result
The two DataFrames are successfully joined row-wise using pd.concat() with axis=0.
