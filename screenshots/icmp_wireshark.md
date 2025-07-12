# Análisis de paquetes ICMP con Wireshark (Día 4)

## 🎯 Objetivo del ejercicio
Capturar y analizar paquetes ICMP generados al hacer `ping` desde Kali Linux utilizando Wireshark.

## ⚙️ Herramientas utilizadas
- Kali Linux
- Terminal (`ping`)
- Wireshark

## 🛠️ Pasos realizados

1. Abrí Wireshark y seleccioné la interfaz `eth0` (interfaz activa de red).
2. Inicié captura de tráfico.
3. Ejecuté el comando: `ping google.com`
4. Apliqué el filtro `icmp` en Wireshark para visualizar únicamente los paquetes ICMP.
5. Analicé los paquetes tipo *Echo Request* y *Echo Reply*.

## 🔍 Observaciones

- Se observaron múltiples paquetes con:
  - **Tipo 8**: Echo Request (petición)
  - **Tipo 0**: Echo Reply (respuesta)
- Los paquetes mostraban correctamente el **IP origen** y **destino**, además del **identificador** y el **TTL** (Time To Live).

## 🖼️ Evidencias

Se tomaron capturas de pantalla donde se muestra:
- El filtro aplicado (`icmp`)
- Los paquetes ICMP enviados y recibidos
- Detalles del contenido de un paquete específico

📂 Ver archivos:  
- `icmp_ping_capture_01.png`  
- `icmp_ping_capture_02.png`

## 🧠 Reflexión final

Este ejercicio fue clave para:
- Entender cómo funciona la comunicación entre equipos en la red.
- Usar Wireshark para analizar tráfico en tiempo real.
- Reconocer estructuras básicas de los paquetes ICMP.

---

✅ **Día 4 completado.**
