# reto-8......

#### 1. De los retos anteriores selecione 3 funciones y escribalas en forma de lambdas.

##### Elevar un numero al cuadrado:

```python 
elevar_al_cuadrado = lambda x: x ** 2
```

##### Sumar dos números
```python 
suma = lambda a, b: a + b
```

##### Calcular el promedio de 5 números
```python 
promedio = lambda a, b, c, d, e: (a + b + c + d + e) / 5
```

#### 2. De los retos anteriores selecione 3 funciones y escribalas con argumentos no definidos (*args)

##### Suma de los cuadrados de varios números

```python 
def suma_cuadrados(*args):
    return sum(x**2 for x in args)
```

##### Calcular el mayor número elevado al menor

```python 
def potencia_mayor_menor(*args):
    mayor = max(args)
    menor = min(args)
    return mayor ** menor
```

##### Verificar si todos los números son pares

```python 
def todos_son_pares(*args):
    return all(x % 2 == 0 for x in args)
```

#### 3. Escriba una función recursiva para calcular la operación de la potencia.

```python 
def potencia(x: float, n: int) -> float:
    if n == 0:
        return 1
    else:
        return x * potencia(x, n - 1)
```

#### 4. Contar el tiempo 

```python 
import time

def potencia(x: float, n: int) -> float:
    if n == 0:
        return 1
    else:
        return x * potencia(x, n - 1)

if __name__ == "__main__":
    base = float(input("Ingrese la base (x): "))
    exponente = int(input("Ingrese el exponente (n): "))

    start_time = time.time()  # Inicia temporizador

    resultado = potencia(base, exponente)

    end_time = time.time()    # Finaliza temporizador

    timer = end_time - start_time

    print(f"{base} elevado a la {exponente} es {resultado}")
    print(f"Tiempo de ejecución: {timer:.6f} segundos")
```

#### 5. Imagen de cuenta 

<img width="1713" height="833" alt="image" src="https://github.com/user-attachments/assets/3014b1f1-17c6-40e4-9a27-b74307be8eb4" />

