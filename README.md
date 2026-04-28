Resumen de la lectura del módulo 7, módulo 8, módulo 9 y módulo 10

MÓDULO 7

1. Contexto general de la computación en la nube

Muchas organizaciones están migrando hacia la nube o usando modelos híbridos para aprovechar beneficios como escalabilidad, acceso remoto y eficiencia operativa. Este cambio también implica retos en seguridad, por lo que existen estándares (como los del NIST) que orientan buenas prácticas. La nube se caracteriza por ofrecer servicios bajo demanda, accesibles desde la red y gestionados de forma automatizada.

2. Tipos de despliegue en la nube

Los modelos de implementación dependen del nivel de acceso y control:

- Nube pública: доступible para cualquier usuario.
- Nube privada: usada por una sola organización.
- Nube comunitaria: compartida por varias organizaciones.
- Nube híbrida: combinación de dos o más modelos anteriores.

3. Modelos de servicio en la nube

Se clasifican según el nivel de control del usuario:

- IaaS (Infraestructura como servicio): el usuario administra sistemas y aplicaciones.
- PaaS (Plataforma como servicio): el proveedor gestiona la infraestructura, el usuario desarrolla aplicaciones.
- SaaS (Software como servicio): aplicaciones listas para usar a través de internet.
  
4. Principales amenazas y ataques en la nube
   
a. Recolección de credenciales
Ataques como phishing y sitios falsos buscan robar datos de acceso. Se apoyan en ingeniería social y malware, aumentando el riesgo a medida que crece el uso de la nube.

b. Escalamiento de privilegios
Un atacante obtiene acceso a niveles superiores dentro del sistema. Puede ser:
- Vertical: obtiene más permisos.
- Horizontal: accede a cuentas con mismos privilegios.
Se previene con auditorías y controles de seguridad.

c. Secuestro de cuentas

Implica el control total de una cuenta mediante robo de credenciales. Afecta la integridad de datos y operaciones. Se detecta monitoreando accesos sospechosos y comportamientos anómalos.

d. Ataques a servicios de metadatos
Explotan vulnerabilidades en servicios internos para robar credenciales (ej. en máquinas virtuales). Se mitigan con controles de acceso y análisis de vulnerabilidades.

5. Ataques por mala configuración

Errores humanos o configuraciones incorrectas generan brechas de seguridad:
- Fallas en autenticación/autorización.
- Problemas en federación de identidades.
- Almacenamiento de datos expuesto.
- Uso de contenedores vulnerables.
- Esto puede permitir acceso no autorizado o pérdida de datos.
  
6. Inyección de malware
Los atacantes insertan código malicioso en aplicaciones o sistemas en la nube, afectando la confidencialidad, integridad y disponibilidad de la información.

7. Ataques de canal lateral
Se basan en analizar información indirecta del sistema (como consumo de energía o tiempo de respuesta) para extraer datos sensibles sin acceso directo.

8. Herramientas de desarrollo en la nube
Los kits de desarrollo facilitan la creación de aplicaciones:

- SDK: herramientas con librerías y compiladores.
- CDK: permiten gestionar infraestructura como código.
Ayudan a desarrollar e implementar soluciones en la nube de forma más eficiente.


MÓDULO 8

Un atacante puede mantener el acceso (persistencia) en un sistema comprometido mediante diferentes técnicas que le permiten seguir controlándolo incluso después del acceso inicial.
Persistencia en sistemas comprometidos

La persistencia se logra mediante acciones como:

- Creación de shells inversos o de enlace
- Manipulación de tareas programadas
- Creación de procesos o daemons personalizados
- Generación de nuevas cuentas o puertas traseras

Estas técnicas permiten al atacante continuar ejecutando acciones como instalar herramientas, hacer análisis del sistema o lanzar nuevos ataques.

Uso de shells

Los shells son interfaces que conectan al atacante con el sistema:

- Shell de enlace: abre un puerto en la víctima esperando conexión
- Shell inverso: el sistema comprometido se conecta al atacante, evitando restricciones como firewalls
- Herramientas como Metasploit (Meterpreter) y Netcat son comúnmente utilizadas.
- Sistemas de comando y control (C2)

Los atacantes utilizan servidores o servicios externos para enviar instrucciones al sistema comprometido. Estos pueden incluir desde servidores propios hasta plataformas en la nube o servicios comunes, lo que facilita el control remoto.

Manipulación de tareas y cuentas

Los atacantes pueden:

- Alterar tareas programadas para ejecutar código automáticamente
- Crear procesos persistentes
- Generar cuentas adicionales (especialmente con privilegios de administrador)
- Esto asegura el acceso continuo al sistema y dificulta su detección.


MÓDULO 9


1. Comparación y estructura de informes escritos
La elaboración de informes en pruebas de penetración requiere una estructura clara y orientada a la audiencia. Es fundamental identificar quién recibirá el informe para adaptar el lenguaje y el nivel técnico, incluyendo siempre un resumen ejecutivo accesible. El contenido debe ser completo, abarcando alcance, metodología, resultados, correcciones y conclusiones, utilizando estándares como CVSS para medir riesgos.
También es clave proteger la información, controlando estrictamente su almacenamiento y distribución. Durante la prueba, la toma constante de evidencias (capturas, notas, videos) garantiza claridad en los hallazgos. El uso de herramientas especializadas facilita la organización del informe. Además, identificar causas raíz permite entender mejor las vulnerabilidades. Finalmente, la calidad del informe impacta directamente la reputación profesional y la toma de decisiones del cliente.

2. Análisis de hallazgos y recomendaciones
En las pruebas de penetración, los hallazgos deben ir acompañados de recomendaciones claras, clasificadas en distintos tipos de controles:

