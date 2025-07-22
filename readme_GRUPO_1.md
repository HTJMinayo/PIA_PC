# Repositorio PIA_PC

### Resumen

Este repositorio es una colección de herramientas básicas dentro del area de ciberseguridad, integradas en un unico sistema que se ejecuta mediante una interfaz basada en línea de comandos (CLI). El proyecto dentro de este repositorio permite realizar varias tareas de análisis y defensa informática desde una unica entrada (main.py).
Las funcionalidades incluidas son: 
* WebScraping, permite extraer información pública de sitios web
* Busquedas con shodan, es un motor de busqueda que permite identificar dispositivos conectados a internet y posibles vulnerabilidades.
* Escaneo de puertos con Nmap, es una herramienta para detectar servicios expuestor en un host 
* Extracción de metadata, utilizado en el analisis forense digital
* Cifrado, permite asegurar información sensible.
* Envío de correos, facilit el uso de alertas automatizadas.

Estas herramientas son fundamentales en cualquier proceso de evaluación de seguridad ofensiva (pentesting) o defensiva (blue team).

## JUSTIFICACIÓN 

Decidimos trabajar con este repositorio porque nos parece útil desde el punto de vista educativo. Tiene una estructura modular bastante clara y reúne varias herramientas conocidas en el mundo de la ciberseguridad. 

### Herramientas estandar en el sector

Este proyecto incorpora herramientas consideradas como apoyo en las prácticas profesionales de ciberseguridad. Por ejemplo, Nmap es una de las herramientas más utilizadas en auditorias. Shodan, tambien conocido con el "Google de los dispositivos IoT", permite identificas servicios y dispositivos expuestos en internet, lo cual es util en aplicaciones forenses. Finalmente, la libreria BeautifulSoup agiliza las tareas de web scrapting y es considerada fiable en investigaciones OSINT.

### Uilidad en Ciberseguridad Ofensiva y defensiva

Este repositorio nos permite trabajar con herramientas que llevan a cabo varias etapas del ciclo de seguridad ofensiva: reconocimiento, explotación y generación de reportes, este flijo de alinea con las fases estándar de PTES (Penetration Testing Execution Standard).

Con herramientas como WebScraping con BeautifulSoup y Shodan se obtienen datos públicos o expuesto del objetivo sin interactuar directamente con él permitiendonos ejecutar la etapa de reconocimiento. Además, NMap nos permite identificar puertos abiertos, protocolos y sistemas operativos activos interactuando directamente con el objetivo.

Si bien este repositorio no consta de herramientas de explotación, mediante la etapa de reconocimiento la información recolectada ayuda a preparar la explotación, al identificar servicios vulnerables y configuraciones débiles. Además, las herramientas de extración de metadatos, cifrado y envio de correor permiten obtener información oculta en archivos, simular mecanismos de exfiltración de datos o automatizar la notificación de hallazgos.

Finalmente, al ser un proycto modular y ejecutarse por CLI, los resultados de cada herramienta se pueden redirigir o guardar como archivos de texto, lo cual facilita integrarlos en un informe.

### Descripción de las herramientas dentro del repositorio

#### ¿Cómo funciona el web scraping?

Dentro del scraping hay diferentes modos de funcionamiento, aunque en general se diferencia entre el scraping automático y el manual. El scraping manual define el copiado y pegado manual de información y datos, como quien recorta y guarda artículos de periódico y solo se lleva a cabo si se desea encontrar y almacenar alguna información concreta. Es un proceso muy laborioso que raras veces se aplica a grandes cantidades de datos.

En el caso del scraping automático, se recurre a un software o un algoritmo que analiza diferentes páginas web para extraer información. Se utiliza software especializado según el tipo de página web y el contenido. Dentro del scraping automático, se diferencian varios modos de proceder:

Analizador sintáctico: los analizadores sintácticos (o parsers) se utilizan para convertir un texto en una nueva estructura. Por ejemplo, en los análisis de HTML, el software lee un documento HTML y almacena la información. Un analizador DOM utiliza la representación de contenidos del lado del cliente en el navegador para extraer datos.
Bots: un bot es un software dedicado a realizar determinadas tareas y automatizarlas. En el caso del web harvesting, los bots se utilizan para examinar páginas web automáticamente y recopilar datos.
Texto: aquellos que tienen experiencia con la línea de comandos pueden aprovechar la función grep de Unix para buscar en la web determinados términos en Python o Perl. Este es un método muy sencillo para extraer datos, aunque requiere más trabajo que la utilización de un software.


#### SHODAN ¿Qué es? Para que sirve

