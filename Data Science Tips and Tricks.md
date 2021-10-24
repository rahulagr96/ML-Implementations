# Data Science Tips and Tricks

## 1. Get Unique Values from a Column in Pandas Data Frame

``` python
penguins_df['species'].unique()
```

## 2. Pop one column and create a new array

```python
y = penguins_df.pop('species').values
```

## 3. Y_pred and Y_actual side by side

``` python
pd.DataFrame(data={'predictions': y_pred, 'actual': y_test})
```

## 4. Confusion Matrix

``` python
import matplotlib.pyplot as plt
from sklearn.metrics import confusion_matrix,accuracy_score,ConfusionMatrixDisplay
cm = confusion_matrix(y_test, y_pred)
ac = accuracy_score(y_test,y_pred)

disp = ConfusionMatrixDisplay(cm)
fig, ax = plt.subplots(figsize=(3,3))
disp.plot(ax=ax)
```

## 5. loc vs iloc

![image-20211022121655744](C:\Users\rahul\AppData\Roaming\Typora\typora-user-images\image-20211022121655744.png)

## 6. Renaming a column

``` python
df = df.rename(columns={"Category":"Pet"})
```

