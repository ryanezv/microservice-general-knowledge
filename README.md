## # Introducción

#### **¿Qué son los microservicios?**

- **Descomposición**: Dividir un problema de software en partes más pequeñas que son faciles de entender y resolver
- **Soporte al desarrollo políglota:** Pueden ser escritos en diferentes lenguajes de programación usando distintas técnologias y facil de comunicarse entre ellos.
- **Todas las comunicaciones sobre REST:** Esto es igual a **agilidad**, por que los desarrolladores de sofware no tienen que entender otro framework o tecnología para llamar a otro servicio.
- **Autodescubrimiento "self-service":** Contratos y limites bien definidos habilitan el autodescubrimiento.
#### *Los beneficios más valuables de esta arquitectura son:*
- Agilidad
- Escalabilidad
- Distribución

#### *Migrar de monolitos a microservicios implica:*
- Incrementar las comunicaciones de red, mayor latencia (COSTO)
- Pasar de pocos artefactos de despliegue a muchos artefactos "pequeños" (COSTO)

## # Conceptos Base

**ACID**

**API Layer**


**Cloud Native**

Frecuentemente cuando la gente escucha "CLOUD", ellos asumen AWS, GCP, Azure, etc., sin embargo, esta solo es una parte de la historia.

*Twelve-factor app**

Es una metodología para construir aplicaciones SaaS Software as a Services y puede ser aplicada a cualquier componente de desarrollo de software, sin importar la tecnología o lenguaje de programación. Puedes leer más aquí https://12factor.net/es/

## # Conceptos Avanzados

Comunicación asincrona

Logging and tracing

**Circuit braker**

Este patrón es especial para definir una logica de tiempo de espera solida entre microservicios y ayuda a evitar los bloqueos "gridlock" en tu sistema

**Design a microservices**

**Continuoud delivery**

DevOps
