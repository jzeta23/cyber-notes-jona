# 🛡️ Día 3 – Escaneo de versión con Nmap (`-sV`)

---

## 🎯 Objetivo del día

Practicar el escaneo de versiones de servicios usando Nmap en un entorno controlado, documentar los resultados y manejar interrupciones o fallas comunes de red.

---

## 🔧 Comando ejecutado

```bash
nmap -sV --max-retries 2 --host-timeout 2m scanme.nmap.org -oN nmap_version_scan.txt
-sV: permite detectar la versión de los servicios que corren en los puertos abiertos.

--max-retries 2: limita los reintentos a 2 por puerto.

--host-timeout 2m: cancela el escaneo completo si demora más de 2 minutos.

-oN nmap_version_scan.txt: guarda el resultado en un archivo legible.

🧪 Resultado del escaneo
text
Copiar
Editar
Nmap scan report for scanme.nmap.org (45.33.32.156)
Host is up (0.054s latency).
Other addresses for scanme.nmap.org (not scanned): 2600:3c01::f03c:91ff:fe18:bb2f
Warning: 45.33.32.156 giving up on port because retransmission cap hit (2).
Skipping host scanme.nmap.org (45.33.32.156) due to host timeout
# Nmap done at Thu Jul 10 23:54:08 2025 -- 1 IP address (1 host up) scanned in 121.50 seconds
🧠 Conclusiones
El escaneo comenzó correctamente y detectó que el host está activo.

Sin embargo, se interrumpió automáticamente debido a un host-timeout de 2 minutos.

La configuración aplicada evitó que Nmap quedara colgado como en el intento anterior.

No se logró obtener el listado de servicios por limitaciones del host remoto.

📘 Aprendizajes clave
✅ La opción --host-timeout es fundamental para no colgar escaneos largos.
✅ Saber interpretar un escaneo incompleto también es parte del trabajo real.
✅ Documentar tanto éxitos como fallos es una práctica profesional en ciberseguridad.

📁 Archivo generado
nmap_version_scan.txt: contiene la salida del escaneo.
