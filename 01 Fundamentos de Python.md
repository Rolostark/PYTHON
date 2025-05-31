# 1. Sintaxis básica, variables, operadores, tipos de datos, estructuras de control, funciones y manejo de errores

## Paso 1: Variables y tipos de datos

```python
nombre = "Ana"
edad = 25
pi = 3.14
activo = True
print(nombre, edad, pi, activo)
```

## Paso 2: Operadores

```python
a = 10
b = 3
print(a + b)  # Suma
print(a - b)  # Resta
print(a * b)  # Multiplicación
print(a / b)  # División
print(a % b)  # Módulo
```

## Paso 3: Estructuras de control

```python
# If
if edad >= 18:
    print("Mayor de edad")
else:
    print("Menor de edad")

# For
for i in range(3):
    print("Ciclo número:", i)

# While
contador = 0
while contador < 3:
    print("Contador:", contador)
    contador += 1
```

## Paso 4: Funciones

```python
def saludar(nombre):
    print(f"Hola, {nombre}")

saludar("Mundo")
```

## Paso 5: Manejo de errores

```python
try:
    resultado = 10 / 0
except ZeroDivisionError:
    print("No se puede dividir por cero")
finally:
    print("Fin de manejo de errores")
```