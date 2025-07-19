PIA - Programación para Ciber Seguridad.
Este proyecto es una recopilación de diversas herramientas de ciberseguridad unidas en una sola que se puedem mandar llamar desde un main. Entre esas tareas se encuentra:

WebScraping.
Investigacion con shodan.
Escaneo de puertos con nmap.
Extracción de metadata.
Cifrado.
Envío de correos.
Cambio OS


¿Cómo funciona el web scraping?
Dentro del scraping hay diferentes modos de funcionamiento, aunque en general se diferencia entre el scraping automático y el manual. El scraping manual define el copiado y pegado manual de información y datos, como quien recorta y guarda artículos de periódico y solo se lleva a cabo si se desea encontrar y almacenar alguna información concreta. Es un proceso muy laborioso que raras veces se aplica a grandes cantidades de datos.

En el caso del scraping automático, se recurre a un software o un algoritmo que analiza diferentes páginas web para extraer información. Se utiliza software especializado según el tipo de página web y el contenido. Dentro del scraping automático, se diferencian varios modos de proceder:

Analizador sintáctico: los analizadores sintácticos (o parsers) se utilizan para convertir un texto en una nueva estructura. Por ejemplo, en los análisis de HTML, el software lee un documento HTML y almacena la información. Un analizador DOM utiliza la representación de contenidos del lado del cliente en el navegador para extraer datos.
Bots: un bot es un software dedicado a realizar determinadas tareas y automatizarlas. En el caso del web harvesting, los bots se utilizan para examinar páginas web automáticamente y recopilar datos.
Texto: aquellos que tienen experiencia con la línea de comandos pueden aprovechar la función grep de Unix para buscar en la web determinados términos en Python o Perl. Este es un método muy sencillo para extraer datos, aunque requiere más trabajo que la utilización de un software.
Investigacion con shodan.
Shodan: ¿Qué es? Para que sirve
Shodan es un motor de búsqueda único que permite explorar dispositivos conectados a internet, desde cámaras de seguridad hasta servidores industriales. A diferencia de los buscadores tradicionales, Shodan revela información técnica sobre equipos expuestos en la red, lo que lo convierte en una herramienta poderosa tanto para profesionales de la ciberseguridad como para investigadores.
Principales usos de Shodan:
Evaluación de seguridad en redes.
Investigación de vulnerabilidades.
Monitoreo de sistemas conectados.
Análisis en ciberinteligencia.
Aunque es una herramienta poderosa, su uso debe ser ético y legal. Expertos en ciberseguridad lo utilizan para mejorar la protección de infraestructuras críticas, pero también puede ser mal usado si cae en manos equivocadas.



Envío de correos.

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

Cambio OS

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