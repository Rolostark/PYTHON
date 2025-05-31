# 2. Listas, tuplas, diccionarios, sets, métodos integrados y list comprehensions

## Paso 1: Listas

```python
frutas = ["manzana", "banana", "cereza"]
frutas.append("naranja")
print(frutas)
```

## Paso 2: Tuplas

```python
coordenadas = (10, 20)
print(coordenadas[0])
```

## Paso 3: Diccionarios

```python
persona = {"nombre": "Ana", "edad": 25}
print(persona["nombre"])
```

## Paso 4: Sets

```python
numeros = {1, 2, 3, 3, 4}
print(numeros)
```

## Paso 5: Métodos integrados

```python
lista = [4, 2, 8]
lista.sort()
print(lista)
print(len(lista))
```

## Paso 6: List comprehensions

```python
cuadrados = [x**2 for x in range(5)]
print(cuadrados)
```