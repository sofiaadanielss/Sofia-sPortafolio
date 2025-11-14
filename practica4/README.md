# PRACTICA 4 - PARADIGMA LOGICO

## Paradigma Logico

La programación en paradigma lógico es un estilo de programación basado en la lógica formal, donde los programas se escriben como un conjunto de hechos y reglas en lugar de una secuencia de comandos. Es un paradigma declarativo, lo que significa que el programador describe cuál es el problema y cuál es el objetivo, sin especificar las instrucciones paso a paso. El sistema utiliza la inferencia lógica para encontrar una solución razonando sobre los hechos y las reglas.

### Características clave

* Hechos y reglas: Los programas constan de una base de conocimiento compuesta por enunciados lógicos.

* Hechos: Enunciados simples que son verdaderos, como «padre(john, jane)».

* Reglas: Enunciados condicionales que afirman que una conclusión es verdadera si se cumple un conjunto de condiciones, como «abuelo(X, Y) :- padre(X, Z), padre(Z, Y)».

* Enfoque declarativo: Se describe el problema y sus relaciones, y el sistema determina cómo resolverlo, a diferencia de un lenguaje imperativo donde se debe especificar cada paso.

* Inferencia: La ejecución del programa implica inferencia lógica, donde el sistema utiliza reglas y hechos para responder consultas y encontrar demostraciones.

* Prolog: El lenguaje más conocido para este paradigma es Prolog, que se utiliza en áreas como la inteligencia artificial y los sistemas de bases de datos.

## Programación con Prolog.

Prolog (Programación Lógica) es un lenguaje de programación declarativo y lógico desarrollado a principios de la década de 1970. Es conocido principalmente por su uso en inteligencia artificial, sistemas expertos y procesamiento del lenguaje natural.

## Características clave:
Paradigma declarativo: A diferencia de los lenguajes imperativos que especifican cómo obtener un resultado, Prolog se centra en describir el problema mediante hechos y reglas. El sistema utiliza la inferencia lógica para encontrar soluciones.

* Hechos: Representan verdades básicas o relaciones entre objetos. Por ejemplo, `friends(raju, mahesh)` indica que Raju y Mahesh son amigos.

* Reglas: Definen relaciones lógicas que permiten inferir nuevos hechos a partir de los existentes. Por ejemplo, `parent(X, Y) :- father(X, Y)` significa que X es padre de Y si X es padre de Y.

* Consultas: Se utilizan para formular preguntas sobre los hechos y reglas definidos. El intérprete de Prolog intenta encontrar soluciones comparando la consulta con la base de conocimiento.

* Unificación: Mecanismo fundamental donde Prolog intenta igualar términos asignando valores a variables.

* Retroceso: Cuando falla un objetivo, Prolog retrocede automáticamente a un punto de decisión anterior y prueba una ruta alternativa para encontrar una solución.

* Recursión: Mecanismo principal de iteración y búsqueda en Prolog. La optimización de llamadas de cola permite la ejecución eficiente de predicados deterministas recursivos de cola.