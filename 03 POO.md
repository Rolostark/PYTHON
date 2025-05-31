# 3. Clases y objetos, herencia, polimorfismo y métodos mágicos

## Paso 1: Clases y objetos

```python
class Persona:
    def __init__(self, nombre):
        self.nombre = nombre

    def saludar(self):
        print(f"Hola, soy {self.nombre}")

ana = Persona("Ana")
ana.saludar()
```

## Paso 2: Herencia

```python
class Empleado(Persona):
    def trabajar(self):
        print(f"{self.nombre} está trabajando")

luis = Empleado("Luis")
luis.saludar()
luis.trabajar()
```

## Paso 3: Polimorfismo

```python
class Animal:
    def hablar(self):
        print("Sonido genérico")

class Perro(Animal):
    def hablar(self):
        print("Guau")

def hacer_hablar(animal):
    animal.hablar()

hacer_hablar(Perro())
```

## Paso 4: Métodos mágicos (__init__, __str__)

```python
class Libro:
    def __init__(self, titulo):
        self.titulo = titulo

    def __str__(self):
        return f"Libro: {self.titulo}"

libro = Libro("1984")
print(libro)
```