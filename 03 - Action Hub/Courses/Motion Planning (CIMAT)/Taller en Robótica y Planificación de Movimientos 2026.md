
## Control visual predictivo basado en geometría multi-vista para robots autónomos
- Visual Predictive Control (MPC) against Visual Classic Control
- Applied to both DDR and Humanoid robot
- Ibero León


## Control de la deformación mediante sistemas robóticos
MIguel Aranda

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