# kurbernetes 🎛️
Si un Pod falla ❗, Kubernetes puede crear uno nuevo para reemplazarlo, siguiendo las directrices de los controladores de nivel superior. Esto contribuye a la resiliencia y disponibilidad de las aplicaciones en el clúster.
# Pods
- Es la unidad con la que trabaja kubernetes
- Contiene un conjunto de contenedores.
- los cotenedores dentro de un mismo pod comparten red 🕸️, almacenamiento 🏬 y recursos.
# ReplicaSets
- Es un controlador que garantiza que un número específico de réplicas (copias) de un Pod esté en funcionamiento en todo momento en el clúster.
- Los ReplicaSets son una forma de asegurarse de que la aplicación se esté ejecutando con la cantidad deseada de instancias, lo que proporciona escalabilidad y alta disponibilidad
- Stateless
- Escalado
+ En Kubernetes, el escalado horizontal 🌅 se logra mediante la creación o eliminación de réplicas ©️ de un conjunto de Pods que ejecutan la misma aplicación.
+ El escalado horizontal permite utilizar los recursos disponibles de manera más eficiente, ya que puedes distribuir la carga en varias instancias en lugar de depender de una sola instancia con recursos más grandes.
- Respuesta a fallo
# Services 
Es un objeto que define una forma de acceder a una o varias instancias de Pods.
- permite que las aplicaciones en el clúster se comuniquen entre sí y con el mundo exterior de manera confiable y predecible.
Funciones ▶️
- Balanceo de carga: Los Servicios pueden distribuir el tráfico de red entrante entre las diferentes réplicas de Pods.
- Estabilidad de la dirección IP: Los Servicios tienen direcciones IP virtuales que persisten a lo largo de la vida útil de la aplicación.
# Tipos de Servicios: 
- ClusterIP
- NodePort
- LoadBalancer
# Healthchecks
Son especialmente relevantes para garantizar la disponibilidad y el rendimiento 📋 de las aplicaciones que se ejecutan en contenedores 🐳
Tipos de healthchecks:
  - Liveness Probe (Sonda de Vida) : verifica si un contenedor está vivo y funcionando.
  - Readiness Probe (Sonda de Preparación):  Una Readiness Probe verifica si un contenedor está listo para        recibir tráfico.
  - Startup Probe (Sonda de Inicio): Verifica si un contenedor ha terminado de inicializarse y está listo         para manejar solicitudes. Esto es útil cuando los contenedores pueden requerir más tiempo para                inicializarse.
# Ingress controller:
componente crucial para administrar la exposición y el enrutamiento de servicios HTTP y HTTPS de manera más flexible y estructurada, lo que facilita la administración de la entrada de tráfico a las aplicaciones en el clúster.
  
