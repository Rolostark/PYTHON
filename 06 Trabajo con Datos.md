# 6. NumPy, Pandas, Matplotlib, Seaborn y APIs (requests, FastAPI)

## Paso 1: NumPy

```python
import numpy as np
a = np.array([1, 2, 3])
print(a + 2)
```

## Paso 2: Pandas

```python
import pandas as pd
datos = {'nombre': ['Ana', 'Luis'], 'edad': [25, 30]}
df = pd.DataFrame(datos)
print(df)
```

## Paso 3: Matplotlib

```python
import matplotlib.pyplot as plt
plt.plot([1, 2, 3], [4, 5, 6])
plt.title("Ejemplo Matplotlib")
plt.show()
```

## Paso 4: Seaborn

```python
import seaborn as sns
import pandas as pd
df = pd.DataFrame({'x': [1, 2, 3], 'y': [5, 6, 7]})
sns.scatterplot(data=df, x='x', y='y')
```

## Paso 5: APIs - requests

```python
import requests
respuesta = requests.get("https://api.github.com")
print(respuesta.status_code)
```

## Paso 6: APIs - FastAPI

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def leer_raiz():
    return {"mensaje": "Hola Mundo"}
```