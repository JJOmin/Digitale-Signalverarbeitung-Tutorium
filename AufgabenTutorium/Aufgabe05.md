# **Vektoralgebra Aufgaben**

1. **Elementweise Multiplikation**: Bei der elementweisen Multiplikation werden die entsprechenden Elemente der Arrays paarweise multipliziert. 

   Wie kann folgender Code an den Stellen <1> und <2> ergänzt werden?

   ```python
   import numpy as np
   
   array1 = np.array([0, 1, 3])
   array2 = np.array([5, 8, 11, 4])
   
   elementwise_product = #array1 "<1>" array2["<2>"] 
   print(elementwise_product)  # Ausgabe: [0, 8, 33]
   ```
2. **Matrixmultiplikation**:
   Bei der Matrixmultiplikation wird das Skalarprodukt der Zeilen der ersten Matrix und der Spalten der zweiten Matrix berechnet.

   Wie kann folgender Code an den Stellen <1>, <2> und <3> ergänzt werden?

   ```python
   import numpy as np
   
   matrix1 = np.array([[0, 1, 3]])
   matrix2 = np.array([5, 8, 11, 4]).reshape("<1>","<2>")
   
   print(matrix1 "<3>" matrix2) # Ausgabe: [[41]]
   ```
3. **Inneres Produkt (Skalarprodukt)**:
   Das innere Produkt ist die Summe der Produkte der entsprechenden Elemente der Vektoren.

   Nenne 2 Möglichkeiten ein **Skalarprodukt** in Python zu berechnen.

   ```python
   
   ```
4. **Äußeres Produkt**: Beschreibe kurz was das **Äußeres Produkt** ist und wie es berechnet wird. Gerne an einem Beispiel :D

   ```python
   
   ```
5. **Skalarprodukt**: 

   Nenne eine 3. Möglichkeit das innere Produkt zu Berechnen.

   ```python
   np.inner([0,1,3], [5,8,11]) # Ausgabe  41
   np.dot([0,1,3], [5,8,11]) # Ausgabe  41
   np.array([0,1,3]) @  np.array([5,8,11]) # Ausgabe  41
   ```
6. **Kreuzprodukt**:
   Das Kreuzprodukt ist eine Operation, die für Vektoren im dreidimensionalen Raum definiert ist und einen Vektor ergibt, der senkrecht zu den Ausgangsvektoren steht.

   Stelle die Rechnung des Kreuzproduktes schrittweise da. (also was wie verrechnet wird)

   Hilfestellung:

   ```python
   np.cross([0,1,3], [5,8,11]) # Ausgabe: [-13  15  -5]
   ```