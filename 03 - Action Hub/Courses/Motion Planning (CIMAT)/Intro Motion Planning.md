---
title: Intro Motion Planning
created: 22-01-2026 10:24
domain:
type: note
tags:
  - engineering
  - robotics
source_note:
Links to your resource note related:
---
# ⚙️ Intro Motion Planning

> **Automatic systems are characterized by being made up of a perception-decision-action cycle.

![[Perception, Desicion, Action.drawio.png|355x286]]


## 🤖 Taxonomy of Motion Planning


## ❓Keywords

* **Completeness**: A complete algorithm gives the correct answer if one exists or declares in finite time that there is not a solution if there is no solution.
	- Completeness is a **theoretical guarantee** about an algorithm’s behavior.

* **Optimality** answers the question: 
	* “Is the solution the best possible according to some criterion?” A cost function is defined, such as:
		* Path length
		* Energy consumption
		* Time
		* Risk or clearance
	* Minimum vs Maximum. 
		* Minimization: shortest path, least energy. 
		* Maximization: maximum clearance, safety margin, reward
	* Local vs Global optimality
		* Local optimum: No small change improves the solution. Common in gradient-based methods
		* Global optimum: Best solution among all feasible solutions

* Complexity, polinomial $x^n$, exponential $n^x$, $x!$, $n^{x^{x}}$.

* **Complexity** in the algorithm vs complexity in the problem. N vs NP.
* Controllability, observability, feedback.
	* Controllability
		* Can I drive the system from any initial state to any desired state using valid controls?
	* Observability
		* Can I infer the internal state from measurements?
	* Feedback
		* Control that depends on the current state or observation

* x state, y observation, u control.

* **policies** $\prod (x): x \rightarrow u$,   $y=h(x)$,   $x=h^{-1}(y)$,  $\Gamma(y):y \rightarrow u$
	* Dado a uno de esos casos, que opción voy a tomar. Dado el estado que accion voy a ejecutar.

---
