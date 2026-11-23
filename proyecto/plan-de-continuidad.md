# Plan de continuidad - Etapa 2 de mi sitio

*Emprendimiento:* Lienzo Vivo
*Sitio de la etapa 1:* https://lienzovivo.infinityfree.me
*Fecha:* 23 de noviembre de 2026

## 1. Qué quedó fuera de la etapa 1 y por qué (3 pts)

Lista las funcionalidades que quisiste hacer y no pudiste. Para cada una, la razón.

| Funcionalidad | Por qué quedó fuera (tiempo, recursos, costo, conocimientos) | Qué aporta a mi emprendimiento |
| :--- | :--- | :--- |
| *Carrito de compras y tienda online de obras originales* | *Tiempo y recursos:* Configurar una tienda completa con cálculo de envíos y gestión de inventario único (cada cuadro original es pieza única) requería más semanas de desarrollo y un servidor con mayor capacidad de memoria PHP que el hosting gratuito InfinityFree. | Permite vender directamente en línea los cuadros originales disponibles en stock sin depender exclusivamente de coordinación manual por mensaje. |
| *Pasarela de pagos en línea (Webpay / MercadoPago)* | *Costo y requisitos técnicos:* Habilitar cobros con tarjeta exige contratar un hosting pago con certificado SSL dedicado y gestionar credenciales comerciales/tributarias previas. | Permite cobrar un abono inicial (ej. 50%) para iniciar los cuadros por encargo personalizado, asegurando el compromiso del cliente y cubriendo materiales. |
| *Página Galería / Obras con catálogo visual segmentado y filtros* | *Tiempo:* En la etapa 1 se priorizó la estructura base del sitio (Inicio, Blog, Nosotros, Contactame) y el formulario de cotización antes de armar un catálogo extenso filtrado por técnica y tamaño. | Facilita que los clientes comparen formatos (ej. 50x60 cm, 50x70 cm), precios referenciales y estilos (óleo vs. acrílico) antes de cotizar. |
| *Sección de seguimiento de envíos y políticas de devolución* | *Tiempo y definición operativa:* Requiere estandarizar tarifas de despacho nacional y embalaje protector para cuadros fragiles antes de publicarlo como flujo automatizado. | Brinda mayor confianza y transparencia al comprador sobre los tiempos de pintado, secado del óleo y entrega a domicilio. |

## 2. Recursos que necesito (2 pts)

| Funcionalidad | Plugin o herramienta | Gratis o de pago | Costo aproximado | Qué tendría que aprender |
| :--- | :--- | :--- | :--- | :--- |
| *Carrito de compras y gestión de obras* | WooCommerce | Gratis (plugin base) | $0 USD (solo comisiones por venta en pasarela) | Configuración de productos únicos (stock = 1 para obras originales) y variaciones de tamaño para encargos. |
| *Pasarela de pagos local* | MercadoPago para WooCommerce o Transbank Webpay | Gratis (el plugin) | ~2.9% a 3.5% de comisión por transacción aprobada | Configuración de claves API (Sandbox y Producción) y gestión de abonos para cuadros a pedido. |
| *Galería filtrable por técnica y temática* | Modula o bloques avanzados de Gutenberg | Freemium | $0 USD (versión gratuita) / ~$39 USD al año (Pro) | Organización de portafolio por categorías (Mascotas, Paisajes, Retratos, Obras Originales) y optimización visual. |
| *Correo transaccional confiable para pedidos* | WP Mail SMTP + Brevo | Freemium | $0 USD (plan gratuito hasta 300 correos/día) | Vinculación mediante clave API para asegurar que los comprobantes de pedido y cotización lleguen a la bandeja de entrada. |

*Servidor:* Para la etapa 2 necesitaré migrar desde el hosting gratuito actual (InfinityFree) hacia un *hosting WordPress pago* (como Hosting.cl, EcoHosting o SiteGround) con dominio propio (ej. lienzovivo.cl). Requerirá *mínimo 10 GB de almacenamiento SSD/NVMe* (para alojar fotografías en alta resolución de las pinturas sin saturar el disco), *PHP 8.0 o superior, base de datos **MySQL / MariaDB, **certificado SSL gratuito (HTTPS)* y puertos *SMTP abiertos*.

## 3. Priorización y cronograma (2 pts)

Ordena lo que harías primero y en cuánto tiempo. Puedes usar una tabla o un diagrama Gantt.

| Prioridad | Qué hago | Cuándo (mes o semana) | Resultado esperado |
| :--- | :--- | :--- | :--- |
| *1 (Crítica)* | Migración desde InfinityFree a hosting pago, registro de dominio propio y verificación de certificado SSL (HTTPS). | Semana 1 (Mes 1) | Sitio web estable sin límites de recursos, con mayor velocidad de carga y soporte completo para comercio electrónico. |
| *2 (Alta)* | Creación de la página *Galería / Obras* segmentada por categorías (Mascotas, Paisajes, Obras Originales) y optimización de imágenes a WebP. | Semana 2 (Mes 1) | Catálogo visual ordenado donde los visitantes exploran fácilmente los trabajos terminados y formatos disponibles. |
| *3 (Media)* | Instalación y configuración de *WooCommerce* para venta directa de obras originales + integración de pasarela de pagos (MercadoPago / Webpay). | Semanas 3 y 4 (Mes 1) | Tienda operativa donde los clientes compran cuadros disponibles en stock con pago en línea seguro. |
| *4 (Evolutiva)* | Incorporación de módulo de seguimiento de envíos, políticas de despacho y formulario avanzado con subida de foto de referencia para encargos. | Semanas 1 y 2 (Mes 2) | Flujo completo automatizado tanto para compra directa como para encargos personalizados. |

## 4. Riesgos y mitigación (1 pt)

| Riesgo | Qué haría | Cuándo se activa |
| :--- | :--- | :--- |
| *Fallas o lentitud en el servidor gratuito durante la etapa de transición* | Realizar respaldos completos .wpress semanales con *All-in-One WP Migration* guardados en Google Drive y adelantar la migración a hosting pago. | Si el sitio presenta errores de servidor (500/503) o tiempos de inactividad superiores a 12 horas. |
| *Incompatibilidad visual entre WooCommerce y el tema Twenty Twenty-Five* | Probar la instalación de la tienda primero en un entorno local (*LocalWP) antes de aplicarla en producción, manteniendo un respaldo previo listo para restaurar. | Si al activar WooCommerce se desconfiguran los bloques, encabezados o estilos del tema **Twenty Twenty-Five*. |
| *Pérdida de correos de cotización o confirmación de pedidos* | Configurar *WP Mail SMTP* conectado vía API a *Brevo* (gratuito) en lugar de depender del envío nativo PHP del servidor. | Si los mensajes enviados desde el formulario o los comprobantes de compra no llegan al correo de destino. |
| *Lentitud de carga por subir fotografías muy pesadas de los cuadros* | Redimensionar las imágenes antes de subirlas (máximo 1920px), convertirlas a formato *WebP* y mantener activo *W3 Total Cache*. | Cuando el puntaje de Rendimiento en Lighthouse baje de 75 puntos o la página tarde más de 3 segundos en cargar. |
