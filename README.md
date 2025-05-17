# RETO #4
En este reto tenemos como objetivo resolver los siguientes 8 problemas usando notebook de python y subirlos a un repositorio en github.
Comenzaremos con el problema 1
## Problema 1
Dado un número entero, determine si ese número corresponde al código ASCII de una minúscula vocal.

    def es_vocal_ascii(codigo):
    return codigo in [ord(v) for v in 'aeiou']
## Problema 2
Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.

    def ascii_par(c):
    if len(c) != 1:
        return "Error: cadena de longitud distinta de 1"
    return ord(c) % 2 == 0
## Problema 3
Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.

    def es_digito(c):
    return c.isdigit()
## Problema 4
Realice un programa que lea dos números reales y determine si el primero es múltiplo del segundo.

    def es_multiplo(a, b):
    if b == 0:
        return "División por cero no permitida"
    return a % b == 0
## Problema 5
Dado un número real x, construye un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:

Positivo: "El número x es positivo"
Negativo: "El número x es negativo"
Cero (0): "El número x es el neutro para la suma"

    def evaluar_signo(x):
    if x > 0:
        return f"El número {x} es positivo"
    elif x < 0:
        return f"El número {x} es negativo"
    else:
        return f"El número {x} es el neutro para la suma"
## Problema 6
Dado el centro y la radio de un círculo, determine si un punto de R2 pertenece o no al interior del círculo.


    import math

    def punto_en_circulo(cx, cy, r, px, py):
    distancia = math.sqrt((px - cx)**2 + (py - cy)**2)
    return distancia < r
## Problema 7
Dadas tres longitudes positivas, determine si con esas longitudes se puede construir un triángulo.


    def es_triangulo(a, b, c):
    return a + b > c and a + c > b and b + c > a
## Problema 8
Escriba un programa que reciba el nombre en minúsculas de un país de América y regrese la ciudad capital, si el país no pertenece al continente debe arrojar país no identificado (Utilice match-case ).

    def capital_pais(pais):
    match pais.lower():
        case "argentina":
            return "Buenos Aires"
        case "brasil":
            return "Brasilia"
        case "chile":
            return "Santiago"
        case "colombia":
            return "Bogotá"
        case "mexico":
            return "Ciudad de México"
        case "peru":
            return "Lima"
        case "venezuela":
            return "Caracas"
        case _:
            return "País no identificado"

Asi finalmente terminamos de solucionar los problemas, solo faltaria correr todos los codigos en python.
