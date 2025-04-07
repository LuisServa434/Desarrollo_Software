# A . Cuestionario
## 1) Motivaciones para la nube
- ¿Qué problemas o limitaciones existían antes del surgimiento de la computación en la nube y cómo los solucionó la centralización de servidores en data centers?
  
Antes del surgimiento de la computación en la nube, las empresas necesitaban invertir grandes cantidades en hardware, software, infraestructura física, mantenimiento,
actualizaciones constantes y personal especializado. Esto generaba altos costos y sistemas vulnerables a fallos locales.
Con la centralización de servidores en data centers y el uso de la nube, las empresas pueden escalar sus recursos según la demanda, reduciendo costos operativos y aumentando la disponibilidad.
Además, si un entorno local falla, el proceso no se detiene, ya que los servicios continúan ejecutándose.

- ¿Por qué se habla de “The Power Wall” y cómo influyó la aparición de procesadores multi-core en la evolución hacia la nube?
  
Se refiere al límite físico que enfrentaron los procesadores cuando, al aumentar la velocidad del reloj (GHz), también aumentaba el consumo de energía y la generación de calor de forma peligrosa , por este motivo
surgió la arquitectura multi-core, donde en lugar de tener un solo núcleo muy rápido, se integraron varios núcleos en un mismo chip. Así, se podían realizar más tareas al mismo tiempo . Gracias a los procesadores
multi-core, los servidores en la nube pueden manejar muchas tareas de múltiples usuarios al mismo tiempo, facilitando la virtualización, el escalado de recursos y el rendimiento necesario para servicios en línea
modernos.

## 2) Clusters y load balancing
- Explica cómo la necesidad de atender grandes volúmenes de tráfico en sitios web condujo a la adopción de clústeres y balanceadores de carga.

Cuando los sitios web empezaron a recibir mucho tráfico, un solo servidor no era suficiente para atender a todos los usuarios. Para solucionarlo, 
se comenzaron a usar clústeres de servidores, que trabajan juntos para repartir el trabajo. Además, se usan balanceadores de carga para distribuir 
las solicitudes entre los servidores del clúster, evitando sobrecargas y asegurando que el sitio funcione rápido y sin interrupciones.

- Describe un ejemplo práctico de cómo un desarrollador de software puede beneficiarse del uso de load balancers para una aplicación web.

Un desarrollador de software está construyendo una aplicación web que se espera tenga un alto volumen de usuarios, como una tienda en línea.
Sin un balanceador de carga, si demasiados usuarios acceden al mismo tiempo, el servidor podría volverse lento o incluso caerse. Usando un 
load balancer, el desarrollador puede distribuir las solicitudes de los usuarios entre varios servidores, asegurando que cada uno maneje solo
una parte del tráfico, lo que mejora el rendimiento, la disponibilidad y la escalabilidad de la aplicación.

## 3) Elastic computing
- Define con tus propias palabras el concepto de Elastic Computing.
  
- ¿Por qué la virtualización es una pieza clave para la elasticidad en la nube?
  
- Menciona un escenario donde, desde la perspectiva de desarrollo, sería muy difícil escalar la infraestructura sin un entorno elástico.

## 4) Modelos de servicio (IaaS, PaaS, SaaS, DaaS)
- Diferencia cada uno de estos modelos. ¿En qué casos un desarrollador optaría por PaaS en lugar de IaaS?
  
- Enumera tres ejemplos concretos de proveedores o herramientas que correspondan a cada tipo de servicio.

## 5) Tipos de nubes (Pública, Privada, Híbrida, Multi-Cloud)
- ¿Cuáles son las ventajas de implementar una nube privada para una organización grande?
  
-  ¿Por qué una empresa podría verse afectada por el “provider lock-in”?
  
- ¿Qué rol juegan los “hyperscalers” en el ecosistema de la nube?

# B) Actividades de investigación y aplicación

## 1)

## 2)

## 3)

## 4) Debate sobre costos

# Comparación de Tipos de Nube

| Tipo de Nube    | Costos Iniciales (CAPEX vs. OPEX)                      | Flexibilidad y Escalabilidad                     | Cumplimiento con Normativas             | Barreras/Complejidades al Cambiar de Proveedor     |
|-----------------|--------------------------------------------------------|--------------------------------------------------|------------------------------------------|-----------------------------------------------------|
| *Nube Pública* |  OPEX: Pago por uso, sin inversión inicial            |  Alta escalabilidad a demanda                   |  Depende del proveedor y región          |  Alto dependencia (vendor lock-in) si se usan servicios nativos  |
| *Nube Privada* |  CAPEX: Alta inversión en infraestructura             |  Limitada; escalar requiere más inversión       |  Control total sobre los datos          |  Menor lock-in si se usan tecnologías abiertas     |
| *Nube Híbrida* |  Mixto: inversión + operación                         |  Flexibilidad combinada con escalabilidad       |  Posibilidad de segmentar según normativa |  Complejidad técnica en interoperabilidad          |
| *Multi-Cloud*  |  OPEX: sin gran inversión inicial, pero más gestión   |  Muy alta; acceso a múltiples proveedores        |  Difícil de gestionar entre proveedores  |  Menor lock-in, pero mayor complejidad operativa   |

# C) Ejercicio de mini-proyecto
