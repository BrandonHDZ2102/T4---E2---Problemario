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




### Implementacion 
- Implementacion en Python


    >def f(x):
    >#Define la función que deseas integrar
    >return x**2  # Ejemplo: x^2

>def metodo_trapecio(a, b, n):
   > #Calcula el ancho de cada subintervalo
   > h = (b - a) / n
    
   > #Inicializa la suma
   > suma = 0
    
   > #Calcula la suma de las áreas de los trapecios
  >  for i in range(1, n):
      >  xi = a + i * h
       > suma += f(xi)
    
    ># Aplica la fórmula del método del trapecio
 >   resultado = h * (f(a) / 2 + f(b) / 2 + suma)
   > return resultado

>#Ejemplo de uso
>a = 0  # Límite inferior
>b = 1  # Límite superior
>n = 1000  # Número de subintervalos

>resultado = metodo_trapecio(a, b, n)
> print("Resultado de la integración usando el método del trapecio:", resultado)




        

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




### Implementacion 
- Implementacion en Python


        

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




### Implementacion 
- Implementacion en Python


        

### Ejercicios en java

[Ejemplo 1](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana1.java)

[Ejemplo 2](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana2.java)

[Ejemplo 3](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana3.java)

[Ejemplo 4](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana4.java)

[Ejemplo 5](https://github.com/GABOHDEZ2001/PROBLEMARIOTEMA4METODOS/blob/main/T4-E2-Problemario/src/M%C3%A9todoDeLaCuadraturaGaussiana/M%C3%A9todoDeLaCuadraturaGaussiana5.java)



