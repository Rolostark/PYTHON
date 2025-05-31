# 2. Listas, tuplas, diccionarios, sets, métodos integrados y list comprehensions

Te explico visualmente cada estructura y método fundamental de Python para trabajar con colecciones de datos:

---

## **Paso 1: Listas**

Las listas son colecciones ordenadas y mutables de elementos.

```python
frutas = ["manzana", "banana", "cereza"]
frutas.append("naranja")
print(frutas)
```

**Visualización:**
```
frutas: ┌────────────┬─────────┬────────┐
        │ "manzana"  │ "banana"│"cereza"│
        └────────────┴─────────┴────────┘
.append("naranja")
        ↓
frutas: ┌────────────┬─────────┬────────┬──────────┐
        │ "manzana"  │ "banana"│"cereza"│"naranja" │
        └────────────┴─────────┴────────┴──────────┘
```

---

## **Paso 2: Tuplas**

Las tuplas son colecciones ordenadas e inmutables.

```python
coordenadas = (10, 20)
print(coordenadas[0])
```

**Visualización:**
```
coordenadas: ( 10 , 20 )
Acceso:
coordenadas[0] → 10
```

---

## **Paso 3: Diccionarios**

Los diccionarios almacenan pares clave-valor.

```python
persona = {"nombre": "Ana", "edad": 25}
print(persona["nombre"])
```

**Visualización:**
```
persona:
┌─────────┬──────┐
│ nombre  │ "Ana"│
├─────────┼──────┤
│ edad    │  25  │
└─────────┴──────┘

Acceso: persona["nombre"] → "Ana"
```

---

## **Paso 4: Sets (Conjuntos)**

Los sets son colecciones no ordenadas y sin elementos duplicados.

```python
numeros = {1, 2, 3, 3, 4}
print(numeros)
```

**Visualización:**
```
numeros: {1, 2, 3, 4}
(Duplicado "3" se elimina automáticamente)
```

---

## **Paso 5: Métodos integrados**

Las listas tienen métodos útiles como `.sort()` y la función `len()`.

```python
lista = [4, 2, 8]
lista.sort()
print(lista)
print(len(lista))
```

**Visualización:**
```
Original:     [4, 2, 8]
.lista.sort() [2, 4, 8]
len(lista)    3  (cantidad de elementos)
```

---

## **Paso 6: List comprehensions**

Permiten crear listas de forma compacta y eficiente.

```python
cuadrados = [x**2 for x in range(5)]
print(cuadrados)
```

**Visualización:**
```
x en range(5): 0, 1, 2, 3, 4

[ x**2 for x in range(5) ] → [0, 1, 4, 9, 16]

Proceso:
0**2 → 0
1**2 → 1
2**2 → 4
3**2 → 9
4**2 → 16
```

---

> **Resumen gráfico:**  
> - **Listas:** Ordenadas, mutables, permiten duplicados  
> - **Tuplas:** Ordenadas, inmutables  
> - **Diccionarios:** Clave-valor, acceso rápido  
> - **Sets:** Sin duplicados, no ordenados  
> - **Métodos integrados:** Manipulan y consultan colecciones  
> - **List comprehensions:** Creación eficiente de listas

¡Así puedes trabajar con las principales colecciones y métodos en Python!
