---
layout: post
title: code example
---

# code example


```python
import math
```

a textbox to explain the code


```python
def a_function(a,b):
    return math.sqrt(a) + b**2
```

show function output


```python
a_function(10,20)
```




    403.1622776601684



# pandas example


```python
import pandas as pd
```


```python
df = pd.DataFrame({'a':[35,63,21,58,84]})
df['b'] = df.a.cumsum()
df['b^2'] = df['b']**2
df['c'] = df['b^2'].map(lambda x: a_function(x,0))
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>a</th>
      <th>b</th>
      <th>b^2</th>
      <th>c</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>35</td>
      <td>35</td>
      <td>1225</td>
      <td>35.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>63</td>
      <td>98</td>
      <td>9604</td>
      <td>98.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>21</td>
      <td>119</td>
      <td>14161</td>
      <td>119.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>58</td>
      <td>177</td>
      <td>31329</td>
      <td>177.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>84</td>
      <td>261</td>
      <td>68121</td>
      <td>261.0</td>
    </tr>
  </tbody>
</table>
</div>


