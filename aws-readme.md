# AWS Cloud Practitioner Study Guide

## Módulo 1: Introducción a AWS

### Equipo de Instructores
- **Roberto**: Instructor con experiencia en arquitectura en la nube, bases de datos, big data y seguridad
- **Mar**: Especialista en procesamiento de lenguaje natural e instructora técnica
- **Vicente**: Ingeniero informático con más de 20 años de experiencia

### Servicios de AWS
- Amplia gama de servicios desde básicos hasta avanzados
- Soluciones de computación, almacenamiento y seguridad de red
- Servicios especializados como blockchain, machine learning, IA y desarrollo de robots
- Herramientas específicas para administración, producción de vídeo y satélites orbitales

### Modelo Cliente-Servidor
- Concepto básico explicado mediante la analogía de una cafetería
- Cliente: Hace solicitudes (como un navegador web o aplicación de escritorio)
- Servidor: Responde a las solicitudes (como Amazon EC2)

### Modelo de Precios
- Principio fundamental: "Pago por uso"
- Solo se paga por los recursos cuando se utilizan
- Escalabilidad flexible según demanda
- No requiere pago por adelantado
- Eliminación de costos por capacidad no utilizada

### Beneficios Clave
- Flexibilidad en la capacidad de recursos
- Modelo de costos eficiente
- Escalabilidad instantánea según necesidades
- Sin compromiso de capacidad a largo plazo

## Módulo 2: Computación en la Nube

### Modelos de Despliegue

#### Basado en la Nube
- Ejecución completa de aplicaciones en la nube
- Opción de migrar aplicaciones existentes
- Posibilidad de crear nuevas aplicaciones directamente
- Uso de infraestructura de bajo nivel o servicios de nivel superior

#### En las Instalaciones (Nube Privada)
- Despliegue local de recursos
- Uso de herramientas de virtualización
- Similar a IT heredada pero con mejor utilización de recursos

#### Híbrido
- Combinación de recursos en la nube y locales
- Útil para mantener aplicaciones heredadas
- Ideal para cumplimiento regulatorio
- Permite aprovechar servicios cloud manteniendo sistemas locales

### Beneficios de la Computación en la Nube

#### Financieros
- Conversión de gastos iniciales a variables
- Pago solo por recursos utilizados
- Beneficios de economías de escala
- Reducción de costos operativos de centros de datos

#### Operativos
- Eliminación de gestión de centros de datos
- Sin necesidad de predecir capacidad
- Escalabilidad según demanda
- Mayor velocidad y agilidad en el desarrollo

#### Estratégicos
- Enfoque en aplicaciones y clientes en lugar de infraestructura
- Capacidad de experimentación e innovación
- Despliegue global rápido
- Baja latencia para clientes globales

### Amazon EC2

#### Conceptos Básicos
- Proporciona capacidad de computación en la nube
- Funciona bajo el modelo cliente-servidor
- Ofrece servidores virtuales flexibles y escalables
- Permite ejecutar aplicaciones empresariales de cualquier tipo

#### Ventajas sobre Infraestructura Tradicional
- No requiere inversión inicial en hardware
- Eliminación de esperas por entrega de equipos
- Sin necesidad de instalación física
- Aprovisionamiento en minutos vs semanas/meses
- Pago solo por uso activo
- Sin compromiso de recursos a largo plazo

#### Aspectos Técnicos
- Utiliza tecnología de virtualización
- Implementa multitenencia mediante hipervisor
- Aislamiento seguro entre instancias
- Comparte recursos físicos de manera eficiente
- AWS gestiona la infraestructura subyacente

### Tipos de Instancias EC2

#### Propósito General
- Equilibrio entre computación, memoria y redes
- Casos de uso:
  - Servidores de aplicaciones
  - Servidores de juegos
  - Backend empresarial
  - Bases de datos pequeñas/medianas

#### Computación Optimizada
- Enfocadas en procesamiento de alto rendimiento
- Casos de uso:
  - Servidores web de alto rendimiento
  - Servidores de juegos dedicados
  - Procesamiento por lotes

#### Optimización de Memoria
- Diseñadas para procesar grandes conjuntos de datos en memoria
- Casos de uso:
  - Bases de datos de alto rendimiento
  - Procesamiento en tiempo real
  - Análisis de datos no estructurados

#### Computación Acelerada
- Utilizan aceleradores de hardware/coprocesadores
- Casos de uso:
  - Cálculos de punto flotante
  - Procesamiento de gráficos
  - Streaming de juegos y aplicaciones

#### Optimizadas para Almacenamiento
- Alto rendimiento en lectura/escritura secuencial
- Casos de uso:
  - Sistemas de archivos distribuidos
  - Almacenamiento de datos
  - Procesamiento OLTP de alta frecuencia

