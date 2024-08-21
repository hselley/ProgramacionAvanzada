---
#author: Dr. Héctor Selley
title: Práctica 6 - Listas por comprensión
fontfamily: libertinus
fontsize: 12pt
geometry: margin=3cm
papersize: letter
documentclass: scrartcl
---

Desarrolle en _Python_ los siguientes programas.

1. Ejercicio: Dadas dos listas de números, por ejemplo [1, 2, 3] y [4, 5, 6], genera 
    una nueva lista que contenga el producto de los elementos correspondientes.

2. Dada una lista de diccionarios que representan personas con claves "nombre", "edad" y "ciudad",      
    genera una nueva lista de nombres de personas que tengan más de 30 años y vivan en "Madrid".

    Ejemplo: Para la lista `[{"nombre": "Ana", "edad": 25, "ciudad": "Madrid"}, {"nombre": "Juan", "edad": 35, "ciudad": "Madrid"}, {"nombre": "Luis", "edad": 32, "ciudad": "Barcelona"}]`, 
    el resultado debería ser ["Juan"].

3.  Dada una lista de listas de números, utiliza una expresión generadora para calcular la media 
    de todos los números. 
    
    Ejemplo: Para la lista [[1, 2, 3], [4, 5], [6, 7, 8]], el resultado debería ser 4.5.

4.  Utiliza una expresión generadora para calcular la varianza de una lista de números. 
    La varianza se calcula como la media de los cuadrados de las diferencias con la media.
    
    Ejemplo: Para la lista [1, 2, 3, 4, 5], el resultado debería ser 2.0.