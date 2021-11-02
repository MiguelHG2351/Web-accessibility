# Que es accesibilidad?

Es la practica de asegurarnos de que todo lo que creamos para la web se puede usar, interpretay acceder, y que todo lo que se muestra en la web es legible.

a11y neuromino de accesibilidad

# Por que accesibilidad web?

- Para situaciones de usuarios con discapacidades visuales o de usuarios con discapacidades auditivas

- Para que las personas puedan acceder a la información de la web

- Para mejorar la experiencia y usabilidad de la web

- Por que en algunos casos la accesibilidad web es una necesidad por ley, etc

# WCAG  y sus criterios de conformidad

WCAG = Web Content Accessibility Guidelines o Pautas de la Accesibilidad para el contenido de la Web

Creado por la W3C

La que se usara: WAI (Web Accessibility Initiative)
La W3C tiene varias iniciativas para mejorar la accesibilidad como WAI-ARIA, WAI-ARIA-TEC, etc

# Profundizando en los 12 criterios de conformidad

A: Nivel básico

AA: Nivel medio

AAA: Nivel avanzado usado en los gobiernos y universidades

# Los 4 principios de la WCAG

- Perceptible: El contenido debe ser perceptible.

No depende de solo una forma de ver el contenido, sino que debe ser perceptible para todos los usuarios de diferentes recursos no solo una imagen, texto, etc.

- Operable: El contenido debe ser operable

Que no dependan de un mouse o teclado

- Comprensible: El contenido debe ser comprensible

- Robusto: Que sea interpretable de forma fiable por una amplia variedad de aplicaciones de usuarios, incluyendo ayudas tecnicas.

# Tecnologias asistivas

- Visuales:
    - Lectores de pantalla
    - Extensiones que manipulan CSS

- Motoras:
    - Varilla bucal
    - Switch 

# Pruebas manuales (extensiones):

NoCoffe vision simulator

Otra Herramienta

[Otra forma de usarlo](https://static.platzi.com/media/user_upload/Captura%20de%20pantalla%202020-06-19%20a%20las%2018.29.01-24983e60-d28a-4867-9ff4-f6a7f88b357f.jpg)

# Pruebas manuales (teclado):

El tabulador :v

# Lectores de pantalla

- NVDA - Mozilla Firefox

- JAWS - Internet Explorer

- Voice Over - Safari

- ChromeVox - Google Chrome

# HTML semantico


[Otra forma de usarlo](https://www.jungledisk.com/blog/content/images/blog/div-soup-vs-semantic-html.png)

# ARIA

ARIA ( Accessible Rich Internet Applications ): Un conjunto de atributos especiales para accesibilidad que pueden añadirse a cualquier etiqueta, pero especialmente adaptado a HTML.

Fue creado por la W3C, lo crearon para que podamos comunicar cambios especiales en nuestras aplicaciones.

** Atributos de ARIA: **

Roles
Propiedades
Estados

# Estados:

Comunican cambios por ejemplo si un checkbox esta seleccionado, etc.

el aria-hidden evita que lea el contenido de un elemento

**El lector no lee esto, puede ser útil para elementos de un carousel que tiene visible x imagenes**
```html
aria-hidden="true"
```

# Skip Links: 

Son enlaces de página internos que ayudan a la navegación por la página actual, en lugar de a páginas completamente nuevas. Es super util para los usuarios con teclado.

Es obligatorio hace parte de la guide 1 del criterio 2.4.1 Bypass Blocks del Principio Navigable.

(Referencia)[https://www.w3.org/TR/WCAG20-TECHS/G1.html]

```html
<a href="#main" class="skip-link">Skip to main content</a>
```
```css
.skip-link {
  height: 0;
}

.skip-link:focus, .skip-link:active {
  background-color: var(--verde);
  border-radius: 5px;
  color: var(--gris-oscuro);
  font-family: var(--secondary-font);
  height: auto;
  margin: 16px 0 8px;
  text-decoration: none;
}
```
