# IDENTITY.md — Sistema visual de @juanaia_

> Documento vivo. Si algún día contratas a un diseñador o le pides ayuda a alguien para producir contenido, este archivo basta para que lo haga on-brand sin preguntarte nada.

---

## 1. Paleta de colores (extraída con lupa)

### Fondo base
El color más importante de tu marca. Presente en TODOS los slides. No es blanco puro, es crema/beige:

```
--bg-cream:       #F2ECD9   (aprox. — crema cálido, casi sepia)
```

Esto es una **decisión de diseño muy fuerte**. El blanco puro habría sido la opción cobarde. El crema:
- Reduce fatiga visual (importante porque tus slides tienen mucho código oscuro).
- Comunica "esto no es un post corporativo más".
- Combina con los colores saturados sin competir.

### Color de contraste principal
```
--bg-terminal:    #0F0F10   (negro profundo con pizca azul)
```
Usado para cajas de código, terminales, timelines. Es tu "pantalla dentro del slide".

### Acentos — los 6 colores de folder

Son los mismos 6 colores pixel-art que aparecen en los folders de la portada del workspace. **Te recomiendo usarlos como sistema**:

| Color | HEX aprox | Uso detectado | Emoción |
|---|---|---|---|
| 🟣 Morado vibrante | `#6B4FE3` | IA, destacados, acento principal, highlights tipográficos | Tech, autoridad |
| 🟢 Verde menta | `#4FD696` | Workspace, Astrya, CTAs positivos, "Success" | Crecimiento, ok |
| 🔴 Rojo coral | `#FF6B5E` | Hackroom, BREACH, alertas, errores | Urgencia |
| 🟡 Amarillo mostaza | `#F4C135` | Folder Clientes, categoría Comunicación | Atención |
| 🟠 Naranja | `#F08A3B` | Folder Diseño | Creativo |
| 🔷 Turquesa | `#2DC4B5` | Folder Automatiza | Sistémico |

**Regla maestra:** cada serie tiene un color dominante. No mezcles más de 2 colores de acento por carrusel, o el estilo empieza a parecer desordenado.

### Color de texto
```
--text-primary:   #0F0F10   (casi negro sobre crema — el mismo negro de las terminales)
--text-muted:     #8C8A80   (gris topo sobre crema, para metadata tipo "prompt log · 2026")
--text-on-dark:   #EDEAE0   (crema suave para texto dentro de terminales)
```

### Código dentro de terminales
Dentro de las cajas oscuras, tu syntax highlighting sigue estas convenciones (muy estable):

```
Comando/prompt     →  Verde menta    (#4FD696)
String/valor       →  Naranja        (#F08A3B)
Keyword/label      →  Rojo coral     (#FF6B5E)
Placeholder [X]    →  Rojo coral     (#FF6B5E)
Comentario (#...)  →  Gris itálica   (#6B6A64)
URL/link           →  Azul lavanda   (#8EA3FF)
Éxito/check ✓      →  Verde menta    (#4FD696)
```

---

## 2. Tipografía

Detecté **tres familias** funcionando en armonía:

### Sans-serif bold — el grito
- **Uso:** títulos grandes de portada y de slide ("Mi setup de IA reemplazó a un equipo de 5 personas", "Asegura tu proyecto en 10 min").
- **Aspecto:** sans bold, muy pesada, inter-letter spacing apretado.
- **Equivalente probable:** familia tipo *Inter Display Bold*, *Söhne Breit*, *PP Neue Montreal Bold*, o *Söhne Kräftig*. También podría ser *Basteleur* o *Geist*. La forma de la `a` es humanista, no geométrica.

### Serif itálica — el susurro
- **Uso:** palabras clave en los títulos (*IA*, *roleplay*, *brutal*, *10 min*, *48h*).
- **Aspecto:** serif clásica en itálica, con contraste alto.
- **Equivalente probable:** *GT Sectra*, *Source Serif*, *PP Editorial New*, o *Reckless*. Tiene el aire "New York Times meets tech bloggy".

