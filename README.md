## Instructions

Contexto:
En el proyecto de Norden surgio el requerimiento de calcular el balance de un equipo de trabajo, tomando como base el seniority de cada integrante del mismo.
El balance de un equipo esta dado por los integrantes del mismo, entre el nivel de seniority de los colaboradores, un equipo 100% balanceado es aquel en el cual el 50% de sus integrantes son juniors, el 30% son mids y le 20% son seniors
Ejemplo:
- para un equipo de 10 colaboradores, 5 de ellos son junior, 3 son mid y 2 son senior >> este equipo esta balanceado al 100%
- Para un equipo de 5 colaboradores, 3 mids y 2 seniors >>  tiene un balance del 34%

## COnsideraciones

* La clase TeamBalanceService se dispara cuando ciertas reglas de negocio se cumplen, y su unica responsabilidad es obtener el balance de un equipo, cuyo id es pasado como parametro (el resultado representa el %).
* La clase TeamRepository es la que se encarga de hacer las consultas a la base de datos, cada una de las consultas aqui utilizadas nos devolveria un array de colaboradores, para fines del ejercicio se esta reemplazando por un array simple.
* Actualmente las pruebas estan fallando ya que el algoritmo para calcular este balance es incorrecto (error presente en el proyecto al momento de la captura del ejemplo).
* No hay ningun requerimiento especifico para la clase TeamBalanceService, la unica condicional es que entrgue el balance de un equipo dado.
* No hay limite en la cantindad de integrantes de un equipo, puede ser desde 1 hasta N.
* No importa el rol de los integrantes del equipo, solo su seniority.
* Sientete libre de agregar tantas pruebas como necesites para tus testcases.


## Preguntas a discutir
- Utilizarias alguna otra herramienta diferente de un service? cual?
- Modificarias de alguna manera la clase TeamRepository?
- Suponiendo que el algoritmo estubiera correcto, que issues podria generar si se deja el codigo tal y como esta?