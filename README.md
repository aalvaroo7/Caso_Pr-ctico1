# Caso_Práctico1

## Ejercicio 1 

### 1.Capa Física (OSI) / Acceso a la Red (TCP/IP)
🔹 Infraestructura:
Cableado estructurado con Ethernet Gigabit y fibra óptica.
Redes inalámbricas con Wi-Fi 6 para movilidad.
 🔹 Equipos de red:
Switches y routers con soporte para QoS y SD-WAN.
Access Points Wi-Fi para conexión de dispositivos IoT.
 🔹 Dispositivos de videoconferencia:
Cámaras IP, micrófonos y altavoces inteligentes conectados vía PoE o Wi-Fi.

 ### 2.Capa de Enlace de Datos (OSI) / Acceso a la Red (TCP/IP)
🔹 Protocolos de red:
Ethernet (IEEE 802.3) y Wi-Fi 6 (IEEE 802.11ax).
 🔹 Seguridad y segmentación:
VLANs para separar tráfico de videoconferencia, datos y dispositivos IoT.
WPA3 y 802.1X para seguridad en redes inalámbricas.
 🔹 Control de acceso:
Autenticación de dispositivos mediante MAC filtering y RADIUS.

### 3.Capa de Red (OSI) / Internet (TCP/IP)
🔹 Protocolos:
IPv4 e IPv6, enrutamiento dinámico con OSPF/BGP.
MPLS y SD-WAN para optimización del tráfico entre oficinas.
 🔹 Seguridad y túneles seguros:
VPNs con IPSec y SSL/TLS para conexión entre sedes.
Firewalls y listas de control de acceso (ACLs) para proteger la red.

### 4.Capa de Transporte (OSI/TCP/IP)
🔹 Protocolos principales:
UDP para transmisión de video en tiempo real.
TCP para señalización y control.
 🔹 Calidad de Servicio (QoS):
Priorización del tráfico de videoconferencia con DiffServ y DSCP.
SRTP (Secure RTP) para cifrado de medios.

### 5.Capa de Sesión (OSI) / Aplicación (TCP/IP)
🔹 Gestión de sesiones:
SIP, H.323 para señalización y establecimiento de llamadas.
RTP/RTCP para control de sincronización de video y audio.

### 6.Capa de Presentación (OSI) / Aplicación (TCP/IP)
🔹 Codificación y cifrado:
Códecs de video H.264, VP9 para optimización de ancho de banda.
SRTP y TLS para seguridad en transmisión de datos.

### 7.Capa de Aplicación (OSI/TCP/IP)
🔹 Plataformas de videoconferencia:
Zoom, Microsoft Teams, Cisco Webex.
Servidores internos para aplicaciones empresariales y grabaciones.
 🔹 Integración con IoT:
Cámaras inteligentes, sensores de sala, asistentes de voz conectados vía MQTT o WebRTC.
 🔹 Seguridad avanzada:
Autenticación multifactor (MFA) y control de accesos IAM.
