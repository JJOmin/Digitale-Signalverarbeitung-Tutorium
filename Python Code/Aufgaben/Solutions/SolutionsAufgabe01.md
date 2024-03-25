# Lösungen für die Aufgabe 01
- Erstelle ein 1D-Array mit den Werten [1, 2, 3, 4, 5].
   ```python 
  import numpy as np
  array_a = np.array([1, 2, 3, 4, 5])
  print(array_a)
  ```
- Erstelle ein 2D-Array mit den Werten [[1, 2], [3, 4], [5, 6]].
  ```python 
  array_b = np.array([[1, 2], [3, 4], [5, 6]])
  print(array_b)
  ```
- Erstelle ein 3x3-Array mit Nullen mit "np.zeros".
  ```python
  array_c = np.zeros((3, 3))
  print(array_c)
  ```
- Erstelle ein 4x2-Array mit Einsen mit "np.ones".
  ```python
  array_d = np.ones((4, 2))
  print(array_d)
  ```
- Was macht"np.arange"?
  ```python
  print(np.arange(1,16))
  >>> [ 1  2  3  4  5  6  7  8  9 10 11 12 13 14 15]
  ```
  

## Hinweise:
- NumPy for beginners [hier](https://numpy.org/doc/stable/user/absolute_beginners.html)
