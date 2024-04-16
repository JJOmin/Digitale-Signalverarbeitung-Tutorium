# **Vektoralgebra wiederholung**

1. **Elementweise Multiplikation**:
   Bei der elementweisen Multiplikation werden die entsprechenden Elemente der Arrays paarweise multipliziert.

   ```python
   import numpy as np
   
   array1 = np.array([0, 1, 3])
   array2 = np.array([5, 8, 11, 4])
   
   elementwise_product = array1 * array2[:len(array1)]  # Nur die ersten 3 Elemente von array2 verwenden
   print(elementwise_product)  # Ausgabe: [0, 8, 33]
   ```
2. **Matrixmultiplikation**:
   Bei der Matrixmultiplikation wird das Skalarprodukt der Zeilen der ersten Matrix und der Spalten der zweiten Matrix berechnet.

   ```python
   import numpy as np
   matrix1 = np.array([[0, 1, 3]])
   matrix2 = np.array([[5],
                       [8],
                       [11]])
   print(matrix1 @ matrix2) # Ausgabe: [[41]]
   ```
3. **Inneres Produkt (Skalarprodukt)**:
   Das innere Produkt ist die Summe der Produkte der entsprechenden Elemente der Vektoren.

   ```python
   np.dot([0,1,3], [5,8,11]) # Ausgabe  41
   print( np.array([0,1,3]) @  np.array([5,8,11])) # Ausgabe  41
   ```
4. **Äußeres Produkt**:
   Das äußere Produkt zwischen zwei Vektoren ergibt eine Matrix, in der das Element an der i-ten Zeile und j-ten Spalte das Produkt des i-ten Elements des ersten Vektors und des j-ten Elements des zweiten Vektors ist. Dies ist nicht direkt mit Python-Arrays darstellbar, aber hier ist eine Möglichkeit, dies zu berechnen:

   ```python
   outer_product = np.outer([0,1,3], [5,8,11])
   print(outer_product)
   # Ausgabe:
   #[[ 0  0  0]
   # [ 5  8 11]
   # [15 24 33]]
   ```
5. **Skalarprodukt**:
   Das Skalarprodukt ist eine spezielle Form des inneren Produkts, bei dem die Vektoren denselben Raum teilen.

   ```python
   np.inner([0,1,3], [5,8,11]) # Ausgabe  41
   np.dot([0,1,3], [5,8,11]) # Ausgabe  41
   np.array([0,1,3]) @  np.array([5,8,11]) # Ausgabe  41
   ```
6. **Kreuzprodukt**:
   Das Kreuzprodukt ist eine Operation, die für Vektoren im dreidimensionalen Raum definiert ist und einen Vektor ergibt, der senkrecht zu den Ausgangsvektoren steht.

   ```python
   np.cross([0,1,3], [5,8,11]) # Ausgabe: [-13  15  -5]
   ```