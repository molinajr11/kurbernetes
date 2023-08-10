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
  
