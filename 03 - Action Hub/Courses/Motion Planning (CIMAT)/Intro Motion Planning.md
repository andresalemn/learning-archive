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
* **Optimality**: minimum or maximum, local vs global.
* Complexity, polinomial $x^n$, exponential $n^x$, $x!$, $n^{x^{x}}$.
* **Complexity** in the algorithm vs complexity in the problem. N vs NP.
* Controllability, observability, feedback.
* x state, y observation, u control.
* **policies** $\prod (x): x \rightarrow u$,   $y=h(x)$,   $x=h^{-1}(y)$,  $\Gamma(y):y \rightarrow u$
	* Dado a uno de esos casos, que opción voy a tomar. Dado el estado que accion voy a ejecutar.

---
