# Elementarsignale Zeichnen - Sprung und impuls

## Sprungfunktion erstellen
- Was macht "np.heaviside" in Python?
  
  A: np.heaviside nimmt ein array von zahlen und returnt 0
  
- Was macht folgender Code?
  ```python
  import numpy as np
  import matplotlib.pyplot as plt
  
  n = np.arange(0,15) #Array mit Werten von 0 bis 14 erstellt
  array = np.heaviside(n,1) #für alle werte in n wird 1 in "array" erstellt
  plt.stem(n,array) #Hier wird das array mit nur 1 auf alle werte für n dargestellt
  ```
  
- Wie kann eine Sprungfunktion erstellt werden, die um 5 Einheiten auf der X-Achse verschoben ist?
```python
  import numpy as np
  import matplotlib.pyplot as plt

  #Standardwerte Sygnalsysnthes
  n = np.arange(0,16+1) #Wertebereiches des Signals
  array = np.heaviside(n-5,1) #Funktion
  plt.stem(n,array) #Plot des arrays, über alle werte in n
  ```