- Técnicos: soluciones tecnológicas como parches, cifrado, autenticación multifactor o segmentación de red.
- Administrativos: políticas, procedimientos y marcos como RBAC o SSDLC que regulan la seguridad.
- Operativos: prácticas del día a día, como capacitación, rotación de funciones o concientización.
- Físicos: medidas de protección en instalaciones, como controles de acceso o videovigilancia.

Esta clasificación permite abordar los riesgos de forma integral, no solo desde lo tecnológico, sino también desde la gestión y operación.

3. Importancia de la comunicación
La comunicación durante una prueba de penetración es tan importante como el informe final. No todo debe esperar al cierre: los hallazgos críticos deben reportarse de inmediato. Una mala comunicación puede generar malentendidos o ampliar innecesariamente el alcance del proyecto.
Es importante mantener informados a todos los actores (contactos técnicos, principales y de emergencia), y emitir reportes de estado cuando sea necesario. Además, la comunicación ayuda a prevenir falsos positivos, gestionar incidentes detectados y ajustar prioridades según los riesgos encontrados.
El informe debe ser claro, detallado y adaptado a la audiencia técnica, incluyendo evidencias suficientes para reproducir los problemas, cuidando siempre la confidencialidad de la información.

4. Actividades posteriores a la entrega del informe

Después de entregar el informe, hay una fase crítica de cierre. Se debe realizar una limpieza completa de los sistemas intervenidos, eliminando datos residuales, herramientas utilizadas, accesos creados y cualquier rastro de la prueba.
También es importante documentar la aceptación del informe por parte del cliente y analizar las lecciones aprendidas para mejorar futuros procesos. El cliente puede solicitar nuevas pruebas o seguimientos, que deben gestionarse dentro de plazos acordados.
Finalmente, toda la información confidencial obtenida durante la prueba debe ser destruida conforme a los acuerdos establecidos, garantizando la seguridad y privacidad del cliente.


MÓDULO 10


1. Análisis de vulnerabilidades

Estas herramientas sirven para detectar fallos de seguridad en sistemas, redes y aplicaciones.
- OpenVAS, Nessus, Nexpose, Qualys: escáneres que identifican vulnerabilidades y ayudan a gestionarlas.
- SQLmap: especializado en detectar y explotar vulnerabilidades de inyección SQL.
- Nikto: analiza servidores web en busca de fallos comunes.
- OWASP ZAP y W3af: prueban la seguridad de aplicaciones web mediante escaneo automatizado.
- DirBuster: descubre directorios ocultos en servidores.

2. Ataques de credenciales

Se enfocan en descifrar contraseñas o acceder a cuentas mediante fuerza bruta o diccionarios.
- John the Ripper, Hashcat, Hydra: herramientas populares para romper contraseñas.
- Cain & Abel: recuperación de contraseñas en sistemas Windows.
- Aircrack-ng: enfocado en redes WiFi.
- Medusa, Ncrack, THC Hydra: automatizan ataques de login en red.
- CeWL: genera listas de palabras desde sitios web.
- Mimikatz: extrae credenciales almacenadas en memoria.
- Patator: herramienta modular para ataques de fuerza bruta.

3. Persistencia

Permiten mantener acceso a un sistema después de comprometerlo.
- PowerSploit: módulos de PowerShell para post-explotación.
- Empire: framework que facilita control remoto y persistencia en sistemas.

4. Evasión

Se utilizan para evadir antivirus, firewalls y otros mecanismos de defensa.
- Veil: genera malware difícil de detectar.
- Tor: anonimiza la conexión en internet.
- Proxychains: enruta tráfico a través de proxies.
- Cifrado: protege la información transmitida.
- Túneles DNS: ocultan tráfico dentro de consultas DNS.


5. Marcos de explotación

Son plataformas para ejecutar ataques y explotar vulnerabilidades.
- Metasploit: el framework más popular para pruebas de penetración.
- BeEF: enfocado en explotar navegadores web.

6. Depuración, desensamblado y análisis

Se enfocan en analizar software, encontrar errores y hacer ingeniería inversa.
- GDB, WinDbg, OllyDbg: depuración de código.
- IDA Pro, Ghidra: desensamblado y análisis avanzado de binarios.
- objdump: inspección de archivos compilados.


7. Análisis forense

Ayudan a investigar incidentes de seguridad y recuperar evidencia digital.
- Autopsy, Sleuth Kit: análisis de discos y archivos.
- Volatility: análisis de memoria.
- EnCase, FTK: herramientas comerciales avanzadas.
- Wireshark: análisis de tráfico de red.
- Cellebrite UFED, X-Ways: análisis de dispositivos móviles y sistemas.


8. Aseguramiento del software

Buscan mejorar la calidad y seguridad del código.
- SpotBugs, FindSecBugs: análisis estático en Java.
- SonarQube: evaluación continua del código.
- Fuzzers (Peach, AFL, etc.): detectan errores enviando datos inesperados.


9. Herramientas inalámbricas

Se usan para evaluar la seguridad de redes WiFi.
- WiFi Pineapple, Aircrack-ng: auditoría de redes.
- Kismet, Reaver: detección y explotación de fallos en WiFi.
- Wifite: automatiza ataques inalámbricos.

10. Esteganografía

Permiten ocultar información dentro de archivos aparentemente normales.
- OpenStego, Steghide: esconden datos en imágenes o audio.
- ExifTool: analiza metadatos.
- Stegosuite: combina varias funciones de ocultación.

11. Herramientas en la nube

Enfocadas en evaluar la seguridad de servicios cloud.
- ScoutSuite: auditoría multi-nube.
- CloudBrute: descubrimiento de recursos expuestos.
- Pacu: explotación en AWS.
- Cloud Custodian: gestión y cumplimiento de políticas.
