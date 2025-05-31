# 5. Threading, multiprocessing y async/await (asyncio)

## Paso 1: Threading

```python
import threading

def imprimir():
    print("Hilo en ejecución")

hilo = threading.Thread(target=imprimir)
hilo.start()
hilo.join()
```

## Paso 2: Multiprocessing

```python
import multiprocessing

def imprimir():
    print("Proceso en ejecución")

proceso = multiprocessing.Process(target=imprimir)
proceso.start()
proceso.join()
```

## Paso 3: Async/Await (asyncio)

```python
import asyncio

async def saludar():
    print("Hola async")
    await asyncio.sleep(1)
    print("Adiós async")

asyncio.run(saludar())
```