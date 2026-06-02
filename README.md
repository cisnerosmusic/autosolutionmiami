# AutoSolution Miami

Landing page de conversión para Eduardo Alvarez — financiamiento de autos en Miami (crédito malo, sin crédito, ITIN, bancarrota).

## Objetivo

Conseguir leads. El visitante hace una breve entrevista en la web (formulario) y al enviarla se arma un mensaje de WhatsApp con sus datos, listo para contactar a Eduardo. También hay CTAs directos para llamar.

## Flujo de conversión

1. **Hero** — gancho "¿Te rechazaron el crédito?" + botón a la entrevista.
2. **Entrevista (formulario)** — nombre, teléfono, ciudad, tipo de auto, situación de crédito, presupuesto y notas.
3. **CTA** — al enviar abre WhatsApp con todos los datos. CTA final con teléfono + WhatsApp y botón flotante.

## Estructura

- `index.html` — página completa (HTML + CSS + JS en un solo archivo, sin dependencias salvo Google Fonts).

## Datos del negocio (configurables)

- **Marca:** AutoSolution Miami
- **Especialista:** Eduardo Alvarez · Doral Lincoln, Miami FL
- **Teléfono:** (305) 218-3558
- **WhatsApp:** en `index.html`, variable `WA_NUMBER = '13052183558'` (formato internacional, sin signos).

Para cambiar el número de WhatsApp, edita `WA_NUMBER` en el `<script>` y los enlaces `wa.me` del HTML. El teléfono de llamada está en los `href="tel:..."`.

## Publicar (GitHub Pages)

1. Sube `index.html` a la raíz del repositorio.
2. Settings → Pages → Source: rama `main`, carpeta `/root`.
3. Apunta el dominio `autosolutionmiami` al sitio (Settings → Pages → Custom domain).

## Pendiente / próximos pasos

- Captura de leads: hoy el formulario solo abre WhatsApp (no guarda nada en servidor). Para no perder leads se puede conectar a email, Google Sheet o Formspree.
- Reemplazar testimonios de ejemplo por reseñas reales (idealmente con enlace a Google Reviews).

## Idiomas (bilingüe ES/EN)

La página está en español por defecto. Si el navegador del visitante está en inglés, se muestra automáticamente en inglés. Hay un botón ES/EN en el menú para cambiar manualmente y la preferencia se recuerda (localStorage).

Los textos se traducen vía atributos `data-i18n` y el diccionario `I18N` dentro del `<script>` de `index.html`. Para editar o añadir textos, modifica las entradas en los bloques `es` y `en` (deben tener las mismas claves).
