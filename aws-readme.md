# AWS Study Guide

Este repositorio contiene un resumen de conceptos clave de AWS basado en varios módulos de estudio.

## Índice
- [Módulo 1: Conceptos Básicos](#módulo-1-conceptos-básicos)
- [Módulo 2: Servicios de AWS](#módulo-2-servicios-de-aws)
- [Módulo 3: Infraestructura Global](#módulo-3-infraestructura-global)
- [Módulo 4: Redes](#módulo-4-redes)
- [Módulo 5: Almacenamiento y Bases de Datos](#módulo-5-almacenamiento-y-bases-de-datos)

## Módulo 1: Conceptos Básicos

### Introducción a AWS
- **Servicios Disponibles:**
  - Amplia gama desde básicos hasta avanzados
  - Soluciones de computación, almacenamiento y seguridad de red
  - Servicios especializados (blockchain, machine learning, IA)
  - Herramientas de administración, producción de vídeo y satélites

### Modelo Cliente-Servidor
- Cliente: Realiza solicitudes (navegador web/aplicación)
- Servidor: Responde a las solicitudes (Amazon EC2)

### Modelo de Precios
- Principio "Pago por uso"
- Sin pago por adelantado
- Escalabilidad flexible según demanda
- Eliminación de costos por capacidad no utilizada

## Módulo 2: Servicios de AWS

### Amazon EC2 (Elastic Compute Cloud)
#### Tipos de Instancias:
1. **Propósito General**
   - Equilibrio entre recursos
   - Ideal para servidores web y bases de datos pequeñas

2. **Computación Optimizada**
   - Alto rendimiento de procesamiento
   - Ideal para servidores de juegos y procesamiento por lotes

3. **Memoria Optimizada**
   - Procesamiento de grandes conjuntos de datos
   - Ideal para bases de datos de alto rendimiento

4. **Computación Acelerada**
   - Uso de coprocesadores
   - Ideal para cálculos complejos y procesamiento gráfico

5. **Almacenamiento Optimizado**
   - Alto rendimiento en I/O
   - Ideal para bases de datos y procesamiento OLTP

#### Opciones de Precios:
- **Bajo Demanda:** Pago por uso sin compromiso
- **Savings Plans:** Ahorro con compromiso de uso
- **Instancias Reservadas:** Descuentos por compromiso temporal
- **Instancias Spot:** Capacidad no utilizada con descuento
- **Hosts Dedicados:** Servidores físicos exclusivos

### Servicios de Mensajería
1. **Amazon SQS (Simple Queue Service)**
   - Sistema de cola de mensajes
   - Buffer entre componentes
   - Alta fiabilidad

2. **Amazon SNS (Simple Notification Service)**
   - Sistema publicación/suscripción
   - Notificaciones múltiples simultáneas
   - Soporta varios tipos de suscriptores

### Computación Sin Servidor
- **AWS Lambda:**
  - Ejecución de código sin gestionar servidores
  - Pago solo por tiempo de ejecución
  - Escalado automático

### Contenedores
- **Amazon ECS:** Sistema de gestión de contenedores
- **Amazon EKS:** Servicio Kubernetes administrado
- **AWS Fargate:** Motor serverless para contenedores

## Módulo 3: Infraestructura Global

### Regiones AWS
#### Factores de Selección:
- Conformidad y regulaciones
- Proximidad a clientes
- Servicios disponibles
- Precios regionales

### Zonas de Disponibilidad (AZ)
- Múltiples centros de datos por región
- Separación física para redundancia
- Alta disponibilidad y resistencia a fallos

### Ubicaciones Periféricas
- **CloudFront (CDN):**
  - Distribución global de contenido
  - Baja latencia
  - Streaming y APIs

### Herramientas de Administración
1. **AWS Management Console:**
   - Interfaz web interactiva
   - Acceso móvil disponible

2. **AWS CLI:**
   - Interfaz de línea de comandos
   - Automatización de tareas

3. **AWS SDK:**
   - APIs para desarrollo
   - Múltiples lenguajes soportados

## Módulo 4: Redes

### Virtual Private Cloud (VPC)
- Red privada virtual en AWS
- Organización en subredes
- Control de acceso granular

### Seguridad
1. **ACL de Red (NACL):**
   - Control a nivel de subred
   - Stateless
   - Verificación bidireccional

2. **Grupos de Seguridad:**
   - Control a nivel de instancia
   - Stateful
   - Gestión de acceso granular

### Conectividad
- **Internet Gateway:** Acceso público
- **Virtual Private Gateway:** Conexiones VPN
- **Direct Connect:** Conexión dedicada

### Route 53 (DNS)
- Gestión de dominios
- Enrutamiento inteligente
- Integración con servicios AWS

## Módulo 5: Almacenamiento y Bases de Datos

### Almacenamiento en Bloques
1. **Volúmenes de Almacén de Instancias:**
   - Almacenamiento temporal
   - Conectado al host EC2
   - Datos efímeros

2. **Amazon EBS (Elastic Block Store):**
   - Almacenamiento persistente
   - Independiente del host
   - Soporta snapshots

---

📝 **Nota:** Este es un resumen en constante evolución. Se irán añadiendo más contenidos conforme se avance en el estudio de AWS.
