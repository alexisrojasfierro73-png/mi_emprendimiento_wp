# Decisiones - Lienzo Vivo

## 1. Plugins 

| Plugin | Funcionalidad que resuelve | Tipo (Gratis / De pago) y qué incluye la versión gratis | Versión de WordPress compatible ("Probado hasta") | ¿Funciona con tema propio (custom)? | Enlace a la ficha en WordPress.org |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Yoast SEO** *(Obligatorio)* | Optimización para motores de búsqueda (SEO), análisis de contenido y mapas de sitio XML. | **Gratis:** Análisis básico de SEO, optimización de palabras clave y metadatos sociales. | 6.4 o superior | Sí | [Yoast SEO en WordPress.org](https://wordpress.org/plugins/wordpress-seo/) |
| **Forminator** *(Obligatorio)* | Creación de formularios avanzados, encuestas y formularios de contacto para cotizaciones de cuadros. | **Gratis:** Formularios de contacto ilimitados con campos de arrastrar y soltar, subida de archivos e integraciones básicas con pagos. | 6.4 o superior | Sí | [Forminator en WordPress.org](https://wordpress.org/plugins/forminator/) |
| **All-in-One WP Migration and Backup** | Exportación e importación de la base de datos, archivos multimedia y temas completos para copias de seguridad. | **Gratis:** Respaldo y exportación completa del sitio de cualquier tamaño con un solo clic. | 6.4 o superior | Sí | [All-in-One WP Migration en WordPress.org](https://wordpress.org/plugins/all-in-one-wp-migration/) |
| **Loginizer** | Protección contra ataques de fuerza bruta limitando los intentos fallidos de inicio de sesión por IP. | **Gratis:** Bloqueo automático de IP tras rebasar los intentos permitidos y gestión de listas blancas/negras. | 6.4 o superior | Sí | [Loginizer en WordPress.org](https://wordpress.org/plugins/loginizer/) |
| **W3 Total Cache** | Optimización del rendimiento web, almacenamiento en caché de páginas y reducción de tiempos de carga. | **Gratis:** Caché de página, de objetos, de navegador y optimización básica de rendimiento web. | 6.4 o superior | Sí | [W3 Total Cache en WordPress.org](https://wordpress.org/plugins/w3-total-cache/) |

---

## 2. Páginas de la Fase 1 

1. **Inicio** *(Obligatoria)*: Presenta la propuesta de valor principal de "Lienzo Vivo" ("Arte hecho a mano que da vida a tus recuerdos"), muestra destacados de cuadros y un llamado a la acción directo para cotizar.
2. **Contacto** *(Obligatoria)*: Permite a los clientes enviar solicitudes de encargos personalizados, medidas y consultas de forma directa mediante un formulario.
3. **Nosotros / La Artista**: Cuenta la historia familiar del emprendimiento, la pasión por la pintura al óleo y la conexión emocional detrás de cada obra creada.
4. **Galería / Obras**: Muestra un catálogo visual organizado de las obras originales, paisajes y ejemplos de cuadros anteriores realizados por encargo.
5. **Blog**: Espacio para compartir el proceso creativo, reflexiones sobre el arte y el trasfondo de las pinturas de la artista.

* **Páginas que quedan para una fase posterior:** Carrito de compras, pasarela de pagos en línea, sección de seguimiento de envíos y políticas de devolución (la tienda de comercio electrónico completa se implementará en una fase posterior).

---

### A. Carta Gantt

| Etapa | Fechas (Noviembre 2026) | Tareas principales |
| :--- | :--- | :--- |
| *Identidad Visual* | 05 Nov - 08 Nov | Definición de tipografías elegantes, paleta de colores neutros y logotipo. |
| *Home (Inicio)* | 09 Nov - 12 Nov | Maquetación de la página de inicio, secciones de presentación y llamadas a la acción. |
| *Páginas y Contenidos* | 13 Nov - 17 Nov | Creación y carga de contenidos para Contacto, Nosotros, Galería y Blog. |
| *Checkpoint* | *18 Noviembre* | *Revisión general del estado del sitio, corrección de errores y validación con docente.* |
| *Plugins y Ajustes* | 19 Nov - 22 Nov | Instalación de Yoast SEO, Forminator, respaldos y pruebas de rendimiento. |
| *Entrega Final* | *25 Noviembre* | *Pulido final, pruebas en producción y entrega del proyecto en GitHub.* |

mermaid
gantt
    title Plan de Desarrollo - Lienzo Vivo
    dateFormat YYYY-MM-DD
    section Etapas
    Identidad Visual     :active, 2026-11-05, 2026-11-08
    Home y Estructura    :2026-11-09, 2026-11-12
    Páginas y Contenidos :2026-11-13, 2026-11-17
    Checkpoint           :milestone, 2026-11-18, 2026-11-18
    Plugins y Ajustes    :2026-11-19, 2026-11-22
    Entrega Final        :milestone, 2026-11-25, 2026-11-25


### B. Elección del Tema

* *Tema elegido:* Twenty Twenty-Five (tema oficial de WordPress).
* *Tipo de tema:* Descargado / oficial (no desarrollado desde cero).
* *Razón de elección:* Se eligió *Twenty Twenty-Five* porque utiliza edición completa del sitio por bloques, es ligero, estable en hosting gratuito (InfinityFree) y permite adaptar la paleta de colores neutros, tipografías elegantes y galerías visuales para resaltar las obras de Lienzo Vivo sin errores de código.

---

## 4. Plan B (Gestión de Riesgos)

| Riesgo identificado | Qué haremos en cada caso (Acción) | Cuándo se activa |
| :--- | :--- | :--- |
| *1. Fallo o lentitud en el hosting gratuito (InfinityFree)* | Realizar respaldos completos periódicos con el plugin All-in-One WP Migration and Backup y, en caso de caída prolongada, restaurar el paquete .wpress en un hosting alternativo o entorno local. | Si el sitio presenta errores de servidor (500/503) o tiempo de inactividad superior a 12 horas antes de la entrega. |
| *2. Conflicto o error de compatibilidad entre plugins* | Desactivar el plugin conflictivo desde el panel de WordPress (o renombrar su carpeta por FTP) y mantener activos únicamente los plugins esenciales (SEO, formularios y respaldo). | Si al instalar o actualizar un plugin la página queda en blanco o se pierden los estilos visuales. |
| *3. Fallo en el envío de correos del formulario de contacto* | Configurar autenticación SMTP o mostrar de forma destacada el correo electrónico directo y redes sociales de Lienzo Vivo en la página Contacto. | Si los mensajes enviados desde Forminator no llegan a la bandeja de entrada durante las pruebas. |

---

## 5. Estado en Producción (Formativa 08: Checkpoint)

* *URL en producción:* https://lienzovivo.infinityfree.me
* *Tema activo:* Twenty Twenty-Five
* *Páginas publicadas en el menú:* Inicio, Blog, Nosotros y Contacto (todas con texto propio).
* *Entradas de blog publicadas:* 3 entradas con texto propio («Lienzo vivo», «La pintura» y «Las dudas y la creación»).
* *Plugins activos y verificados en WordPress:*
  * All-in-One WP Migration and Backup (v7.113) — Respaldo y migración.
  * Forminator (v1.58.4) — Formularios de contacto y cotización.
  * Loginizer (v2.1.2) y Loginizer Pro (v2.1.3) — Seguridad contra ataques de fuerza bruta.
  * Speed Optimizer (v7.8.6) y W3 Total Cache (v2.11.0) — Optimización de rendimiento y caché.
  * Yoast SEO (v28.8) — Optimización para buscadores.

---

## 6. Cambios respecto de la Sumativa 2

### Qué se mantuvo
* *Identidad y propuesta visual:* Se mantuvo el concepto artístico de Lienzo Vivo, la paleta de colores neutros, las tipografías elegantes y las páginas base planificadas en la Fase 1 (incluyendo Inicio, Nosotros, Blog y Contacto).
* *Contenido propio:* Se conservaron las 3 entradas del blog con reflexiones originales sobre la pintura y el proceso creativo.

### Qué se cambió y por qué
* *Explicitación del tema y versión de plugins:* Siguiendo la retroalimentación de la evaluación anterior, se formalizó el uso del tema oficial *Twenty Twenty-Five* y se verificaron las versiones instaladas de los plugins activos dentro del entorno de WordPress en producción.
* *Simplificación del contacto en fase de checkpoint:* Para asegurar estabilidad y evitar fallos de envío de correo en el servidor gratuito, la página Contacto se publicó con información directa (correo, redes y horarios) respaldada por Forminator.

---

## 7. Decisión: Continuar con Twenty Twenty-Five

* *Decisión tomada:* *Continuar* con el tema *Twenty Twenty-Five* y la arquitectura actual hacia la entrega final.
* *Justificación y evidencia:* El sitio carga correctamente en producción (https://lienzovivo.infinityfree.me), mantiene la identidad visual de Lienzo Vivo, cuenta con todas las páginas (incluyendo Inicio y Contacto en el menú) y las 3 entradas de blog exigidas para el checkpoint. Evidencia verificable mediante el historial de commits de este repositorio y el sitio activo en producción.
