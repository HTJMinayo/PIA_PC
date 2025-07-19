PIA - Programación para Ciber Seguridad.
Este proyecto es una recopilación de diversas herramientas de ciberseguridad unidas en una sola que se puedem mandar llamar desde un main. Entre esas tareas se encuentra:

WebScraping.
Investigacion con shodan.
Escaneo de puertos con nmap.
Extracción de metadata.
Cifrado.
Envío de correos.
Este script funciona mediante argumentos, solo ciertos script requieren de la interacción del usuario, a continuacion se muestra cómo lo puedes obtener.
Web Scraping: definición
Durante el web scraping (del inglés scraping = arañar/raspar) se extraen y almacenan datos de páginas web para analizarlos o utilizarlos en otra parte. Por medio de este raspado web se almacenan diversos tipos de información: por ejemplo, datos de contacto, tales como direcciones de correo electrónico o números de teléfono, o también términos de búsqueda o URL. Estos se almacenan en bases de datos locales o tablas.
¿Cómo funciona el web scraping?
Dentro del scraping hay diferentes modos de funcionamiento, aunque en general se diferencia entre el scraping automático y el manual. El scraping manual define el copiado y pegado manual de información y datos, como quien recorta y guarda artículos de periódico y solo se lleva a cabo si se desea encontrar y almacenar alguna información concreta. Es un proceso muy laborioso que raras veces se aplica a grandes cantidades de datos.

En el caso del scraping automático, se recurre a un software o un algoritmo que analiza diferentes páginas web para extraer información. Se utiliza software especializado según el tipo de página web y el contenido. Dentro del scraping automático, se diferencian varios modos de proceder:

Analizador sintáctico: los analizadores sintácticos (o parsers) se utilizan para convertir un texto en una nueva estructura. Por ejemplo, en los análisis de HTML, el software lee un documento HTML y almacena la información. Un analizador DOM utiliza la representación de contenidos del lado del cliente en el navegador para extraer datos.
Bots: un bot es un software dedicado a realizar determinadas tareas y automatizarlas. En el caso del web harvesting, los bots se utilizan para examinar páginas web automáticamente y recopilar datos.
Texto: aquellos que tienen experiencia con la línea de comandos pueden aprovechar la función grep de Unix para buscar en la web determinados términos en Python o Perl. Este es un método muy sencillo para extraer datos, aunque requiere más trabajo que la utilización de un software.
Referencia: https://www.ionos.es/digitalguide/paginas-web/desarrollo-web/que-es-el-web-scraping/