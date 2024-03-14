
# Metodos Numericos
## Problemario Tema 2

En este problemario veremos diferentes metodos como Biseccion, Regla falsa,Interpolacion y Secante


## Biseccion
La bisección es un método numérico para encontrar raíces de funciones. Se divide un intervalo donde se sospecha que se encuentra la raíz hasta alcanzar una precisión deseada. Es simple y garantiza convergencia si se cumplen ciertas condiciones.

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/eb3a25aa73f54c11aa88f4796f16fc5d3bb5f8c1/Biseccion1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/0bae9d0382efd0142d31a2a92e2b025e1c9d4964/Biseccion2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/e9b34dfe70013d1f7034eec67a7666816b7ed27d/Biseccion3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/159febd048141ac6d9d256dfb46c95ab84511fe1/Biseccion4)


## Regla Falsa
Se basa en la interpolación lineal entre dos puntos extremos del intervalo que contiene la raíz, y luego utiliza el punto de intersección con el eje x como una mejor aproximación de la raíz. Este proceso se repite hasta que se alcanza la precisión deseada.

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/6786f9c122d5064914e1e38efde893955d4aeca1/Reglafalsa1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/b375f73ca211f0fc6408d6e664a3b2aa89b101c8/Reglafalsa2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/b375f73ca211f0fc6408d6e664a3b2aa89b101c8/Reglafalsa3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/b375f73ca211f0fc6408d6e664a3b2aa89b101c8/Reglafalsa4)

[Ejemplo 5](https://github.com/jaircanorojas/metodosnumericos/blob/b375f73ca211f0fc6408d6e664a3b2aa89b101c8/Reglafalsa5)

## Interpolacion
Es un método para encontrar una función que pase a través de un conjunto de puntos dados. Utiliza diferentes técnicas, como el polinomio de Lagrange o el polinomio de Newton, para encontrar una aproximación de la función entre los puntos conocidos. 

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion4)

[Ejemplo 5](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion5)

## Secante
Es un método numérico para encontrar raíces de funciones que combina la idea del método de Newton-Raphson con la aproximación de la pendiente mediante una secante.

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/7b0eb88398b20966db1b99998749e87731d44efe/Secante1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/7b0eb88398b20966db1b99998749e87731d44efe/Secante2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/7b0eb88398b20966db1b99998749e87731d44efe/Secante3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/7b0eb88398b20966db1b99998749e87731d44efe/Secante4)


## Problemario Tema 3
"Equipo: Wenceslao Benitez Rosquero, Jair Cano Rojas y Adriana Jamileth Mendoza Ortiz"

## MÉTODO DE ELIMINACIÓN GAUSSIANA
Es un algoritmo utilizado para resolver sistemas de ecuaciones lineales. Su objetivo es transformar el sistema original en otro equivalente más simple mediante una secuencia de operaciones elementales (como sumar un múltiplo de una fila a otra o intercambiar filas), hasta obtener un sistema triangular superior o triangular inferior.

[![matrix-echelon-form.png](https://i.postimg.cc/Kcn3HhvW/matrix-echelon-form.png)](https://postimg.cc/K48Y1VT7)

[Implementacion en java](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/javaelimgau)

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU4)

[Ejemplo 5](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU5)

## MÉTODO DE Gauss Jordan
Se basa en la eliminación de incógnitas mediante operaciones elementales sobre filas para transformar la matriz original en una forma escalonada o reducida por filas.

[![Captura-de-Pantalla-2021-11-09-a-las-11-28-59.png](https://i.postimg.cc/4dVWF4dd/Captura-de-Pantalla-2021-11-09-a-las-11-28-59.png)](https://postimg.cc/1nR08QDh)

[Implementacion en java]()

[Ejemplo 1]()

[Ejemplo 2]()

[Ejemplo 3]()

[Ejemplo 4]()

[Ejemplo 5]()












