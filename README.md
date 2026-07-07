# Viva Viviendas · Propiedades

Portal de propiedades en venta y renta para Puerto Vallarta, con panel de administración, generador de tarjeta de presentación y publicación sobre hosting estático.

## Estructura

```
index.html          Aplicación completa (público + panel admin)
properties.json     Catálogo publicado que ven todos los visitantes
```

## Cómo administrar y publicar propiedades

El sitio es estático, así que las propiedades que ven todos viven en `properties.json`. El panel es tu herramienta para editarlas y generar ese archivo.

1. Entra al panel con el botón **Administrar** (clave por defecto `viva2026`, cámbiala en **Ajustes**).
2. Agrega o edita propiedades. En **Nueva propiedad** puedes **subir fotos** (se optimizan solas) o pegar URLs. La primera foto es la portada.
3. Tus cambios quedan como **borrador** en tu navegador y aparece la barra “cambios sin publicar”.
4. Pulsa **Exportar properties.json** y reemplaza el archivo del repo con el descargado (commit).
5. Al terminar el deploy, todos los visitantes ven las propiedades actualizadas.

**Descartar** en la barra de borrador regresa a la versión publicada.

## Tarjeta de presentación del asesor

En **Panel → Mi tarjeta** capturas los datos del asesor. El WhatsApp alimenta los botones de contacto del sitio. Desde ahí generas:

- **vCard (.vcf)** — se guarda directo en los contactos del cliente.
- **Tarjeta HTML** — archivo independiente para enviar por WhatsApp o publicar como tarjeta digital.
- **Imprimir / PDF** — versión imprimible.