### Opciones de Precios EC2

#### Instancias Bajo Demanda
- Pago solo por tiempo de uso (por hora o segundo)
- Sin compromiso a largo plazo
- Sin pagos adelantados
- Ideal para:
  - Pruebas iniciales
  - Cargas de trabajo irregulares
  - Desarrollo y pruebas
  - Patrones de uso impredecibles

#### Savings Plans
- Ahorro hasta 72% con compromiso de uso
- Términos de 1 o 3 años
- Flexible para diferentes familias de instancias, regiones y sistemas operativos
- Aplicable también a Fargate y Lambda

#### Instancias Reservadas
- Ahorro hasta 75% vs precio bajo demanda
- Opciones de pago:
  - Pago total anticipado
  - Pago parcial anticipado
  - Sin pago inicial
- Tipos:
  - Standard (menor flexibilidad, mayor ahorro)
  - Convertible (mayor flexibilidad)
- Compromiso de 1 o 3 años

#### Instancias Spot
- Ahorro hasta 90% del precio bajo demanda
- AWS puede recuperar la instancia con 2 minutos de aviso
- Ideal para:
  - Cargas interrumpibles
  - Procesamiento por lotes
  - Trabajos flexibles en tiempo

#### Hosts Dedicados
- Servidores físicos dedicados
- Uso exclusivo del hardware
- Ideal para:
  - Cumplimiento normativo
  - Licencias específicas
- Opción más costosa

### Escalabilidad y Amazon EC2 Auto Scaling

#### Problemática Tradicional
- Los centros de datos físicos enfrentan dilemas de capacidad
- Fluctuación de cargas de trabajo en el tiempo
- Dilema entre comprar para uso medio o para carga máxima

#### Solución AWS
- Aprovisionamiento exacto según demanda
- Capacidad ajustable las 24 horas
- Balance entre satisfacción del cliente y eficiencia de costos
- Sistema de alta disponibilidad sin puntos únicos de fallo

#### Amazon EC2 Auto Scaling
- Ajuste automático del número de instancias
- Respuesta a demanda cambiante
- Estrategias principales:
  - Escalado Dinámico: responde a cambios en tiempo real
  - Escalado Predictivo: programa recursos según demanda prevista

### Elastic Load Balancing (ELB)
- Distribuye automáticamente el tráfico entrante
- Actúa como punto único de contacto
- Integración con Auto Scaling
- Garantiza alto rendimiento y disponibilidad

### Servicios de Mensajería

#### Amazon SQS (Simple Queue Service)
- Servicio de cola de mensajes
- Permite enviar, almacenar y recibir mensajes entre componentes
- Funciona como buffer entre aplicaciones
- Escalado automático y alta fiabilidad

#### Amazon SNS (Simple Notification Service)
- Sistema de publicación/suscripción (pub/sub)
- Permite crear "temas" para enviar mensajes
- Notifica a múltiples suscriptores simultáneamente
- Soporta múltiples tipos de suscriptores:
  - Colas SQS
  - Funciones Lambda
  - Enlaces web HTTPS/HTTP
  - Notificaciones a usuarios (SMS, email, push móvil)

### Computación Sin Servidor y Contenedores

#### AWS Lambda
- Permite ejecutar código sin gestionar servidores
- El usuario solo se centra en el código
- Escalado automático según necesidad
- Pago por uso (solo cuando el código se ejecuta)

#### Contenedores
- Método para empaquetar código y dependencias
- Garantiza consistencia entre diferentes entornos
- Incluye aplicaciones, bibliotecas, SO y servidor

#### Servicios de Contenedores AWS
- **Amazon ECS (Elastic Container Service)**:
  - Sistema de gestión de contenedores escalable
  - Compatible con Docker
  - Permite iniciar/detener aplicaciones Docker

- **Amazon EKS (Elastic Kubernetes Service)**:
  - Servicio administrado para Kubernetes
  - Permite gestionar contenedores a gran escala
  - Mantenido por una comunidad activa
  - Actualizaciones automáticas

- **AWS Fargate**:
  - Motor de computación sin servidor para contenedores
  - Compatible con ECS y EKS
  - Elimina necesidad de gestionar servidores
  - Pago por recursos utilizados

## Módulo 3: Infraestructura Global

### Infraestructura Global AWS
- AWS tiene centros de datos agrupados en "regiones" globalmente
- Las regiones están conectadas por red de fibra de alta velocidad
- Cada región tiene múltiples centros de datos
- Proporciona redundancia y protección contra desastres
- Ofrece aislamiento entre regiones por defecto

### Factores para Seleccionar Región

#### Conformidad y Regulaciones
- Prioridad máxima en la selección
- Algunas empresas deben cumplir requisitos específicos de ubicación de datos
- Las regiones respetan leyes y normativas locales

