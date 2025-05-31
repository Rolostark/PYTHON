# 4. Crear/importar módulos, pip, entornos virtuales y librerías estándar

## Paso 1: Crear e importar módulos

**mi_modulo.py**
```python
def saludar():
    print("Hola desde mi módulo")
```

**main.py**
```python
import mi_modulo
mi_modulo.saludar()
```

## Paso 2: Pip y entornos virtuales

```bash
python -m venv mi_entorno
# Activar entorno virtual en Windows
mi_entorno\Scripts\activate
# Activar en Mac/Linux
source mi_entorno/bin/activate
pip install requests
```

## Paso 3: Librerías estándar

```python
import os
import datetime
import math

print(os.getcwd())
print(datetime.datetime.now())
print(math.sqrt(16))
```