Shodan es un motor de búsqueda único que permite explorar dispositivos conectados a internet, desde cámaras de seguridad hasta servidores industriales. A diferencia de los buscadores tradicionales, Shodan revela información técnica sobre equipos expuestos en la red, lo que lo convierte en una herramienta poderosa tanto para profesionales de la ciberseguridad como para investigadores.
Principales usos de Shodan:
Evaluación de seguridad en redes.
Investigación de vulnerabilidades.
Monitoreo de sistemas conectados.
Análisis en ciberinteligencia.
Aunque es una herramienta poderosa, su uso debe ser ético y legal. Expertos en ciberseguridad lo utilizan para mejorar la protección de infraestructuras críticas, pero también puede ser mal usado si cae en manos equivocadas.

#### NMAP

Nmap es una herramienta de escaneo de redes utilizada para descubrir hosts y servicios activos. Permite identificar qué puertos están abiertos en un dispositivo, qué servicios se están ejecutando en ellos y, en algunos casos, incluso el sistema operativo que usa el host.

Funciona enviando paquetes a una dirección IP o a un rango de direcciones, y analizando las respuestas que se reciben. Según el tipo de escaneo (TCP, UDP, SYN, etc.), Nmap puede detectar servicios vulnerables o mal configurados que representan un riesgo para la seguridad

#### Extracción de metadata

La extracción de metadatos consiste en recuperar información oculta que está incrustada dentro de archivos digitales. Esta información puede incluir el autor, la fecha de creación, el software usado, la ubicación GPS (en el caso de imágenes), entre otros datos.

Se utilizan herramientas o librerías que analizan los encabezados de los archivos para leer sus atributos internos. Esta técnica es muy utilizada en el análisis forense digital y la inteligencia de fuentes abiertas (OSINT), ya que puede revelar detalles sensibles sin necesidad de modificar el archivo.

#### Cifrado 

El cifrado es el proceso de transformar datos legibles en un formato codificado que solo puede ser descifrado por alguien que tenga la clave correcta. Es una medida fundamental para proteger la confidencialidad de la información.

Existen varios algoritmos de cifrado, pero el proceso básico implica aplicar una función matemática que mezcla el contenido original con una clave. En el cifrado simétrico (como AES), la misma clave se usa para cifrar y descifrar. En el cifrado asimétrico (como RSA), se utilizan claves públicas y privadas.

#### Envío de correos.

Módulo diseñado para automatizar el envío de correos electrónicos con fines legítimos (notificaciones, alertas de seguridad) o pruebas controladas (simulación de ataques phishing en entornos autorizados).
Protocolos soportados: SMTP, APIs de servicios como Gmail, Outlook o SendGrid.
Funcionalidades avanzadas:
- Cifrado de contenido (PGP, S/MIME).
- Soporte para adjuntos (archivos, imágenes, documentos ofuscados).
- Personalización de cabeceras (spoofing controlado para pruebas de concienciación).
- Envío masivo con gestión de listas de distribución.
Casos de uso:
- Respuesta a incidentes: Notificación inmediata a equipos de seguridad.
- Pentesting: Simulación de campañas de phishing ético para evaluar la resistencia de usuarios.
- Automatización: Envío de reportes periódicos (ej.: logs de intrusiones).

#### Cambio OS

Herramienta para modificar configuraciones dinámicas del sistema operativo, ideal para red teams, pruebas de escalamiento de privilegios o hardening.
Características técnicas:
Operaciones soportadas:
- Modificación de registros (Windows) o archivos de configuración (Linux: /etc/, crontabs).
- Manipulación de variables de entorno.
-Cambio temporal de permisos de archivos o usuarios.
- Interacción con servicios del sistema (inicio/detención de daemons).
- Compatibilidad: Multiplataforma (scripts en Python, Bash o PowerShell).
Casos de uso:
- Escalada de privilegios: Alterar permisos para acceder a recursos restringidos (ej.: modificar /etc/sudoers temporalmente).
- Evasióon de controles: Deshabilitar logs o servicios de monitoreo durante pruebas de penetración.
- Hardening automatizado: Aplicar configuraciones seguras basadas en benchmarks (CIS, NIST).

### Referencias
* Scraping the Web for Public Health Gains: Ethical Considerations from a ‘Big Data’ Research Project on HIV and Incarceration, https://pmc.ncbi.nlm.nih.gov/articles/PMC7392638/?utm_source=chatgpt.com
* Guía de referencia de Nmap, https://nmap.org/man/es/index.html
* What is Shodan, https://help.shodan.io/the-basics/what-is-shodan
* ¿Qué es OSINT?, https://www.ibm.com/mx-es/topics/osint
* Penetration Testing Execution Standard (PTES), https://www.geeksforgeeks.org/software-engineering/penetration-testing-execution-standard-ptes/