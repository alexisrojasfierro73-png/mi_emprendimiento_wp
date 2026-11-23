# Lienzo Vivo · Sitio WordPress

* *Sitio en producción:* https://lienzovivo.infinityfree.me
* *Autora: Johana Rojas Sección 01-D

## Contexto de la web

*Lienzo Vivo* es un emprendimiento familiar dedicado a la pintura artística hecha a mano en óleo y acrílico, especializado en cuadros por encargo personalizado (mascotas, paisajes y retratos) y venta de obras originales. El sitio está dirigido a personas que buscan regalos únicos y recuerdos duraderos pintados sobre tela, permitiéndoles explorar el estilo de la artista, conocer la historia del taller y solicitar cotizaciones a medida.

## Mi tema

* *Tema instalado desde WordPress:* Twenty Twenty-Five - https://es.wordpress.org/themes/twentytwentyfive/

## Instrucciones si uso un tema descargado

### Requisitos del tema

| Dato | Mi tema |
| :--- | :--- |
| Nombre y enlace a la ficha | [Twenty Twenty-Five](https://es.wordpress.org/themes/twentytwentyfive/) |
| Gratis o de pago | Gratis (tema oficial de WordPress) |
| Tipo (clásico o de bloques) | De bloques (Full Site Editing / Edición completa del sitio) |
| Versión de WordPress que requiere | 6.4 o superior |
| Versión de PHP que requiere | 7.2.24 o superior (recomendado PHP 8.0+) |
| Plugins que necesita (si alguno) | Ninguno obligatorio |
| Licencia | GPLv2 o posterior |

### Cómo llevar mi sitio de Local a producción

Para migrar el sitio desde el entorno local hacia el alojamiento en producción (InfinityFree) se utilizó un plugin de migración todo en uno:

* *Plugin de migración que uso:* [All-in-One WP Migration and Backup](https://es.wordpress.org/plugins/all-in-one-wp-migration/). Es gratis en su versión base. Su límite principal es el tamaño máximo de subida en el servidor de destino.
* *Qué se exporta:* Base de datos completa (entradas, páginas, configuraciones, menús), archivos multimedia (fotografías de las pinturas), temas y plugins instalados.

*Pasos:*
1. *En Local:* Se instaló y activó All-in-One WP Migration, luego se fue a Exportar > Exportar a > Archivo para generar el paquete .wpress.
2. *En producción:* Se realizó una instalación limpia de WordPress en InfinityFree, se instaló y activó el plugin All-in-One WP Migration y el tema oficial Twenty Twenty-Five.
3. *Importa:* Desde el panel de producción se entró a All-in-One WP Migration > Importar y se subió el archivo .wpress generado.
4. *Revisa:* Se guardaron nuevamente los enlaces permanentes (Ajustes > Enlaces permanentes), se verificó que el menú de navegación y la página de inicio cargaran bien, y se revisaron las imágenes y el formulario de contacto.
5. *Problemas que tuve y cómo los resolví:* Para evitar caídas o demoras por límite de carga en el servidor gratuito, se simplificó el tamaño de las imágenes y se activó W3 Total Cache para optimizar el rendimiento.

## Respaldo y reinstalación en otro servidor

El objetivo de este proyecto es que puedas respaldar tu sitio y reinstalarlo en cualquier servidor. Aquí están los pasos para replicarlo:

*Qué respaldar:*
* Los archivos de WordPress (tema Twenty Twenty-Five, plugins instalados y carpeta uploads con las imágenes de las obras).
* La base de datos (páginas, entradas del blog, menús y configuración general).

*Cómo respaldo mi sitio:* Se utiliza el plugin *All-in-One WP Migration and Backup. Al ir a *All-in-One WP Migration > Exportar > Archivo, el plugin genera un único archivo empaquetado con extensión .wpress que se descarga directamente en la computadora.

*Cómo lo reinstalo en un servidor nuevo:*
1. *Requisitos del servidor:* Hosting o servidor local con PHP 7.4 o superior, base de datos MySQL/MariaDB y al menos 500 MB de espacio libre en disco.
2. *Instalar WordPress limpio:* Descargar e instalar WordPress desde cero en el nuevo dominio o servidor local y crear su base de datos vacía.
3. *Restaurar el respaldo:* Entrar al panel /wp-admin, instalar y activar All-in-One WP Migration, ir a Importar y cargar el archivo .wpress respaldado.
4. *Ajustar:* Ir a Ajustes > Enlaces permanentes y hacer clic en Guardar cambios dos veces para regenerar las rutas. Verificar en Ajustes > Generales que la URL del sitio coincida con el nuevo dominio.
5. *Probar:* Navegar por todas las páginas del sitio verificando que carguen las fotografías de los cuadros, el menú, las entradas del blog y probar el envío del formulario de contacto.

*Problemas que tuve y cómo los resolví:* Al restaurar en un servidor distinto, a veces las rutas internas o los enlaces permanentes arrojan error 404; se soluciona entrando a Ajustes > Enlaces permanentes y guardando los cambios nuevamente.

## Plugins instalados

| Plugin | Para qué lo uso | Gratis o de pago | Versión |
| :--- | :--- | :--- | :--- |
| Yoast SEO | Optimización de títulos, meta descripciones y SEO básico | Gratis | 23.x |
| Forminator | Creación e inserción del formulario de contacto y cotizaciones | Gratis | 1.48.6 |
| All-in-One WP Migration and Backup | Exportación, respaldo y migración completa del sitio | Gratis | 7.101 |
| Loginizer | Seguridad y bloqueo de intentos fallidos de inicio de sesión | Gratis | 2.0.3 |
| W3 Total Cache | Optimización de rendimiento y almacenamiento en caché | Gratis | 2.8.13 |

## Páginas y entradas

* *Páginas:* Inicio, Blog, Nosotros, Contactame
* *Entradas del blog:* Lienzo vivo, La pintora, Las dudas y la creación

## Cómo me organicé

Mi plan y mi plan B están en [decisiones.md](proyecto/decisiones.md).

## Plan de continuidad y rendimiento

* Plan de continuidad (etapa 2 de mi web): [plan-de-continuidad.md](proyecto/plan-de-continuidad.md)
* Análisis de rendimiento con Lighthouse: [lighthouse.md](proyecto/lighthouse.md)

## Uso de IA

* *Gemini:* Lo utilicé como apoyo para estructurar la documentación técnica en Markdown, redactar los textos del proyecto y guiar la resolución de problemas de configuración en WordPress, ajustando manualmente los datos específicos de mis plugins, rutas y enlaces del proyecto.
*
