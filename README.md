# Laboratorio 3 — Selectores, Box Model y Positioning <img src="https://upload.wikimedia.org/wikipedia/commons/6/61/HTML5_logo_and_wordmark.svg" alt="HTML5" width="50" height="50"><img src="https://upload.wikimedia.org/wikipedia/commons/d/d5/CSS3_logo_and_wordmark.svg" alt="CSS3" width="50" height="50">


💻 **Laboratorio 3**  

**Nombre:** Eyden Su Díaz
**Carné:**  *2023025837*
**Curso:**  IC-8057 – Introducción al Desarrollo de Páginas Web  
**Fecha:**  25/8/2025

---

## 📝 Aplicación de Elementos Solicitados
 

### Selectores

- **Selectores de tipo**:  
  - `header`, `nav`, `section`, `img` (definidos en `base.css` y `layout.css`).

- **Selectores de clase**:  
  - `.btn` aplicado en el botón de envío del formulario.  
  - `.card` en las secciones de expositores.  
  - `.badge` en etiquetas dentro de las tarjetas.  
  - `.input-field` en campos del formulario.

- **Selectores de ID**:  
  - `#agenda`, `#exponentes`, `#temas`, `#testimonios`, `#registro`, `#contacto` (secciones principales).

- **Selectores de atributo**:  
  - `#registro input[type="text"]`, `#registro input[type="email"]` en campos específicos del formulario.  
  - `aside ul li a[aria-label*="X"]`, `...Facebook`, `...Instagram` para personalizar efectos en cada red social.

- **Combinadores**:  
  - `nav a + a` → separador en el menú de navegación.  
  - `.card p` → estilos de párrafos dentro de tarjetas.  
  - `h2 ~ p` → párrafos que siguen a títulos en las secciones.

---

### Pseudo-clases

- **Pseudo-clases de estado**:  
  - `.btn:hover` cambia color de fondo y eleva el botón.  
  - `a:hover` cambia color y subraya.  
  - `.input-field:focus-visible` y `nav a:focus-visible` añaden borde/outlines accesibles.  
  - `nav a:active` aplica un efecto de clic.

- **Pseudo-clases estructurales**:  
  - `#agenda tbody tr:nth-child(even)` alterna colores en filas pares.  
  - `#registro input:not([type="radio"])` aplica estilos a inputs que no son tipo radio.  
  - `footer p:last-child` cambia estilo al último párrafo del pie de página (para el copyright).  

---

### Especificidad

- `!important` aplicado en `.badge` (color y posición).  
- **Inline style**: en el `h1` dentro de `<header>` se aplica `style="color: white"`.

---

### Propiedades y modelos

- **Box model**:  
  - `.card` y secciones como `#registro` usan `margin`, `padding`, `border` y `box-shadow`.  

- **Overflow**:  
  - `.card img` usa `overflow: hidden` al recortar imágenes dentro de las tarjetas.  
  - También aplicable a párrafos extensos dentro de `.card`.

- **Flexbox**:  
  - `nav` usa `display: flexbox` (alineación de enlaces del menú).  
  - También en `figure` para centrar contenido.

- **Grid**:  
  - `body` definido como `display: grid` para el layout principal.  
  - `.cards-container` organiza las tarjetas de exponentes con `grid-template-columns`.

- **Position (relative/absolute)**:  
  - `.card` tiene `position: relative`.  
  - `.badge` dentro de `.card` está en `position: absolute` para colocarse en la esquina.

