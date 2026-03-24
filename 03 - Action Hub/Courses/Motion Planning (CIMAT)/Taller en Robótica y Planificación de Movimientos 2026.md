
## Control visual predictivo basado en geometría multi-vista para robots autónomos
- Visual Predictive Control (MPC) against Visual Classic Control
- Applied to both DDR and Humanoid robot
- Ibero León


## Control de la deformación mediante sistemas robóticos
Miguel Aranda

- Control de forma usando modelos geométricos de deformación 
- Control de forma para objetos con deformación isométrica
- Position-Based Dynamics (PBD)
- Control de forma usando As-Rigid-As-Possible (ARAP)
- Modelo de retícula tridimensional con ARAP
- Control multi-robot basado en deformación
- Transporte multi-robot con control de la deformación y restricciones de seguridad
- Control de formaciones con deformación afín

## Navegación, percepción y control de vehículos aéreos autónomos
Diego Mercado, CINVESTAV GDL

- Dron híbrido aire/agua
- Transporting a suspended payload
- Crowd analysis: automatic social distance monitoring
- Automatic monitoring social distance
- Aterrizaje autónomo. Landing avoiding people
- Robot-in-the-loop validation
- Complex urban environments. Semantic Segmentation. Risk Assessment and Risk Plane
- ViVa-SAFELAND: An Open-Source Simulation Platform for Safe Validation of Vision-Based Navigation
- Vision-Based Risk-Aware Emergency Landing in Complex Urban Environments
- Reconstrucción 3D de entornos urbanos a gran escala usando modelos fundacionales
	- 

## Seguimiento visual desde drones. Problemas reales: retardos, ruido, pérdida de características
**Fátima Oliva**, CIMAT

- Control Visual
- Modelo Cámara
	- Objeto en 3D  -> Imagen 2D sin profundidad -> Pérdida de información
	- Distorsión debida a lentes (normal, pincushion, barrel)
	- Marcadores ArUco
- Esquemas de Control . Control Servo-Visual 
	- IBVS (Image-Based Visual Servoing)
	- PBVS (Position-Based Visual Servoing)
- Ejemplo de IBVS
	- EL drone cuadri-rotor es un sistema subactuado.
	- Problemas
		- Ruido en los sensores.
		- Oclusiones o Salida del campo visual
		- Retardos en el procesamiento de la información visual
		- Inestabilidad a lazo cerrado originada por retardos
	- Control Dinámico No Lineal
	- Ardupilot + Gazebo
		- SIm2Real eficiente
		- Comunicación por medio de MAVLink
- Ejemplos de PBVS
	- Control por campos de velocidad
	- Aterrizaje con Deep learning con filtros de Kalman

## Navegación basada en retroalimentación de distancia mínima factible para un robot DDR en un entorno con obstáculos
 **Edgar Martínez**, CIMAT

- DDR robot
- Gap Navigation Tree

## Reconstrucción 4D con redes neuronales
**Edgar Sucar***, U. of Oxford

- Spatial AI
- Develop a method to get 3D dynamic reconstruction (4D) from any YouTube video.
- Dynamic Point Maps
- DUSt3R

## Causal reinforcement learning and its application to robotics
**Enrique Sucar**, INAOE

- Causal graphical models
	- Causal Bayesian Networks(CBN)	
	- Markov's Equivalence Class
- Causal models and reinforcement learning
	- An agent could learn a policy and a causal model at the same time.
	- By using a Causal Model(s)

## Un juego de vigilancia entre un robot de tracción diferencial y un perseguidor aéreo
**Ubaldo Ruiz**, CICESE

- Cops and robbers game
- Lion and man game
- Homicidal Chauffeur problem
	- Differential Games. Rufus Isaacs.

## Control de formaciones de múltiples agentes basado en orientaciones
**Frida López y Julio Rodríguez**, estudiantes de doctorado, CINVESTAV-Gdl

- Multi-agent systems (MAS)
	- Robustness
	- Scalability
	- Heterogenecity
	- Cost efficiency
- Bearing-only formation control
	- Bearing (Vectores de orientación unitarios)
	- Ensure a group of agents maintains a desired geometric pattern.
- Oriented graph

##  Research trends in automotive industry
 **Cesar Magaña**, Aumovio
- Aumovio
- EP-Diffuser. An Efficient Diffusion Model for Traffic Scene Generation and Prediction via Polynomial Representation
- Setup
	- Train on Argoverse
	- Test on Waymo
- Current problems of interest
	- Neural Network Quantization
	- Sensor Data Fusion
	- Safe AI for Automated Driving
	- Autonomous Driving (KI Wissen)
	- Explainability for  validation of AI applications (AIDE-X)
	- Ethical and Responsible AI. _Ethical and Trustworthy Artificial and Machine Intelligence_ (etami).
	- FALCON Project - Image Captioning/Scene Graph Generation
	- Automated Sensor Calibration
	- LiDAR Object Detection
	- Training and Evaluation
	- Intelligent Infrastructure

##  Swarm-SLAM: cien agentes, un modelo emergente, cero mapas prefabricados
**Carlos Lara**, CIMAT

- Evolución del problema del SLAM
	- EFK-SLAM (1985)
	- Mapas de ocupación de celdillas (1990)
	- EKF-SLAM (1991-1995) Matemáticamente sólido
- NERF (Neural Radiance Fields)
	- Generar vistas nuevas de una escena a partir de un conjunto limitado de imágenes.
- BARF (Bundle-Adjusting Neural Radiance Fields)
	- Extensión de NeRF, que permite reconstruir
- Swarm SLAM
	- Mandar varios drones requiere ancho de banda amplio, los errores se van generando y hay falta de consenso. 
- MNE SLAM
	- En lugar de intercambiar fotos, los drones solo comparten pequeñas "redes cerebro" que resumen lo que ham visto. 
	- MNE-SLAM: Multi-Agent Neural SLAM for Mobile Robots
- Ultra-Lightweight C-SLAM
	- Lograr localización y mapeo precisos de un entorno desconocido con NANO drones.
	- Restricciones de hardware (memoria y capacidad de cálculo)
- Retos para Swarm SLAM
	1. Pequeños errores de pose causan grandes inconsistencias fotométricas
	2. Saturan la red Wi-Fi con solo 3 robots
	3. Consenso sobre la estructura del mapa sin sincronización ni servidor central
	4. En enjambres heterogéneos
	5. Robustez ante fallos
	6. Falta de validación en enjambres grandes
- Aprendizaje de recompensas basado en LLMs
	- Entornos condicionados por lenguaje
	- Entornos basados en texto
- MARL para tareas de Largo Horizonte en Equipos de Robots Heterogéneos

## Beyond geometric patterns: The evolution of coverage path planning in the machine learning era
 **Irving Vasquez**, IPN

- Coverage path planning. Addressed as region filling problem
	- NP-Hard problem complexity
- The Boustrophedon path
	- Simplifies the planning
	- Both convex and non convex regions