### Monospace — el código
- **Uso:** metadata superior (`juana_ia.workspace`, `juana.ia 2026`), cajas de terminal, nombres de archivo, prompts.
- **Aspecto:** mono bold para títulos de ventana, mono regular para contenido.
- **Equivalente probable:** *JetBrains Mono*, *Geist Mono*, *IBM Plex Mono*, *Berkeley Mono*. Claramente una mono de programador, no una genérica tipo Courier.

**Regla maestra de tipografía:**
- Nunca mezcles las 3 en un mismo elemento.
- Sans + itálica serif → solo en títulos grandes, para highlights.
- Mono → solo dentro de "ventanas" (con las 3 bolitas de macOS) o como metadata.

---

## 3. Elementos de interfaz (el "sistema operativo")

Tu gran hallazgo visual: cada slide simula ser una ventana del sistema. Esto es lo que compone esa ventana:

### 3.1 — La cabecera de macOS
```
🔴 🟡 🟢   nombre_ventana.tipo
           subtítulo o tag          [página X/Y]
```

- 3 círculos a la izquierda: **rojo (#FF5F57), amarillo (#FEBC2E), verde (#28C840)** — colores EXACTOS de macOS, no inventes.
- Nombre de ventana en mono bold: `juana_ia.workspace`, `juaniaia_.hackroom`, `juanaia_.promptroom`.
- Subtítulo en mono más pequeño y gris: `juana.ia 2026`, `incident log · 2026`, `prompt log · 2026`.
- Indicador de página **a la derecha, en píldora negra**: `1/8`, `4/9`, etc.

### 3.2 — La barra de búsqueda
Aparece en casi todas las slides. Imita una search bar (Spotlight de macOS o barra de navegador):

```
┌──────────────────────────────────────────────┐
│ 🔍  Enséñame cualquier cosa en 20 minutos  🔍 │
└──────────────────────────────────────────────┘
```

- Fondo blanco, pill redondeada, sombra muy sutil.
- Icono de lupa a la izquierda (en cajas de prompt) o a la derecha (en cajas de workspace).
- El contenido de la búsqueda ES el hook del carrusel o el query a resolver.

### 3.3 — Los folders pixel-art
Solo en la serie `.workspace`, pero son tu firma más reconocible:

- Pixel-art perfecto, cuadrado, con sombra muy sutil.
- 6 colores (los mismos de la paleta).
- Cada folder tiene un icono pixel dentro (documento, carta, lupa, rejilla, diana, rayo).
- Nombre del folder justo debajo en mono: `Contenido/`, `Clientes/`, `Research/`, `Diseño/`, `Automatiza/`.
- El `/` final es clave — comunica "es una ruta de sistema, no una etiqueta".

### 3.4 — Las cajas de terminal / ventana
```
┌─ ● ● ●   Terminal — zsh ─────────────────┐
│                                          │
│  juana@mac ~/astrya                      │
│  $ npx vercel deploy --prod              │
│  ...                                     │
└──────────────────────────────────────────┘
```

- Fondo negro (`#0F0F10`).
- Bordes redondeados (radius ~12-16px).
- Barra superior con las 3 bolitas + nombre del proceso.
- Sombra muy sutil hacia abajo.
- Padding interior generoso (~24-32px).

### 3.5 — Los badges / pills
Usas píldoras para categorizar. Patrón detectado:

```
/ 02    APRENDER       →  numeración + categoría (Promptroom)
♡ GUÍA  si tienes...   →  CTA / aviso (Hackroom)
● Ready                →  estado (dentro de cajas)
⚠ BREACH               →  alerta roja (Hackroom)
```

### 3.6 — El paginador space invaders
**Es tu firma más distintiva.** Al final de cada slide, en lugar de los típicos puntos de paginación:
- Una fila de aliens de Space Invaders en pixel-art.
- Todos en gris/lavanda excepto **uno en morado (#6B4FE3)** que marca la slide actual.
- Comunica: "esto es una serie, y estás en el slide N".

Nunca cambies esto. Es lo que hace que aunque cambies de tema, la gente sepa "es un carrusel de Juana".

---

## 4. Layout y composición

### Grid general
Las slides son **1080 × 1350** (formato 4:5, vertical Instagram/TikTok).
Zona segura: 80px de margen en todos los bordes aproximadamente.

### Estructura vertical típica (de arriba a abajo)
```
┌──────────────────────────────────────┐
│  [cabecera macOS + nombre ventana]   │  ← ~80px altura
├──────────────────────────────────────┤
│                                      │
│  [search bar o tag/badge]            │  ← opcional, 60-80px
│                                      │
│  [TÍTULO GRANDE                      │
│   con highlight en itálica]          │  ← 180-280px, el protagonista
│                                      │
│  [CONTENIDO PRINCIPAL:               │
│   - caja de terminal, O              │
│   - grid 2x2 de cards, O             │
│   - folders pixel-art]               │  ← el cuerpo del slide
│                                      │
├──────────────────────────────────────┤
│  @juanaia_  ·  log 2026     invaders │  ← ~60px footer
└──────────────────────────────────────┘
```

### Ritmo visual dentro del carrusel
Analizando el orden de tus 8 slides del carrusel de Vercel:
1. Slide 1: PORTADA (imagen pixel grande + título a gritos)
2. Slide 2: TIMELINE (la historia cronológica)
3-6: DESARROLLO (cada ángulo/lección)
7: SLIDE DE VALOR PRÁCTICO (los "4 pasos")
8: CIERRE

→ Fórmula: **Gancho visual → Timeline → 4-5 slides de desarrollo → Slide útil → Cierre/CTA**.

---

## 5. Tokens de diseño (resumen técnico)

```css
/* Colores */
--bg-cream: #F2ECD9;
--bg-terminal: #0F0F10;
--text-primary: #0F0F10;
--text-muted: #8C8A80;
--text-on-dark: #EDEAE0;

--accent-purple: #6B4FE3;
--accent-green: #4FD696;
--accent-coral: #FF6B5E;
--accent-yellow: #F4C135;
--accent-orange: #F08A3B;
--accent-teal: #2DC4B5;

/* Radii */
--radius-card: 16px;       /* cajas grandes */
--radius-pill: 999px;      /* badges, search bar */
--radius-small: 8px;       /* elementos pequeños */

/* Spacing */
--space-slide-padding: 80px;
--space-element-gap: 32px;
--space-tight: 16px;

/* Typography sizes */
--text-title-xl: 72px;     /* portadas tipo "Mi setup..." */
--text-title-lg: 56px;     /* títulos de slide secundario */
--text-body: 22px;
--text-mono-title: 28px;
--text-mono-body: 20px;
--text-meta: 16px;
```

---

## 6. Lo que NO hacer (anti-patterns de tu marca)

- ❌ **Emojis decorativos** (🚀✨💡). Destrozan el estilo de código. Los únicos "emojis" que encajan son los círculos de macOS 🔴🟡🟢 y los iconos pixel.
- ❌ **Fondos con gradiente**. Tu marca es plana y crema. Los gradientes son de 2021.
- ❌ **Iconos de Font Awesome o Heroicons**. Solo pixel-art, o emojis-círculo de estado.
- ❌ **Más de 2 colores de acento en un solo slide**. Rompe la paleta.
- ❌ **Hashtags en el propio slide** (en el caption sí). Dentro del slide se ven amateur.
- ❌ **Firmas/watermarks gigantes**. El paginador space invaders + el footer `@juanaia_` basta.
- ❌ **Frases motivacionales de LinkedIn**. Tu voz es irónica, técnica, cercana. Nunca "el éxito está en intentarlo".
- ❌ **Slide final de "gracias" o "sígueme"** sin utilidad. Si haces CTA, que vaya envuelta en el lenguaje de la marca (`$ sígueme`, `→ DM abierto`).
