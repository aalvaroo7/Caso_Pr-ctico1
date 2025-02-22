# Caso_Práctico1

 
## Ejercicio 1 

Esquematizar la arquitectura lógica de la red utilizando los modelos OSI y TCP/IP.
Incluir dispositivos de videoconferencia, servidores de aplicaciones y equipos de red.

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


## Ejercicio 2

# Capa Física: Cálculo de Tasa de Transmisión y Selección de Modulación

Para diseñar correctamente la **capa física** en la red de videoconferencia, es necesario calcular la **tasa de transmisión máxima** usando la **fórmula de Shannon**, y seleccionar una modulación adecuada para enlaces **cableados e inalámbricos**.

---

## 1)Cálculo de la Tasa de Transmisión Máxima (Shannon)

La **capacidad máxima del canal** según Shannon se calcula con la ecuación:

 C = B * log_2(1 + SNR) 

Donde:
- **C** = Capacidad del canal en **bps** (bits por segundo).
- **B** = Ancho de banda del canal en **Hz**.
- **SNR** = Relación señal-ruido en **escala lineal** (no en dB).

###  Cálculo

Supongamos que tenemos:
- **Ancho de banda (B):** 20 MHz (Wi-Fi)
- **SNR en dB:** 30 dB (relación señal-ruido común en redes Wi-Fi)

### 🔹 Conversión de SNR a escala lineal

Para convertir SNR de dB a escala lineal:

SNR_{lineal} = 10^{(SNR_{dB} / 10)} 

 SNR_{lineal} = 10^{(30 / 10)} = 10^3 = 1000

### 🔹 Aplicando la ecuación de Shannon

 C = 20 \times 10^6 \times \log_2(1 + 1000) 

 C \approx 20 \times 10^6 \times \log_2(1001)

 C \approx 20 \times 10^6 \times 9.97 

 C \approx 199.4 \text{ Mbps}

###  Conclusión

En un canal **Wi-Fi de 20 MHz** con **SNR = 30 dB**, la **tasa máxima teórica de transmisión** es aproximadamente **199.4 Mbps**. 
