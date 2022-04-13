## # Introducción

#### **Normalmente cuando hablamos de Microservicios, nos referimos a:**

- **Descomposición**: Dividir un problema de software en partes más pequeñas que son faciles de entender y resolver.
- **Desarrollo  de sofware políglota:** Pueden ser escritos en diferentes lenguajes de programación usando distintas técnologias, frameworks. Puedes aprovechar técnologias emergentes.
- **Todas las comunicaciones son sobre REST:** Esto es igual a **agilidad**, por que los desarrolladores de sofware no tienen que entender otro framework o tecnología para llamar a otro servicio.
- **Enfoque a productos** de software, no como proyectos. 
- **Self-service:** Contratos e interfaz bien definidos habilitando así el autodescubrimiento de los microservicios.

#### *Los beneficios más valuables de esta arquitectura son:*
- Agilidad
- Escalabilidad
- Distribución

#### *Consideraciones fundamentales de diseño en una arquitectura de Microservicios:*

- **CI / CD pipelines**, primer aspecto de tu diseño. Si no cuidamos el continuos delivery, el despliegue de muchos microservicios puede ser una pesadilla.
- **Logging and tracing** framework, segundo aspecto de tu diseño. Una buena estrategia de logging te ayudará a las operaciones de día a día, solución de problemas "troubleshooting", mantenimiento, investigaciones y otras tareas generales.
- Considerar **DDD Domain Driven Design** para el diseño y codificación de tus servicios. 
- Considerar **Circuit Braker Pattern** ayudando a evitar los bloqueos "gridlock" en tu sistema y definiendo una logica de tiempo de espera solida entre la comunicación de los servicios.
- **STLC "Sofware Testing Life Cycle"** para asegurar la calidad de tu software.


#### *Migrar de monolitos a microservicios implica:*
- Incrementar las comunicaciones de red, mayor latencia (COSTO)
- Pasar de pocos artefactos de despliegue a muchos artefactos "pequeños" (COSTO)


## # Conceptos Base

**ACID**

ACID se refiere a 4 propiedades que garantizan que las transacciones se realicen de forma confiable:

**1. Atomic:** Tiene exito o falla por completo, es decir, no hay área gris.
**2. Consistent:** Garantiza que aplicará todas las restricciones o reglas del modelo de datos
**3. Isolated:** Asegura que no puede ser leído por otras transacciones hasta que se encuentre en un estado específico basado en reglas de aislamiento.
**4. Durable:** Asegura que una vez guardado, se garantiza que estará en la base de datos hasta que se modifique.

--


**API Layer**

Deberia solo ser usada como "proxy-layer". O al implementar soluciones más completas como Google APIGEE y extender sus capacidades y beneficios.

**Cloud Native**

Frecuentemente cuando la gente escucha "CLOUD", piensan rapidamente en AWS, GCP, Azure, etc., sin embargo, esta solo es una parte de la historia.

Cloud Native se trata sobre como se crean e implementan las aplicaciones, no donde se ejecutan

CNFC Cloud Native Landscape: 


**Twelve-factor app**

Es una metodología para construir aplicaciones SaaS Software as a Services y puede ser aplicada a cualquier componente de desarrollo de software, sin importar la tecnología o lenguaje de programación. Puedes leer más aquí https://12factor.net/es/

**API Rest**

Recursos (Resources)

- Los **recursos** son el pilar de sistemas basados en la web, incluso a menudo la Web es referida como **"resource-oriented"**
- Un recurso basicamente es cualquier cosa que expones en la Web, puede ser un documento, un video, un servicio, un servidor de contenido multimedia, etc.
- Para identificar un recurso en la red, la Web proporciona el URI Uniform Resource Identifier y de esta forma tener un medio para manipularlo usando un protocolo como HTTP.
- Una URI identifica un y solo un recurso en la red.


## # Conceptos Avanzados

Comunicación asincrona

Logging and tracing

**Circuit braker**


**Design a microservices**

**DevOps**

Hay tres aspectos importantes en DevOps:

1. **Continuous Integration (CI):** Es la practica de enviar frencuentemente cambios al codigo fuente y lanzar un compilación automatica que valida el código en varios sentidos: compilation errors, dependencies missing, automated test, static code analisys, etc.
2. **Continuous Delivery (CD):** Es la capacidad de mantener siempre un producto en estado estable despues de cada cambio y este listo para ser enviado a los consumidores.
3. **Continous Deployment:** Automaticamente desplegar el product increment a producción.
