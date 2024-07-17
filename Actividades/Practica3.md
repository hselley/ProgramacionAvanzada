---
#author: Dr. Héctor Selley
title: Práctica 3 - Programación Orientada a Objetos
fontfamily: libertinus
fontsize: 12pt
geometry: margin=3cm
papersize: letter
documentclass: scrartcl
---

Desarrolle en _Python_ los siguientes programas.

1. Escriba una clase llamada _vector_ que deberá tener dos propiedades _x_, _y_ para almacenar 
    la posición del vector en el plano cartesiano. Además debe tener un método que calcule
    la magnitud del vector, uno que determine el ángulo en radianes y otro método que determine
    el ángulo en grados. La clase debe utilizar la función _str()_ para mostrar la representación 
    del vector de la forma $(x,y)$.

    La magnitud del vector se obtiene mediante la siguiente expresión:

    $$r = \sqrt{x^2 + y^2}$$

    El ángulo se obtiene mediante la expresión:

    $$\theta = \arctan{\left(\frac{y}{x}\right)} $$

    La clase también debe utiluizar la función _add_ para la suma de vectores. Recuerde que la 
    suma de dos vectores se hace por compontentes _x_ y por componentes _y_. La suma debe devolver
    el resultado como vector en la forma $(x,y)$.

    **Ejemplo**.
    $$p = (5, -1)$$
    $$r_p = \sqrt{26}$$
    $$\theta_p = -0.1973\, \mbox{rad} = -11.30^\circ $$
    $$q = (2, -4)$$ 
    $$r_q = \sqrt{20}$$
    $$\theta_q = -1.1071\, \mbox{rad} = -63.43^\circ $$
    $$p + q = (5 + 2, -1 + (-4)) = (7, -5)$$

2. Desarrollar un mini-sistema para el registro de huespedes de un hotel. Para ello desarrolle una 
    clase _Persona_ que tenga los atributos _nombre_ y _edad_. debe tener una propiedad
    que muestre la información de la persona. Desarrolle además otra clase llamada _Huesped_ que se 
    construya a partir de la clase _Persona_ de manera que herede sus propiedades y métodos. 

    La clase _Huesped_ debe tener además sus propiedades adicionales para la información requerida:
    * Habitación (int)
    * RFC (string)
    * Número de cuenta (float)
    * Fecha de ingreso (string)
    * Hospedado actualmente (booleano)
    * Servicio a la habitación (Un diccionario donde la _llave_ es el producto y el _valor_ el costo 
    del producto)

    Además, la clase debe tener un par de métodos:
    * Mostrar información básica del huesped
    * Saldo hasta el día de hoy. Se debe considerar el costo de la renta de la habitación por los días
    que lleva hospedado y los gastos del servicio a la habitación (almacenados en el diccionario).