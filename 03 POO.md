# 3. Clases y objetos, herencia, polimorfismo y métodos mágicos

En este apartado aprenderás cómo funcionan los pilares de la Programación Orientada a Objetos (POO) en Python, acompañados de explicaciones y ejemplos.

---

## Paso 1: Clases y objetos

Una **clase** es como un molde o plantilla para crear objetos. Un **objeto** es una instancia de una clase, con características (atributos) y comportamientos (métodos).

```python
class Persona:
    def __init__(self, nombre):   # Método especial que inicializa el objeto
        self.nombre = nombre      # Atributo del objeto

    def saludar(self):            # Método para saludar
        print(f"Hola, soy {self.nombre}")

# Crear un objeto "ana" de la clase Persona
ana = Persona("Ana")
ana.saludar()  # Imprime: Hola, soy Ana
```

---

## Paso 2: Herencia

La **herencia** permite crear una nueva clase a partir de otra existente. La clase nueva (subclase) hereda los atributos y métodos de la clase base (superclase), y además puede agregar nuevos o modificar los existentes.

```python
# Definición de la clase base Persona
class Persona:
    def __init__(self, nombre):   # Método constructor, inicializa el atributo 'nombre'
        self.nombre = nombre      # Guarda el nombre en el objeto

    def saludar(self):            # Método para saludar
        print(f"Hola, soy {self.nombre}")  # Imprime un saludo usando el nombre

# Definición de la clase Empleado que hereda de Persona
class Empleado(Persona):          # Empleado hereda de Persona
    def trabajar(self):           # Nuevo método específico de Empleado
        print(f"{self.nombre} esta trabajando")  # Imprime que el empleado está trabajando

# Crear un objeto llamado luis de la clase Empleado
luis = Empleado("Luis")           # Se crea un empleado llamado Luis
luis.saludar()                    # Llama al método heredado de Persona
luis.trabajar()                   # Llama al método propio de Empleado
```

---

## Paso 3: Polimorfismo

El **polimorfismo** es la capacidad de usar una misma interfaz (método) para diferentes tipos de objetos. Es decir, distintos objetos pueden responder de manera diferente a un mismo método.

```python
class Animal:
    def hablar(self):
        print("Sonido genérico")

class Perro(Animal):
    def hablar(self):          # Sobrescribe el método de Animal
        print("Guau")

def hacer_hablar(animal):     # Función que acepta cualquier animal
    animal.hablar()

hacer_hablar(Perro())         # Imprime: Guau
```

---

## Paso 4: Métodos mágicos (`__init__`, `__str__`)

Los **métodos mágicos** (o dunder methods) son métodos especiales que Python reconoce por tener dos guiones bajos antes y después de su nombre. Permiten modificar el comportamiento por defecto de los objetos.

- `__init__`: Se llama automáticamente al crear una nueva instancia.
- `__str__`: Define cómo se representa el objeto como texto (por ejemplo, al usar `print()`).

```python
class Libro:
    def __init__(self, titulo):
        self.titulo = titulo

    def __str__(self):
        return f"Libro: {self.titulo}"

libro = Libro("1984")
print(libro)   # Imprime: Libro: 1984
```

---

**Resumen:**  
- **Clases y objetos**: Creas moldes y luego instancias de esos moldes.
- **Herencia**: Puedes reutilizar y extender código de otras clases.
- **Polimorfismo**: Distintos objetos pueden comportarse de manera diferente usando la misma interfaz.
- **Métodos mágicos**: Personalizan el comportamiento de tus objetos en Python.
