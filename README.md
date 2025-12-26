# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np
d=eval(input())
arr=np.array(d)
print("Given array")
print(f" {arr}")

print(f"\n{np.sort(arr,axis=0)}")
```

## Output
![502982354-5873a7b9-1bf4-4fe1-9ea7-5bbe07b48f25](https://github.com/user-attachments/assets/9db882c3-b51a-4ae4-b83c-44eb9520069b)

## Result
The program successfully accepts a 2D array from the user, sorts each column in ascending order, and prints both the original and column-wise sorted arrays using NumPy.

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
x=eval(input())
y=eval(input())
a=np.array(x)
b=np.array(y)
pos=np.where(a>b)
posequal=np.where(a==b)
print(pos)
print(posequal)
```
## Output
![502982485-9f862645-3f77-4f3e-aff6-6bce60edb027](https://github.com/user-attachments/assets/abdbb094-a927-4826-ac5f-3334c1172300)

## Result
The program successfully finds the indices where elements in array x are greater than or equal to their corresponding elements in array y. #NumPy Program: Replace the Second Column in a 2D Array

# NumPy Program: Replace the Second Column in a 2D Array

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
val=eval(input())
arr=np.array(val)
print("Printing Input Array")
print(arr)
print("\nPrinting array of items in the third column from all rows")
print(arr[:,2])
```
## Output
![502982919-eef449ba-c2e9-4e3c-b027-5750899fd220](https://github.com/user-attachments/assets/76ce14fa-e318-4271-93bf-ece102cfac84)

## Result
The program successfully takes a 2D NumPy array, deletes the second column (index 1), and inserts a new column at the same position.

# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import pandas as pd
l1=eval(input())
df=pd.DataFrame(l1)
print(df)
```

## Output
![502983171-dfcbc004-050b-44f0-b1a4-47c3fbc4961a](https://github.com/user-attachments/assets/80c95397-a6c7-4163-93ca-780ddf14cc05)

## Result
The program successfully creates a Pandas DataFrame from a dictionary and applies custom index labels. The DataFrame displays all columns (name, score, attempts, qualify) along with the specified row indices (a, b, c, d, e). ``# 🧪 Pandas Program: Join Two DataFrames Along Rows

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
df1=pd.DataFrame({
    's_id':['S1','S2','S3','S4','S5'],
    'name':['Dan','Ryder','Bryce','Bernal','Kwame'],
    'marks':[200, 210, 190, 222,199]
})
df2=pd.DataFrame({
    's_id':['S4','S5','S6','S7','S8'],
    'name':['Scart','Willy','Dani','Kaise','Madeeha'],
    'marks':[201,200,198,219,201]
})
res=pd.concat([df1,df2],axis=0)
print("Original DataFrames:")
print(df1)
print("-------------------------------------")
print(df2)
print()
print("Join the said two dataframes along rows:")
print(res)
```

## Output
![502983384-c6a92bd3-519d-4d9b-b166-08d1702aa609](https://github.com/user-attachments/assets/31cdc968-eb8e-4f17-a734-9e3a2939047b)

## Result
The program successfully join two DataFrames along rows (row-wise concatenation) and assign all data to a new DataFrame.
