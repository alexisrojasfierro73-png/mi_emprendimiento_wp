# Decisiones - Lienzo Vivo

## 1. Plugins (10 pts)

| Plugin | Funcionalidad que resuelve | Tipo (Gratis / De pago) y qué incluye la versión gratis | Versión de WordPress compatible ("Probado hasta") | ¿Funciona con tema propio (custom)? | Enlace a la ficha en WordPress.org |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Yoast SEO** *(Obligatorio)* | Optimización para motores de búsqueda (SEO), análisis de contenido y mapas de sitio XML. | **Gratis:** Análisis básico de SEO, optimización de palabras clave y metadatos sociales. | 6.4 o superior | Sí | [Yoast SEO en WordPress.org](https://wordpress.org/plugins/wordpress-seo/) |
| **Forminator** *(Obligatorio)* | Creación de formularios avanzados, encuestas y formularios de contacto para cotizaciones de cuadros. | **Gratis:** Formularios de contacto ilimitados con campos de arrastrar y soltar, subida de archivos e integraciones básicas con pagos. | 6.4 o superior | Sí | [Forminator en WordPress.org](https://wordpress.org/plugins/forminator/) |
| **All-in-One WP Migration and Backup** | Exportación e importación de la base de datos, archivos multimedia y temas completos para copias de seguridad. | **Gratis:** Respaldo y exportación completa del sitio de cualquier tamaño con un solo clic. | 6.4 o superior | Sí | [All-in-One WP Migration en WordPress.org](https://wordpress.org/plugins/all-in-one-wp-migration/) |
| **Loginizer** | Protección contra ataques de fuerza bruta limitando los intentos fallidos de inicio de sesión por IP. | **Gratis:** Bloqueo automático de IP tras rebasar los intentos permitidos y gestión de listas blancas/negras. | 6.4 o superior | Sí | [Loginizer en WordPress.org](https://wordpress.org/plugins/loginizer/) |
| **W3 Total Cache** | Optimización del rendimiento web, almacenamiento en caché de páginas y reducción de tiempos de carga. | **Gratis:** Caché de página, de objetos, de navegador y optimización básica de rendimiento web. | 6.4 o superior | Sí | [W3 Total Cache en WordPress.org](https://wordpress.org/plugins/w3-total-cache/) |

---

## 2. Páginas de la Fase 1 (5 pts)

1. **Inicio** *(Obligatoria)*: Presenta la propuesta de valor principal de "Lienzo Vivo" ("Arte hecho a mano que da vida a tus recuerdos"), muestra destacados de cuadros y un llamado a la acción directo para cotizar.
2. **Contacto** *(Obligatoria)*: Permite a los clientes enviar solicitudes de encargos personalizados, medidas y consultas de forma directa mediante un formulario.
3. **Nosotros / La Artista**: Cuenta la historia familiar del emprendimiento, la pasión por la pintura al óleo y la conexión emocional detrás de cada obra creada.
4. **Galería / Obras**: Muestra un catálogo visual organizado de las obras originales, paisajes y ejemplos de cuadros anteriores realizados por encargo.
5. **Blog**: Espacio para compartir el proceso creativo, reflexiones sobre el arte y el trasfondo de las pinturas de la artista.

* **Páginas que quedan para una fase posterior:** Carrito de compras, pasarela de pagos en línea, sección de seguimiento de envíos y políticas de devolución (la tienda de comercio electrónico completa se implementará en una fase posterior).

---

## 3. Plan del Tema 

### A. Carta Gantt 

| Etapa | Fechas (Noviembre 2026) | Tareas principales |
| :--- | :--- | :--- |
| **Identidad Visual** | 05 Nov - 08 Nov | Definición de tipografías elegantes, paleta de colores neutros y logotipo. |
| **Home (Inicio)** | 09 Nov - 12 Nov | Maquetación de la página de inicio, secciones de presentación y llamadas a la acción. |
| **Páginas y Contenidos** | 13 Nov - 17 Nov | Creación y carga de contenidos para Contacto, Nosotros, Galería y Blog. |
| **Checkpoint** | **18 Noviembre** | **Revisión general del estado del sitio, corrección de errores y validación con docente.** |
| **Plugins y Ajustes** | 19 Nov - 22 Nov | Instalación de Yoast SEO, Forminator, respaldos y pruebas de rendimiento. |
| **Entrega Final** | **25 Noviembre** | **Pulido final, pruebas en producción y entrega del proyecto en GitHub.** |

```mermaid
gantt
    title Plan de Desarrollo - Lienzo Vivo
    dateFormat  YYYY-MM-DD
    section Etapas
    Identidad Visual       :active, 2026-11-05, 2026-11-08
    Home y Estructura      :2026-11-09, 2026-11-12
    Páginas y Contenidos   :2026-11-13, 2026-11-17
    Checkpoint             :milestone, 2026-11-18, 2026-11-18
    Plugins y Ajustes      :2026-11-19, 2026-11-22
    Entrega Final          :milestone, 2026-11-25, 2026-11-25
