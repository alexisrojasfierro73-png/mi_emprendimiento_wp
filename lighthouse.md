# Análisis de rendimiento con Lighthouse - Lienzo Vivo

*URL analizada:* https://lienzovivo.infinityfree.me  
*Herramienta:* Google PageSpeed Insights (Lighthouse)  
*Enlace al informe:* (https://pagespeed.web.dev/analysis/https-lienzovivo-infinityfree-me/nqxe3nxs24?form_factor=desktop)

## 1. Puntajes obtenidos

### Resultados en Móvil (Celulares)
* *Rendimiento (Performance):* *97* / 100
* *Accesibilidad (Accessibility):* *100* / 100
* *Prácticas recomendadas (Best Practices):* *100* / 100
* *SEO:* *92* / 100

### Resultados en Escritorio
* *Rendimiento (Performance):* *99* / 100
* *Accesibilidad (Accessibility):* *100* / 100
* *Prácticas recomendadas (Best Practices):* *100* / 100
* *SEO:* *92* / 100

## 2. Análisis de los resultados

* *Rendimiento (97 móvil / 99 escritorio):* El sitio obtuvo una calificación sobresaliente gracias a una estructura liviana y al uso activo del plugin *W3 Total Cache. Las métricas principales muestran tiempos muy rápidos (*First Contentful Paint de 1.3 s en móvil y 0.5 s en escritorio; Largest Contentful Paint de 2.5 s en móvil y 0.8 s en escritorio), sin desplazamientos inesperados de diseño (Cumulative Layout Shift = 0). Los únicos avisos menores detectados en móvil corresponden a la visualización de fuentes (ahorro estimado de 40 ms) y la entrega de imágenes (ahorro estimado de 33 KiB).
* *Accesibilidad (100 / 100):* Se alcanzó el puntaje máximo tanto en móvil como en escritorio. El tema oficial *Twenty Twenty-Five* asegura una estructura semántica adecuada, contraste de colores legibles y correcta navegación.
* *Prácticas recomendadas (100 / 100):* El sitio cumple al 100% con los estándares web modernos, incluyendo conexión segura mediante certificado SSL activo (https://), ausencia de errores en consola y correcta configuración de seguridad.
* *SEO (92 / 100):* Aunque el sitio es rastreable e indexable correctamente, PageSpeed Insights detectó una advertencia específica: "El documento no tiene una meta descripción", lo que impide llegar a los 100 puntos en esta categoría.

## 3. Mejoras propuestas o aplicadas (mínimo 2)

1. *Activación de caché estática y optimización de carga (Aplicada):* Se instaló y configuró el plugin *W3 Total Cache* en WordPress, logrando reducir los tiempos de respuesta del servidor gratuito InfinityFree y alcanzando puntajes de 97 en móvil y 99 en escritorio.
2. *Incorporación de Meta Descripciones con Yoast SEO (Propuesta):* Utilizar el bloque de *Yoast SEO* en el editor de cada página (Inicio, Blog, Nosotros, Contactame) para redactar meta descripciones personalizadas y atractivas, resolviendo la única observación detectada en la auditoría SEO para alcanzar el 100 / 100.
3. *Optimización de formato de imágenes a WebP (Propuesta):* Convertir las fotografías de las pinturas a formato moderno *WebP* antes de subirlas a la biblioteca de medios para aprovechar el ahorro de peso sugerido por Lighthouse (33 KiB en móvil) y mantener tiempos de carga bajos a medida que crezca el catálogo de cuadros.
