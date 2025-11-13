# Practica 3 — Haskell 

Haskell es un lenguaje de programación funcional, a diferencia de C, que es imperativo.

En C, el programador describe paso a paso cómo se hace algo.

En Haskell, el programador describe qué es el resultado, y el lenguaje se encarga del “cómo”.

Esto cambia varias cosas importantes:

## C	 vs. 	Haskell

Variables cambian de valor | Los valores son inmutables
Se usan ciclos (for, while) | Se usa recursión o funciones como map, filter, fold
Las funciones pueden tener efectos secundarios | Las funciones son puras (mismo input → mismo output)
Se maneja memoria manualmente | La administración es automática (garbage collector)


## Tipos

En Haskell, el compilador deduce los tipos.
Pero también se pueden especificar:

suma :: Int -> Int -> Int
suma a b = a + b


Esto significa:

suma es una función que recibe dos Int y regresa un Int.


Listas

Las listas son fundamentales:

numeros = [1, 2, 3, 4]


Y puedes usar funciones sobre ellas:

dobles = map (*2) numeros


Esto produce:

[2,4,6,8]


Recursión en lugar de ciclos

C:

int sum(int a[], int n) {
    int total = 0;
    for(int i=0; i<n; i++) {
        total += a[i];
    }
    return total;
}


Haskell:

sumar [] = 0
sumar (x:xs) = x + sumar xs


## Archivos
- `hello.hs` — imprime un saludo y una lista de numeros impares.

## Proposito
Demuestra IO basico y el procesamiento de listas en Haskell (filtrando los numeros impares).

## Como correr:
- Usando runhaskell:
  runhaskell hello.hs

- Compilando con GHC:
  ghc -o hello hello.hs
  ./hello        (en Windows: hello.exe)

## Resultado esperado
Hello, everyone!!!
Please look at my favorite odd numbers: [11,13,15,17,19]