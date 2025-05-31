# 1. Sintaxis básica, variables, operadores, tipos de datos, estructuras de control, funciones y manejo de errores (Python)

A continuación te ofrezco una explicación visual y mejorada de cada concepto fundamental de Python, con diagramas simples y comentarios para facilitar el aprendizaje.

---

## **Paso 1: Variables y Tipos de Datos**

Las variables son contenedores para almacenar datos. En Python no necesitas declarar el tipo, se infiere automáticamente.

| Nombre    | Tipo    | Valor   | Ejemplo de uso           |
|-----------|---------|---------|--------------------------|
| nombre    | str     | "Ana"   | nombre = "Ana"           |
| edad      | int     | 25      | edad = 25                |
| pi        | float   | 3.14    | pi = 3.14                |
| activo    | bool    | True    | activo = True            |

```python
nombre = "Ana"     # Texto
edad = 25          # Número entero
pi = 3.14          # Número decimal
activo = True      # Booleano
print(nombre, edad, pi, activo)
```

**Visualización:**

```
+---------+---------+
| nombre  |  "Ana"  |
+---------+---------+
| edad    |   25    |
+---------+---------+
| pi      |  3.14   |
+---------+---------+
| activo  |  True   |
+---------+---------+
```

---

## **Paso 2: Operadores**

Los operadores permiten realizar operaciones matemáticas y lógicas.

| Operador | Descripción          | Ejemplo      | Resultado        |
|----------|---------------------|--------------|------------------|
| +        | Suma                | 10 + 3       | 13               |
| -        | Resta               | 10 - 3       | 7                |
| *        | Multiplicación      | 10 * 3       | 30               |
| /        | División            | 10 / 3       | 3.333...         |
| %        | Módulo (resto)      | 10 % 3       | 1                |

```python
a = 10
b = 3
print(a + b)  # Suma
print(a - b)  # Resta
print(a * b)  # Multiplicación
print(a / b)  # División
print(a % b)  # Módulo
```

**Visualización:**

```
a = 10
b = 3

[ a ]---+---[ + ]---[ a + b ]--> 13
        |
        +---[ - ]---[ a - b ]--> 7
        |
        +---[ * ]---[ a * b ]--> 30
        |
        +---[ / ]---[ a / b ]--> 3.33
        |
        +---[ % ]---[ a % b ]--> 1
```

---

## **Paso 3: Estructuras de control**

Permiten controlar el flujo del programa: condicionales y bucles.

### a) If / Else (Condicional)

```python
edad = 19
if edad >= 18:
    print("Mayor de edad")
else:
    print("Menor de edad")
```
**Visualización:**
```
        +--------------------------+
        |         edad = 19        |
        +--------------------------+
                    |
            edad >= 18?
                /    \
         Sí /         \ No
     "Mayor de edad"   "Menor de edad"
```

---

### b) For (Bucle con rango)

```python
for i in range(3):
    print("Ciclo número:", i)
```
**Visualización:**
```
i = 0 --> Imprime: Ciclo número: 0
i = 1 --> Imprime: Ciclo número: 1
i = 2 --> Imprime: Ciclo número: 2
```

---

### c) While (Bucle condicional)

```python
contador = 0
while contador < 3:
    print("Contador:", contador)
    contador += 1
```
**Visualización:**
```
contador = 0
¿contador < 3? Sí → imprime y suma 1
contador = 1
¿contador < 3? Sí → imprime y suma 1
contador = 2
¿contador < 3? Sí → imprime y suma 1
contador = 3
¿contador < 3? No → termina bucle
```

---

## **Paso 4: Funciones**

Las funciones son bloques de código reutilizables.

```python
def saludar(nombre):
    print(f"Hola, {nombre}")

saludar("Mundo")
```

**Visualización:**

```
+-------------------+
|  def saludar()    |
+-------------------+
          |
          v
   saludar("Mundo")
          |
          v
     Hola, Mundo
```

---

## **Paso 5: Manejo de errores (Try/Except)**

Permite manejar situaciones inesperadas, como errores en el código.

```python
try:
    resultado = 10 / 0
except ZeroDivisionError:
    print("No se puede dividir por cero")
finally:
    print("Fin de manejo de errores")
```

**Visualización:**

```
try:
    10 / 0   ---> ERROR!
      |
      v
except ZeroDivisionError:
    "No se puede dividir por cero"
finally:
    "Fin de manejo de errores"
```

---

> **Resumen gráfico:**  
> - **Variables** almacenan datos de distintos tipos  
> - **Operadores** permiten hacer cálculos  
> - **Estructuras de control** deciden el flujo del programa  
> - **Funciones** organizan el código en bloques reutilizables  
> - **Manejo de errores** evita que el programa se detenga por fallos

¡Ahora tienes una visión clara y gráfica de los fundamentos de Python!
