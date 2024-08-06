---
#author: Dr. Héctor Selley
title: Práctica 5 - Programación funcional
fontfamily: libertinus
fontsize: 12pt
geometry: margin=3cm
papersize: letter
documentclass: scrartcl
---

Desarrolle en _Python_ los siguientes programas.

1. Dada una lista de números enteros cualquiera, utilice los métodos map, filter y reduce para 
    filtrar los números impares de la lista y calcular la suma de sus cuadrados.

2. Dada una lista de diccionarios que representan productos con nombre (llave en el diccionario) 
    y precio (valor de la llave en el diccionario), filtre los productos que cuestan más de $200, 
    y aplique un descuento del 10%. Finalmente calcule el total de los productos que tienen 
    descuento.

3. Existe un método llamado mínimos cuadrados que en su caso lineal permite obtener una línea recta
    que se aproxima a una serie de $m$ puntos $(x,y)$. La recta resultante del método es 
    $y = a_0 + a_1x$, y para calcular los coeficientes $a_0$ y $a_1$ se utilizan las siguientes 
    fórmulas: 

    $$
    a_0 = \dfrac{\displaystyle{\sum_{i=1}^{m}x_i^2 \sum_{i=1}^{m}y_i - \sum_{i=1}^{m}x_iy_i \sum_{i=1}^m x_i}}{m \left(\displaystyle{\sum_{i=1}^{m}x_i^2}\right) - \left(\displaystyle{\sum_{i=1}^m x_i}\right)^2} 
    $$
    $$
    a_1 = \dfrac{\displaystyle{m\sum_{i=1}^{m}x_iy_i - \sum_{i=1}^{m}x_i \sum_{i=1}^m y_i}}{m \left(\displaystyle{\sum_{i=1}^{m}x_i^2}\right) - \left(\displaystyle{\sum_{i=1}^m x_i}\right)^2}
    $$

    Desarrolle un programa en Python que realice el cálculo de las fórmulas, utilice las funciones
    `lambda`, `map`, `filter` y/o `reduce` para el calculo de las sumatorias según sea necesario. 
    Considere que los puntos para el cálculo se reciben como una lista de tuplas (cada tupla es un 
    punto $(x,y)$) y $m$ es el número de tuplas en la lista.

    Considere este ejemplo del método como referencia:

    <!-- ```python -->
    $$datos = [(1, 1.3), (2, 3.5), (3, 4.2), (4, 5), (5, 7), (6, 8.8), (7, 10.1), (8, 12.5), (9, 13), (10, 15.6)]$$
    <!-- ``` -->
    $$a_0 = \dfrac{385(81) - 55(572.4)}{10(385) - (55)^2} = -0.360$$
    $$a_1 = \dfrac{10(572.4) - 55(81)}{10(385) - (55^2)} = 1.538$$
    $$y = - 0.360 + 1.538x$$
