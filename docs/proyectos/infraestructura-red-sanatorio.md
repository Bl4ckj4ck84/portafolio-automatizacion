#  Implementación de Infraestructura de Red y Servidor - Sanatorio Colegiales

**Estado:** ✅ Implementado y en mantenimiento  
**Cliente:** Sanatorio Colegiales, Buenos Aires, Argentina  
**Empresa:** Hypertelia SA  
**Rol:** Técnico de Infraestructura y Soporte TI  
**Fecha:** 2015 - 2016  

---

## 📋 Descripción del Proyecto

Diseño, implementación y puesta en marcha de la infraestructura de red local y servidor para un centro médico (Sanatorio Colegiales). El proyecto buscaba garantizar una conectividad estable, segura y segmentada para el personal médico/administrativo y los pacientes/visitantes del sanatorio.

**Nota:** Proyecto ejecutado en colaboración con el Administrador de Sistemas Senior. Mi rol se enfocó en la **implementación técnica de hardware, redes, configuración de servicios y mantenimiento continuo**.

---

##  Objetivos

- Desplegar un servidor local basado en **Ubuntu Server** para la gestión de datos del sanatorio.
- Implementar **servicio DHCP** para asignación automática de IPs a dispositivos conectados.
- Segmentar la red en dos zonas: **WiFi pública** (pacientes/visitantes) y **WiFi privada** (personal médico/administrativo).
- Garantizar la estabilidad y disponibilidad de la red en un entorno crítico (salud).
- Establecer un plan de mantenimiento preventivo y correctivo.
- Facilitar el acceso remoto al servidor mediante **virtualización VMware**.

---

## ⚙️ Especificaciones Técnicas y Rol

### 🛠️ Mi Responsabilidad Técnica (Infraestructura, Redes y Servicios)

#### **Servidor y Sistemas Operativos**
- **Servidor principal:** Ubuntu Server (Linux)
- **Virtualización:** VMware para acceso remoto y local al servidor
- **Servicio DHCP:** Configuración e implementación de servidor DHCP para asignación automática de direcciones IP a todos los dispositivos conectados a la red del sanatorio
- **Mantenimiento del servidor:** Verificación de logs, actualizaciones de seguridad, monitoreo de recursos (CPU, RAM, disco)

#### **Infraestructura de Red**
- **Cableado estructurado:** Instalación y certificación de cableado de red (UTP) para conectar el rack de servidores con los puntos de acceso y estaciones de trabajo
- **Switches:** Configuración de switches para segmentación de tráfico
- **Access Points:** Instalación y configuración de puntos de acceso inalámbricos con cobertura en áreas administrativas, médicas y de atención al público

#### **Segmentación de Redes WiFi**
- **Red WiFi Pública:** 
  - Acceso para pacientes y visitantes del sanatorio
  - Captive portal para autenticación
  - Ancho de banda limitado para garantizar prioridad a la red interna
  - Aislamiento de clientes (client isolation) para seguridad
  
- **Red WiFi Privada (Personal):**
  - Acceso exclusivo para personal médico y administrativo
  - Autenticación WPA2-Enterprise
  - Acceso a recursos internos (servidor, impresoras de red, sistemas médicos)
  - Prioridad de ancho de banda para aplicaciones críticas

#### **Mantenimiento y Monitoreo**
- Verificación diaria del estado del servidor (hardware, temperaturas, discos)
- Revisión de logs de red y access points
- Monitoreo del servicio DHCP (leases, conflictos de IP)
- Soporte técnico de nivel 1 y 2 ante caídas de red o fallas de hardware
- Gestión de backups y recuperación ante desastres

###  Responsabilidad del Administrador de Sistemas (Software/Server)
- Configuración avanzada del Sistema Operativo Ubuntu Server
- Gestión de usuarios y permisos
- Políticas de seguridad y firewall
- Configuración de servicios adicionales (DNS, Samba, etc.)

*(Esta colaboración me permitió aprender la integración completa entre el hardware de red, los servicios de servidor y la virtualización).*

---

