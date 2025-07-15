## 🧪 Día 6 - Escaneo de Puertos UDP con Nmap

Hoy realizamos un escaneo de los **20 puertos UDP más comunes** utilizando `nmap`, con el objetivo de identificar servicios activos y analizar cómo responde el host frente a peticiones UDP.

---

### 🔧 Comando utilizado:
```bash
sudo nmap -sU --top-ports 20 scanme.nmap.org

🔐 Se usó sudo para permitir escaneo de puertos UDP, que requiere privilegios elevados.

💡 Resultados destacados:
Host: scanme.nmap.org (45.33.32.156)

Tiempo de escaneo: 3.06 segundos

Respuesta: El host está activo (0.022s de latencia)

Puerto	Estado	Servicio
53	open	filtered
67	open	filtered
123	open	NTP
445	open	filtered
9929	open	filtered
31337	open	filtered

⚠️ La mayoría de los puertos aparece como open|filtered, ya que el protocolo UDP no confirma entrega y muchos sistemas aplican firewalls silenciosos.

🎯 Objetivo del ejercicio
Introducir los conceptos de escaneo UDP

Comprender el significado de open|filtered

Identificar servicios que pueden estar corriendo en un host usando UDP

📚 Aprendizaje del día
Cómo lanzar un escaneo UDP básico con nmap

Qué limitaciones tiene el protocolo UDP para reconocimiento

Cómo interpretar correctamente los resultados ambiguos del escaneo
