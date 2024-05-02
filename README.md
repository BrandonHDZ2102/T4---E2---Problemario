# T4---E2---Problemario
Desarrolla ejercicios que involucren cálculos numéricos para solución de problemas que apliquen diferenciación e integración, empleando los siguientes métodos: Método de trapecio, Regla se Simpson y Método de la Cuadratura Gaussiana y documenta problemario a entregar.

# MetodosNumericosTema3Problemario

### Equipo

- Italia Yoselin Lozada Olvera
- Gabriel Hernandez Zavala
- Brandon Hernández Espinosa


## Método de trapecio
### Descripcion 

El Método de Eliminación de Gauss consiste en utilizar reiteradas veces las propiedades de los sistemas lineales, que hemos visto ante- riormente, para transformar un sistema de ecuaciones lineales en otro equivalente (con las mismas soluciones) pero que sea triangular.

### Pseudocódigo 
```
Función MetodoTrapecio(a, b, n, f):
    h = (b - a) / n
    sum = 0.5 * (f(a) + f(b))

    Para cada i de 1 a n-1:
        x = a + i * h
        sum += f(x)

    retornar h * sum

Función funcionEjemplo(x):
    retornar x * x

a = 0 // Límite inferior de integración
b = 2 // Límite superior de integración
n = 100 // Número de trapecios

integral = MetodoTrapecio(a, b, n, funcionEjemplo)

Imprimir "La aproximación de la integral es: " + integral

```


### Implementacion 
- Implementacion en Python

```
  def f(x):
    # Define la función que deseas integrar
    return x**2  # Ejemplo: x^2

def metodo_trapecio(a, b, n):
    # Calcula el ancho de cada subintervalo
    h = (b - a) / n
    
    # Inicializa la suma
    suma = 0
    
    # Calcula la suma de las áreas de los trapecios
    for i in range(1, n):
        xi = a + i * h
        suma += f(xi)
    
    # Aplica la fórmula del método del trapecio
    resultado = h * (f(a) / 2 + f(b) / 2 + suma)
    return resultado

# Ejemplo de uso
a = 0  # Límite inferior
b = 1  # Límite superior
n = 1000  # Número de subintervalos

resultado = metodo_trapecio(a, b, n)
print("Resultado de la integración usando el método del trapecio:", resultado)

```




        

### Ejercicios en java

[Ejemplo 1](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeTrapecio/MetodoTrapecio1.java)

[Ejemplo 2](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeTrapecio/MetodoTrapecio2.java)

[Ejemplo 3](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeTrapecio/MetodoTrapecio3.java)

[Ejemplo 4](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeTrapecio/MetodoTrapecio4.java)

[Ejemplo 5](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeTrapecio/MetodoTrapecio5.java)


==========================================================================================================================

## Regla de Simpson
### Descripcion 

El Método de Eliminación de Gauss consiste en utilizar reiteradas veces las propiedades de los sistemas lineales, que hemos visto ante- riormente, para transformar un sistema de ecuaciones lineales en otro equivalente (con las mismas soluciones) pero que sea triangular.

### Pseudocódigo 
```
Función funcion(x):
    retornar 2 * x + 3 // Función lineal: f(x) = 2x + 3

Función reglaDeSimpson(a, b, n):
    h = (b - a) / n
    sum = funcion(a) + funcion(b)

    Para cada i de 1 a n-1, incrementando de 2 en 2:
        sum += 4 * funcion(a + i * h)

    Para cada i de 2 a n-1, incrementando de 2 en 2:
        sum += 2 * funcion(a + i * h)

    retornar (h / 3) * sum

a = 0 // Límite inferior
b = 4 // Límite superior
n = 100 // Número de intervalos

Imprimir "Resultado: " + reglaDeSimpson(a, b, n)

```



### Implementacion 
- Implementacion en Python

