# Lösung für die Aufgabe 03


1. Welche Bibliotheken benötigst du, um Grafiken zu erstellen?

    matplotlib.pyplot

3. Plotte einen Sinus mit einer Länge von 9. Der dargestellte Bereich soll von 0 bis 20 gehen.

     ```python
     n = np.arange(0, 21)
     omega = 2 * np.pi 
     sin = np.sin(omega/9 * n)
     plt.stem(n, sin)
      ```

4. Plotte einen Cosinus mit einer Länge von 11. Der dargestellte Bereich soll von 0 bis 30 gehen.
     ```python
     n = np.arange(0, 31)
     omega = 2 * np.pi
     cos = np.cos(omega/11 * n)
     plt.stem(n, cos)
      ```
   
5. Plotte einen Sinus und einen Cosinus in einem Diagramm(mit unterschiedlichen Farben). Beide Funktionen sollen eine Länge von 8 haben, und der dargestellte Bereich soll von 0 bis 17 gehen.
      ```python
      n = np.arange(0, 18)
      omega = 2 * np.pi
      sin = np.sin(omega/8 * n)
      cos = np.cos(omega/8 * n)
      plt.stem(n, sin, 'r')
      plt.stem(n, cos, 'g')
      ```
  
6. Plotte einen Sinus, der um 3 Einheiten nach links verschoben ist. Die Funktion soll eine Länge von 10 haben, und der dargestellte Bereich soll von 0 bis 20 gehen.
   ```python
   n = np.arange(0, 21)
   omega = 2 * np.pi
   sin = np.sin(omega/10 * (n+3))
   plt.stem(n, sin)
   ```

7. Plotte einen Cosinus, der um 2 Einheiten nach unten verschoben ist. Die Funktion soll eine Länge von 12 haben, und der dargestellte Bereich soll von 0 bis 25 gehen.
   ```python
   n = np.arange(0, 26)
   omega = 2 * np.pi
   cos = np.cos(omega/12 * (n))-2
   plt.stem(n, cos)
   ```
   
8. Plotte einen Sinus, der um 3 Einheiten gestreckt ist. Die Funktion soll eine Länge von 6 haben, und der dargestellte Bereich soll von 0 bis 18 gehen.

   ```python
   n = np.arange(0, 19)
   omega = 2 * np.pi
   sin = 3*np.sin(omega/6 * n)
   plt.stem(n, sin)
   ```