## 🔌 Diagrama de la Solución Implementada



---

## 📈 Resultados y Logros

| Métrica | Resultado |
|---------|-----------|
| **Cobertura WiFi** | 100% de las áreas administrativas, médicas y de atención al público |
| **Disponibilidad de Red** | 99.9% (Uptime) durante el período de mantenimiento |
| **Asignación DHCP** | 0 conflictos de IP reportados |
| **Tiempo de Respuesta** | Resolución de incidencias de red en < 30 minutos |
| **Entorno Crítico** | Cero interrupciones en sistemas médicos por fallas de red |
| **Segmentación de Red** | Aislamiento completo entre red pública y privada |

---

## 🔧 Desafíos y Soluciones

1. **Interferencias en el entorno médico**  
   → *Solución:* Estudio de espectro y configuración de canales específicos en los Access Points para evitar interferencias con equipos médicos.

2. **Mantenimiento sin interrumpir la operación del sanatorio**  
   → *Solución:* Programación de tareas de mantenimiento preventivo y reinicios de equipos en horarios de baja afluencia (madrugada).

3. **Seguridad de la red pública**  
   → *Solución:* Implementación de captive portal, aislamiento de clientes y limitación de ancho de banda para la red de pacientes.

4. **Acceso remoto al servidor**  
   → *Solución:* Configuración de VMware para permitir acceso remoto seguro al servidor Ubuntu, facilitando el mantenimiento sin necesidad de estar físicamente en el datacenter.

5. **Gestión automática de IPs**  
   → *Solución:* Implementación de servidor DHCP con rangos de IPs segregados por tipo de dispositivo (público vs privado) y reservas de IP para equipos críticos.

---

##  Competencias Demostradas

✅ **Administración de servidores Linux (Ubuntu Server)**  
✅ **Configuración de servicios de red (DHCP, DNS)**  
✅ **Virtualización con VMware**  
✅ **Segmentación de redes (VLANs, redes públicas/privadas)**  
✅ **Configuración de Access Points con múltiples SSIDs**  
✅ **Seguridad en redes inalámbricas (WPA2-Enterprise, captive portal)**  
✅ **Cableado estructurado y certificación de redes**  
✅ **Mantenimiento preventivo y correctivo de hardware**  
✅ **Monitoreo de servidores y redes**  
✅ **Trabajo en entornos críticos (Salud/Hospitales)**  
✅ **Trabajo en equipo con Administradores de Sistemas**  
✅ **Soporte técnico en sitio (On-site)**

---

## 💡 Aprendizaje para la Automatización Industrial

Este proyecto me enseñó conceptos fundamentales que son **directamente aplicables a las redes industriales (OT)**:

1. **Servicios de red críticos (DHCP)**  
   → En automatización, los PLCs y dispositivos IoT también necesitan asignación automática de IPs para comunicarse eficientemente.

2. **Segmentación de redes**  
   → En la industria, es vital separar la red de control (PLCs, SCADA) de la red corporativa para seguridad y rendimiento.

3. **Virtualización (VMware)**  
   → Los servidores SCADA y HMI modernos corren en entornos virtualizados para facilitar backups y recuperación ante desastres.

4. **Mantenimiento preventivo**  
   → Un PLC no puede comunicarse si el cableado o el switch falla. El mantenimiento preventivo es vital para evitar paradas de planta.

5. **Entornos críticos**  
   → Trabajar en un sanatorio me preparó para trabajar en plantas industriales donde una falla de red puede detener la producción.

---

## 🚀 Tecnologías Utilizadas

| Categoría | Tecnología |
|-----------|------------|
| **Servidor** | Ubuntu Server (Linux) |
| **Virtualización** | VMware |
| **Servicios de Red** | DHCP, DNS |
| **Redes Inalámbricas** | Access Points con múltiples SSIDs |
| **Seguridad** | WPA2-Enterprise, Captive Portal, Firewall |
| **Hardware** | Switches, Cableado UTP, Patch Panels |
| **Sistemas Operativos Cliente** | Windows 10/11, macOS, iOS, Android |
