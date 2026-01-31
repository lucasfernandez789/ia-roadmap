# Teoría y Referencia Rápida de Python

## 1. Sintaxis Básica
- No se usan llaves ni punto y coma; la indentación define los bloques.
- Comentarios: `# Esto es un comentario`

## 2. Tipos de Datos
- Números: `int`, `float`, `complex`
- Texto: `str`
- Booleanos: `bool` (`True`, `False`)
- Listas: `list` (`[1, 2, 3]`)
- Tuplas: `tuple` (`(1, 2, 3)`)
- Diccionarios: `dict` (`{"clave": valor}`)
- Conjuntos: `set` (`{1, 2, 3}`)

## 3. Operadores
- Aritméticos: `+`, `-`, `*`, `/`, `//` (división entera), `%` (resto), `**` (potencia)
- Comparación: `==`, `!=`, `>`, `<`, `>=`, `<=`
- Lógicos: `and`, `or`, `not`
- Pertenencia: `in`, `not in`
    - Permiten verificar si un elemento está (o no) en una colección (lista, string, diccionario, etc.)
    - Ejemplos:
        ```python
        # Con listas
        nombres = ["Lucas", "Mica", "Mikaela"]
        print("Lucas" in nombres)      # True
        print("Juan" not in nombres)   # True

        # Con strings
        texto = "Hola mundo"
        print("Hola" in texto)         # True
        print("chau" in texto)         # False

        # Con diccionarios (busca en las claves)
        persona = {"nombre": "Lucas", "edad": 25}
        print("nombre" in persona)     # True
        print("Lucas" in persona)      # False
        print("Lucas" in persona.values()) # True
        ```

## 4. Estructuras de Control
- Condicional:
  ```python
  if condicion:
      # bloque
  elif otra_condicion:
      # bloque
  else:
      # bloque
  ```
- Bucle for:
  ```python
  for elemento in lista:
      # bloque
  ```
- Bucle while:
  ```python
  while condicion:
      # bloque
  ```

## 5. Funciones
```python
def mi_funcion(param1, param2="valor por defecto"):
    return param1 + param2
```

## 6. Métodos Útiles
### Listas
- `append(x)` – agrega x al final
- `remove(x)` – elimina la primera aparición de x
- `pop([i])` – elimina y devuelve el elemento en la posición i (o el último)
- `sort()` – ordena la lista
- `reverse()` – invierte el orden
- `count(x)` – cuenta cuántas veces aparece x
- `index(x)` – devuelve la posición de x

### Diccionarios
- `get(clave, valor_por_defecto)` – obtiene el valor de una clave
- `keys()` – devuelve las claves
- `values()` – devuelve los valores
- `items()` – devuelve pares (clave, valor)
- `update(otro_diccionario)` – actualiza con otro diccionario
- `pop(clave)` – elimina y devuelve el valor de la clave

### Strings
- `lower()`, `upper()`, `capitalize()`, `title()`
- `replace(a, b)` – reemplaza a por b
- `split(sep)` – separa en lista
- `join(lista)` – une una lista de strings
- `strip()` – elimina espacios al inicio y final

## 7. Manejo de Archivos
```python
with open("archivo.txt", "r") as f:
    contenido = f.read()
```

## 8. Manejo de Errores
```python
try:
    # código
except Exception as e:
    print(e)
finally:
    # siempre se ejecuta
```

## 9. Importar Módulos
```python
import math
from math import sqrt
```

## 10. List Comprehension
```python
cuadrados = [x**2 for x in range(10)]
```

## 11. Funciones Lambda
```python
f = lambda x: x*2
```

## 12. Recursos Útiles
- Documentación oficial: https://docs.python.org/3/
- Tutorial interactivo: https://www.learnpython.org/
- Cheatsheet: https://www.pythoncheatsheet.org/

---

Agregá tus propias notas y ejemplos a medida que avances.