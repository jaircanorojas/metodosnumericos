
# Metodos Numericos
## Problemario Tema 2

En este problemario veremos diferentes metodos como Biseccion, Regla falsa,Interpolacion y Secante


## Biseccion
La bisección es un método numérico para encontrar raíces de funciones. Se divide un intervalo donde se sospecha que se encuentra la raíz hasta alcanzar una precisión deseada. Es simple y garantiza convergencia si se cumplen ciertas condiciones.

[![biseccion1.png](https://i.postimg.cc/KYxWYnCm/biseccion1.png)](https://postimg.cc/hXZsy7SY)

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/eb3a25aa73f54c11aa88f4796f16fc5d3bb5f8c1/Biseccion1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/0bae9d0382efd0142d31a2a92e2b025e1c9d4964/Biseccion2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/e9b34dfe70013d1f7034eec67a7666816b7ed27d/Biseccion3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/159febd048141ac6d9d256dfb46c95ab84511fe1/Biseccion4)


## Regla Falsa
Se basa en la interpolación lineal entre dos puntos extremos del intervalo que contiene la raíz, y luego utiliza el punto de intersección con el eje x como una mejor aproximación de la raíz. Este proceso se repite hasta que se alcanza la precisión deseada.

[![regla-falsa-3.jpg](https://i.postimg.cc/d3jb64bN/regla-falsa-3.jpg)](https://postimg.cc/SYj1N7Nc)

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/6786f9c122d5064914e1e38efde893955d4aeca1/Reglafalsa1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/b375f73ca211f0fc6408d6e664a3b2aa89b101c8/Reglafalsa2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/b375f73ca211f0fc6408d6e664a3b2aa89b101c8/Reglafalsa3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/b375f73ca211f0fc6408d6e664a3b2aa89b101c8/Reglafalsa4)

[Ejemplo 5](https://github.com/jaircanorojas/metodosnumericos/blob/b375f73ca211f0fc6408d6e664a3b2aa89b101c8/Reglafalsa5)

## Interpolacion
Es un método para encontrar una función que pase a través de un conjunto de puntos dados. Utiliza diferentes técnicas, como el polinomio de Lagrange o el polinomio de Newton, para encontrar una aproximación de la función entre los puntos conocidos. 

[![grafica-de-polinomios-de-legendre.png](https://i.postimg.cc/bw9Rv4QB/grafica-de-polinomios-de-legendre.png)](https://postimg.cc/hXhmyyZL)

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion4)

[Ejemplo 5](https://github.com/jaircanorojas/metodosnumericos/blob/b69ce628c56d8db89d99f4efe00ffca2a7e17661/interpolacion5)

## Secante
Es un método numérico para encontrar raíces de funciones que combina la idea del método de Newton-Raphson con la aproximación de la pendiente mediante una secante.

[![220px-Secant-method-svg.png](https://i.postimg.cc/SsCRSb9X/220px-Secant-method-svg.png)](https://postimg.cc/MMZq54dx)

[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/7b0eb88398b20966db1b99998749e87731d44efe/Secante1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/7b0eb88398b20966db1b99998749e87731d44efe/Secante2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/7b0eb88398b20966db1b99998749e87731d44efe/Secante3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/7b0eb88398b20966db1b99998749e87731d44efe/Secante4)


# Problemario Tema 3
"Equipo: Wenceslao Benitez Rosquero, Jair Cano Rojas y Adriana Jamileth Mendoza Ortiz"

## MÉTODO DE ELIMINACIÓN GAUSSIANA
Es un algoritmo utilizado para resolver sistemas de ecuaciones lineales. Su objetivo es transformar el sistema original en otro equivalente más simple mediante una secuencia de operaciones elementales (como sumar un múltiplo de una fila a otra o intercambiar filas), hasta obtener un sistema triangular superior o triangular inferior.

[![matrix-echelon-form.png](https://i.postimg.cc/Kcn3HhvW/matrix-echelon-form.png)](https://postimg.cc/K48Y1VT7)

[Implementacion en java](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/javaelimgau)

**ALGORITMO**
1. Entrada: Matriz aumentada [A|b] del sistema de ecuaciones lineales.
2. Para cada fila i desde 1 hasta n-1:
     a. Encuentra el pivote máximo en la columna actual y intercambia filas si es necesario.
     b. Para cada fila j desde i+1 hasta n:
           i. Calcula el factor de eliminación f = A(j, i) / A(i, i).
           ii. Para cada columna k desde i hasta n:
                 1. Actualiza A(j, k) = A(j, k) - f * A(i, k).
           iii. Actualiza b(j) = b(j) - f * b(i).
3. Sustitución hacia atrás:
     a. Para k = n hasta 1, de manera decreciente:
           i. Calcula la solución X(k) = (b(k) - Σ(A(k, j) * X(j)) para j = k+1 hasta n) / A(k, k).
4. Devuelve el vector de soluciones X como resultado del sistema de ecuaciones lineales.


[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU4)

[Ejemplo 5](https://github.com/jaircanorojas/metodosnumericos/blob/2b00a6fa1cbf1bf081eb4e8c5032d194a0aa0b0c/GAU5)

## MÉTODO DE GAUSS JORDAN
Se basa en la eliminación de incógnitas mediante operaciones elementales sobre filas para transformar la matriz original en una forma escalonada o reducida por filas.

[![Captura-de-Pantalla-2021-11-09-a-las-11-28-59.png](https://i.postimg.cc/4dVWF4dd/Captura-de-Pantalla-2021-11-09-a-las-11-28-59.png)](https://postimg.cc/1nR08QDh)

[Implementacion en java](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/javajordan)

**ALGORITMO**
1. Inicia con una matriz aumentada [A | b], donde A es la matriz de coeficientes y b es el vector de términos independientes.
2. Para cada fila i de la matriz:
      a. Encuentra el pivote, que es el elemento A[i][i].
      b. Divide la fila i por el pivote para hacer que el pivote sea igual a 1.
      c. Para cada fila j ≠ i:
            i. Resta un múltiplo apropiado de la fila i de la fila j para hacer que todos los elementos debajo del pivote sean iguales a cero.
3. Para cada fila i de la matriz:
      a. Para cada fila j ≠ i:
            i. Resta un múltiplo apropiado de la fila i de la fila j para hacer que todos los elementos encima del pivote sean iguales a cero.
4. Devuelve la matriz resultante, que ahora estará en la forma escalonada reducida por filas. Si se está resolviendo un sistema de ecuaciones lineales, extrae el vector de soluciones.


[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/gaus1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/gaus2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/gaus3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/gaus4)

[Ejemplo 5](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/gaus5)

## MÉTODO DE GAUSS SEIDEL

1. **Adivina**: Adivina un conjunto inicial de soluciones.
   
2. **Itera**: Actualiza iterativamente las soluciones utilizando la información más reciente.

3. **Repite**: Continúa hasta que las soluciones converjan.

4. **Obtén resultados**: Utiliza las soluciones convergentes como las aproximaciones finales del sistema.

[![descarga.png](https://i.postimg.cc/wBvnq4cp/descarga.png)](https://postimg.cc/BjrmNgVY)

[Implementacion en java](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/seideljava)

**ALGORITMO**
1. Inicializa un conjunto de soluciones inicial, X^(0).
2. Repite hasta que converja:
      a. Para cada variable i del sistema:
            i. Inicializa una variable auxiliar, sum = 0.
            ii. Para cada variable j del sistema donde j ≠ i:
                  Calcula la suma: sum = sum + (A_ij * X_j^(k)).
            iii. Calcula el valor actualizado de la variable:
                  X_i^(k+1) = (1 / A_ii) * (b_i - sum).
3. Verifica el criterio de convergencia. Si se cumple, termina el proceso.
4. Incrementa el contador de iteración k.
5. Devuelve el conjunto de soluciones X^(k+1) como la aproximación del sistema.


[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/seidel1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/seidel2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/seidel3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/seidel4)

[Ejemplo 5](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/seidel5)

## MÉTODO DE JACOBI

1. **Inicializa**: Empieza con una suposición inicial de las soluciones.

2. **Itera**: Actualiza simultáneamente todas las soluciones utilizando las versiones anteriores de las soluciones.

3. **Repite**: Continúa iterando hasta que se alcance la convergencia.

4. **Obtén resultados**: Utiliza las soluciones convergentes como las aproximaciones finales del sistema.

[![maxresdefault.jpg](https://i.postimg.cc/4dZZ1kDT/maxresdefault.jpg)](https://postimg.cc/FfP29qFP)

[Implementacion en java](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/jacobijava)

**ALGORITMO**
1. Inicializa un conjunto de soluciones inicial, X^(0).
2. Para cada iteración k = 1, 2, ..., hasta que converja:
      a. Para cada variable i del sistema:
            i. Calcula el valor actualizado de la variable utilizando la fórmula de Jacobi:
                 X_i^(k) = (1 / A_ii) * (b_i - Σ(A_ij * X_j^(k-1)), para j ≠ i)
      b. Verifica el criterio de convergencia. Si se cumple, termina el proceso.
3. Devuelve el conjunto de soluciones X^(k) como la aproximación del sistema.


[Ejemplo 1](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/jacobi1)

[Ejemplo 2](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/jacobi2)

[Ejemplo 3](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/jacobi3)

[Ejemplo 4](https://github.com/jaircanorojas/metodosnumericos/blob/4d1c3495c888bfaa13390802cc004bc4d2e5c3a2/jacobi4)




















