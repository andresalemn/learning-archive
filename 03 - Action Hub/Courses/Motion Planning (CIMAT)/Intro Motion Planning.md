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
## 🎯 Goal of Motion Planning

* Compute **motion strategies**
	* geometric paths
	* time-parameterized trajectories
	* sequence of sensor-based motion commands
* To achieve **high-level goals**:
	* go to A without colliding with obstacles
	* assemble product P
	* build map of environment E
	* find object O

## 🤖 Basic Motion Planning Problem

> Compute a **collision-free path** for a rigid or articulated object among static obstacles.

* Inputs:
	* Geometry of moving object and obstacles.
	* Kinematics of moving object (degrees of freedom)
	* Initial and goal **configurations** (placements)
* Outputs:
	* Continuous sequence of collision-free robot configurations connecting the initial and goal configurations.

### ➕ Extensions of Basic Problem

|                                                                                                             |                                                                       |
| ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| Moving obstacles                                                                                            | Optimal planning                                                      |
| Multiple robots                                                                                             | Uncertainty in model, control and sensing                             |
| Movable objects                                                                                             | Exploiting task mechanics (sensorless motions, underactuated systems) |
| Assembly planning                                                                                           | Physical models and deformable objects                                |
| Goal is to acquire information by sensing:<br>- Model building<br>- Object finding/tracking<br>- Inspection | Integration of planning and control                                   |
| Nonholonomic constraints                                                                                    | Integration with higher-level planning                                |
| Dynamic constraints                                                                                         | Stability constraints                                                 |

### 🔎 Applications

- Lunar vehicle (Athlete, NASA/JPL)
- Dexterous Manipulation
- Manipulation of Deformable Objects
- Animation of Crowds
- Radiosurgical Planning
- Building Code Verification
- Egress Simulations
- Transportation of A380 Fuselage trough Small Villages

Gradiente. Vector con magnitud y orientación


 