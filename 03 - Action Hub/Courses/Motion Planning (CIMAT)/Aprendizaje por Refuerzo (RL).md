## Introducción 
-  Inteligencia Artificial -> Aprendizaje Máquina -> Aprendizaje Por Refuerzo
-  El RL se centra en cómo un agente debe actuar en un entorno.
- El objetivo es aprender a mapear situaciones a acciones para maximizar una señal de recompensa numérica (el retorno).
## Elementos
- Ciclo de aprendizaje
	1. El Agente toma una observación del ambiente
	2. El agente envía una acción al ambiente para modificarlo en modo favorable
	3. EL ambiente transita a un estado siguiente como consecuencia de la acción realizada por el agente y el estado anterior.
	4. El agente recibe una observación y una recompensa que utiliza para mejorar en la tarea.
* Componentes
	* Agente
	* Ambiente
	* La política $\pi (\cdot)$ 

-  La política $\pi (s)$ ->  Acción tomada en el estado $s$ bajo una política determinista.
- La probabilidad 
## Programación Dinámica
- Nota histórica: En 1949 el matemático estadounidense Richard Bellman trabajaba como colaborador de la corporación RAND donde tenia como propósito abordar problemas de planificación militar. 
- Bellman por sugerencia del también matemático Edwin Paxson empezó a trabajar en problemas de decisión Multi-etapa, es decir problema donde la solución es una secuencia de decisiones tomadas en instantes de tiempo, en la que en cada instante o etapa se tiene acceso a un cierta información 8,; la decisión d se toma en base a esta información.
- La función $f(\cdot)$ es la función de costo/beneficio que resulta

## Procesos de decisión de Markov

- Ejemplo: Lago Congelado

## Método del gradiente de la política

- Monte-Carlo Policy-Gradient Control (episodic) for $\pi$
