---
#author: Dr. Héctor Selley
title: Práctica 4 - Métodos Mágicos
fontfamily: libertinus
fontsize: 12pt
geometry: margin=3cm
papersize: letter
documentclass: scrartcl
---

Desarrolle en _Python_ los siguientes programas.

1. Implemente una clase `Rectangulo` que represente un rectángulo y que tenga dos atributos
    `base` y `altura`. Use `__eq__` para comparar si dos rectángulos son iguales (misma base y 
    altura) y `__ne__` para verificar si son diferentes. Utilice los métodos `__gt__` y `__lt__`
    para comparar el área de dos rectángulos, devuelva `True` o `False` según sea el caso.

2. Implemente una clase `Playlist` que tenga una lista de sus canciones favoritas. Use el 
    método `__len__` para devolver el número de canciones mediante el llamado `len(miLista)`.
    Utilice además el método `__getitem__` para devolver una canción de la lista de acuerdo al 
    argumento recibido en el método. Finalmente utilice `__setitem__` para establecer una nueva 
    canción en la posición indicada, ambos pasados como argumentos del método.