#### Proximidad a Clientes
- Impacta en la latencia del servicio
- La distancia física afecta la velocidad de respuesta
- Importante para aplicaciones que requieren baja latencia

#### Servicios Disponibles
- No todas las regiones tienen todos los servicios
- Los nuevos servicios se despliegan gradualmente
- El hardware específico puede limitar disponibilidad

#### Precios
- Varían según la región
- Influenciados por costos locales y fiscalidad
- Pueden existir diferencias significativas

### Zonas de Disponibilidad (AZ)

#### Concepto
- Una AZ es un centro de datos o grupo de centros de datos dentro de una región
- Cada región tiene múltiples AZ (ejemplo: us-west-1a, 1b, 1c)
- Cada AZ tiene alimentación, redes y conectividad redundante

#### Diseño y Distribución
- Las AZ están separadas físicamente
- Suficientemente cercanas para baja latencia (<10ms)
- Suficientemente lejanas para aislamiento de desastres
- Conectadas entre sí con alta velocidad

### Ubicaciones Periféricas y CloudFront

#### Ubicaciones Periféricas
- Sitios distribuidos globalmente
- Independientes de las regiones AWS
- Diseñadas para acercar contenido a usuarios finales
- Solución para clientes geográficamente dispersos

#### Amazon CloudFront (CDN)
- Servicio de red de entrega de contenido
- Beneficios:
  - Baja latencia
  - Altas velocidades de transferencia
  - Distribución global
- Usos:
  - Entrega de datos
  - Streaming de video
  - Aplicaciones
  - APIs

### Interacción con AWS

#### Consola de Administración AWS
- Interfaz web interactiva
- Características:
  - Acceso rápido a servicios recientes
  - Búsqueda por nombre/palabra clave/acrónimo
  - Asistentes y flujos automatizados
- Versión móvil disponible

#### AWS Command Line Interface (CLI)
- Interfaz por línea de comandos
- Disponible para Windows, macOS y Linux
- Ideal para automatización y scripts

#### Software Development Kits (SDK)
- APIs para diferentes lenguajes de programación
- Integración con aplicaciones existentes
- Documentación completa
- Soporte para múltiples lenguajes

### Herramientas de Administración Avanzada

#### AWS Elastic Beanstalk
- Servicio para aprovisionar entornos EC2
- Despliegue automatizado
- Ajuste de capacidad automático
- Monitoreo integrado

#### AWS CloudFormation
- Infraestructura como código (IaC)
- Plantillas en JSON o YAML
- Aprovisionamiento en paralelo
- Soporte multi-región y multi-cuenta

## Módulo 4: Redes

### VPC (Virtual Private Cloud)

#### Conceptos Fundamentales
- Red privada virtual dentro de AWS
- Permite definir rangos de IP privadas
- Recursos organizados en subredes

#### Tipos de Acceso y Conectividad
- **Internet Gateway (IGW)**:
  - Permite acceso público desde internet
  - Necesaria para recursos públicos
- **Virtual Private Gateway**:
  - Permite conexiones VPN
  - Usa internet público con conexión cifrada
- **AWS Direct Connect**:
  - Conexión física dedicada
  - Menor latencia y mayor seguridad

### Seguridad en VPC

#### ACL de Red (NACL)
- Actúa a nivel de subred
- Sin estado (stateless)
- Verifica cada paquete
- No recuerda decisiones previas

#### Grupos de Seguridad
- Actúa a nivel de instancia EC2
- Con estado (stateful)
- Por defecto:
  - Bloquea todo el tráfico entrante
  - Permite todo el tráfico saliente
  - Permite tráfico de retorno

### DNS y Amazon Route 53

#### DNS (Sistema de Nombres de Dominio)
- Traduce nombres de dominio a direcciones IP
- Funciona como "guía telefónica" de Internet

#### Amazon Route 53
- Servicio DNS web de AWS
- Enruta usuarios a aplicaciones
- Gestiona registros DNS
- Permite registrar nuevos dominios
- Soporta transferencia de dominios existentes

## Módulo 5: Almacenamiento

### Almacenamiento en Bloques

#### Volúmenes de Almacén de Instancias
- Almacenamiento físico conectado al host EC2
- Datos efímeros/temporales
- Se eliminan al detener la instancia
- Útiles para archivos temporales y datos provisionales

#### Amazon EBS (Elastic Block Store)
- Discos duros virtuales persistentes
- Independientes del host EC2
- Datos persisten entre reinicios
- Varios tipos y tamaños disponibles
- Soporta copias de seguridad (snapshots)

#### Características
- Almacena datos como bloques
- Actualiza solo los bloques modificados
- Eficiente para:
  - Bases de datos
  - Software empresarial
  - Sistemas de archivos