```
def f(x):
    # Define la función que deseas integrar
    return x**2  # Ejemplo: x^2

def regla_simpson(a, b, n):
    # Calcula el ancho de cada subintervalo
    h = (b - a) / n
    
    # Inicializa la suma
    suma = 0
    
    # Calcula la suma para los puntos impares
    for i in range(1, n, 2):
        xi = a + i * h
        suma += 4 * f(xi)
    
    # Calcula la suma para los puntos pares
    for i in range(2, n-1, 2):
        xi = a + i * h
        suma += 2 * f(xi)
    
    # Aplica la fórmula de la regla de Simpson
    resultado = h / 3 * (f(a) + f(b) + suma)
    return resultado

#Ejemplo de uso
a = 0  # Límite inferior
b = 1  # Límite superior
n = 1000  # Número de subintervalos

resultado = regla_simpson(a, b, n)
print("Resultado de la integración usando la regla de Simpson:", resultado)

```   
    
### Ejercicios en java

[Ejemplo 1](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/ReglaDeSimpson/ReglaDeSimpson1.java)

[Ejemplo 2](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/ReglaDeSimpson/ReglaDeSimpson2.java)

[Ejemplo 3](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/ReglaDeSimpson/ReglaDeSimpson3.java)

[Ejemplo 4](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/ReglaDeSimpson/ReglaDeSimpson4.java)

[Ejemplo 5](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/ReglaDeSimpson/ReglaDeSimpson5.java)


==========================================================================================================================


## Método de la Cuadratura Gaussiana 
### Descripcion 

El Método de Eliminación de Gauss consiste en utilizar reiteradas veces las propiedades de los sistemas lineales, que hemos visto ante- riormente, para transformar un sistema de ecuaciones lineales en otro equivalente (con las mismas soluciones) pero que sea triangular.

### Pseudocódigo 

```
Función cuadraturaGaussiana(funcion, limiteInferior, limiteSuperior, numeroPuntos):
    nodos = [-0.9324695142, -0.6612093865, -0.2386191861, 0.2386191861, 0.6612093865, 0.9324695142] // Nodos predefinidos para seis puntos
    pesos = [0.1713244924, 0.3607615730, 0.4679139346, 0.4679139346, 0.3607615730, 0.1713244924] // Pesos predefinidos para seis puntos

    suma = 0

    Para cada i de 0 a numeroPuntos-1:
        transformacion = (limiteSuperior - limiteInferior) / 2 * nodos[i] + (limiteSuperior + limiteInferior) / 2
        suma += pesos[i] * funcion(transformacion)

    retornar (limiteSuperior - limiteInferior) / 2 * suma

funcion = función(x) -> 1 / (1 + x * x)
limiteInferior = 0
limiteSuperior = 1
numeroPuntos = 6 // Utilizando seis puntos para la cuadratura gaussiana

resultado = cuadraturaGaussiana(funcion, limiteInferior, limiteSuperior, numeroPuntos)
Imprimir "Resultado de la integral: " + resultado

```

### Implementacion 
- Implementacion en Python

 ```
import numpy as np

def f(x):
    # Define la función que deseas integrar
    return x**2  # Ejemplo: x^2

def cuadratura_gaussiana(f, a, b, n):
    # Obtiene los nodos y pesos de Gauss-Legendre
    nodos, pesos = np.polynomial.legendre.leggauss(n)
    
    # Transforma los nodos de [-1, 1] al intervalo [a, b]
    x_transformed = 0.5 * (b - a) * nodos + 0.5 * (a + b)
    
    # Calcula la suma ponderada de los valores de la función en los nodos transformados
    suma = sum(pesos * f(x_transformed))
    
    # Aplica el factor de escala para el intervalo [a, b]
    resultado = 0.5 * (b - a) * suma
    return resultado

# Ejemplo de uso
a = 0  # Límite inferior
b = 1  # Límite superior
n = 5  # Orden de la cuadratura

resultado = cuadratura_gaussiana(f, a, b, n)
print("Resultado de la integración usando Cuadratura Gaussiana:", resultado)

 ```

### Ejercicios en java

[Ejemplo 1](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana1.java)

[Ejemplo 2](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana2.java)

[Ejemplo 3](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana3.java)

[Ejemplo 4](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana4.java)

[Ejemplo 5](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana5.java)



