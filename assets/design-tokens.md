# assets/design-tokens.md — Tokens de diseño

> Valores exactos para que cualquier herramienta (Figma, Canva, Framer, código) pueda reproducir tu estilo. Copia-pega directo.

---

## Dimensiones base

```
slide-width:      1080px
slide-height:     1350px     (formato 4:5 Instagram/TikTok)
safe-margin:      80px (todos los bordes)
max-content:      920px (ancho útil dentro del margen)
```

## Spacing scale

```
space-xs:         4px
space-s:          8px
space-m:          16px
space-l:          24px
space-xl:         32px
space-2xl:        48px
space-3xl:        64px
space-4xl:        96px
```

**Uso:**
- Entre párrafos dentro de caja: `space-l` (24px)
- Entre elementos principales del slide: `space-2xl` (48px)
- Margen del slide: `space-4xl` (96px) o `safe-margin` (80px)

## Border radius

```
radius-s:         8px       (badges pequeños, botones)
radius-m:         12px      (cards secundarias)
radius-l:         16px      (cajas principales de terminal y cards)
radius-xl:        20px      (cajas grandes)
radius-pill:      999px     (search bar, pills de categoría)
```

## Sombras

Muy sutiles — tu marca casi no usa sombra. Las que detecté:

```
shadow-soft:      0 1px 3px rgba(0,0,0,0.08)   → folders pixel-art
shadow-card:      0 2px 8px rgba(0,0,0,0.06)   → cajas negras
shadow-none:      none                          → default para casi todo
```

**Regla:** si dudas si añadir sombra, no la añadas. Tu estilo es plano.

---

## Tipografía — escalas exactas

### Títulos (sans-serif bold)

```
title-xl:         84px / lh 0.95 / weight 800   → portadas gigantes
title-l:          64px / lh 1.0 / weight 800    → títulos de slide secundario
title-m:          44px / lh 1.1 / weight 700    → subtítulos grandes
title-s:          28px / lh 1.3 / weight 700    → títulos de card
```

### Itálicas serif (highlights)

Heredan el tamaño del título al que acompañan, pero:
```
font-style: italic
font-family: serif (ver IDENTITY.md)
color: depende del contexto (purple-hero o coral-red)
```

### Body text

```
body-l:           22px / lh 1.4 / weight 400    → subtítulos, bajadas
body-m:           18px / lh 1.5 / weight 400    → texto corriente
body-s:           14px / lh 1.4 / weight 400    → leyendas
```

### Monospace

```
mono-title:       22px / lh 1.3 / weight 700    → nombre de ventana ("juana_ia.workspace")
mono-body:        18px / lh 1.6 / weight 400    → contenido de terminal
mono-meta:        14px / lh 1.4 / weight 400    → metadata gris (prompt log · 2026)
mono-small:       12px / lh 1.3 / weight 400    → etiquetas tipo "anon@0xff"
```

---

## Componentes reutilizables

### macOS Window Header
```
Altura: 48px
Padding: 16px horizontal, 12px vertical
Elementos:
  - 3 círculos (12px cada uno, 8px gap entre ellos)
  - nombre ventana (mono-title, text-primary)
  - subtítulo (mono-meta, text-muted) debajo del nombre o a la derecha
  - indicador página (pill negra redonda, 24px alto, texto blanco 14px)
```

### Search Bar
```
Alto: 64px
Padding horizontal: 24px
Background: #FFFFFF (blanco puro, única excepción)
Border-radius: pill (999px)
Border: 1px solid #E8E2D0 (crema oscuro)
Sombra: shadow-soft
Contenido: lupa (20px) + texto body-l + (opcional) folder colored a la derecha
```

### Pill de Categoría
```
Alto: 36px
Padding: 8px horizontal 16px
Border-radius: pill
Background: color de categoría (amarillo, verde, morado, etc.)
Text: 16px bold, text-primary o text-on-dark según contraste
Ejemplos: "APRENDER", "COMUNICACIÓN", "FINANZAS"
```

### Caja de Terminal
```
Background: bg-terminal (#0F0F10)
Border-radius: radius-l (16px)
Padding: 32px
Sombra: shadow-card
Header interno:
  - 3 bolitas macOS (10px cada una, 6px gap)
  - nombre archivo/proceso (mono-meta 14px, text-muted)
  - 16px margen inferior antes del contenido
```

### Tarjeta Grid 2x2
```
Background: bg-terminal (#0F0F10)
Border-radius: radius-l (16px)
Padding: 32px
Height: 420px aprox (que quepa el grid 2x2 en la slide)
Número (01, 02...): 
  - font: serif italic
  - size: 56px
  - weight: 400
  - color: purple-hero
  - margin-bottom: 24px
Título de card:
  - font: sans bold
  - size: 22px
  - color: text-on-dark
Descripción:
  - font: mono o sans regular
  - size: 16px
  - color: text-muted
Pill de comando (bottom):
  - background: transparent con border subtle
  - O background: rgba(79,214,150,0.15)
  - color: green-mint
  - position: absolute bottom 32px left 32px
```

### Folder Pixel-Art
```
Size: 160x140px aprox (proporción tipo folder)
Style: pixel-art con 2-3 tonos del color base
Icono interior: pixel negro sobre el fondo del folder
Nombre debajo:
  - font: mono
  - size: 20px
  - color: text-primary
  - margin-top: 12px
Sombra: shadow-soft
```

### Paginador Space Invaders
```
Position: bottom, centrado
Gap entre invaders: 16px
Size de cada invader: 28-32px
Color default: #D6CDB5 (crema oscuro, muy tenue)
Color activo: purple-hero (#6B4FE3)
Asset: sprite pixel-art 11x8px aprox, escalado a tamaño visible
```

---

## Iconografía

### Estilo único: pixel-art
Todos tus iconos son pixel-art. No mezcles estilos.

**Iconos detectados en tus slides:**
- 📁 Folder (6 variantes de color)
- ⚡ Rayo (workspace/astrya)
- 🔍 Lupa (research / search bar)
- ✉ Sobre (clientes)
- ⚙ Engranaje / diana (automatiza)
- ▦ Rejilla (diseño)
- 📄 Documento (contenido)
- 🎭 Hacker encapuchado (hackroom portada)
- 🐙 Pulpo morado (workspace mascot)
- 👾 Space invaders (paginador)

**Si necesitas más iconos:** mantén la estética 8-bit/16-bit, resolución baja (16x16 o 24x24 escalado), colores planos, sin gradientes.

---

## Export / producción

### Formato final
```
File type:    PNG (no JPG — te comes el detalle del pixel-art)
Dimensions:   1080 x 1350
DPI:          72
Color space:  sRGB
Compression:  lossless para el PNG
```

### Si exportas para TikTok carrusel
```
Dimensions:   1080 x 1920 (9:16 vertical)
Safe zone:    dejar 250px top y 300px bottom libres
              (la interfaz de TikTok come los bordes)
```

---

## Checklist de QA antes de publicar

- [ ] Todos los slides usan bg-cream (#F2ECD9), no blanco.
- [ ] El negro de terminales es #0F0F10, no #000000.
- [ ] Las 3 tipografías están presentes (sans bold, serif italic, mono).
- [ ] El paginador space invaders está en TODAS las slides, con el correcto en morado.
- [ ] La cabecera macOS está en TODAS las slides, con el nombre de la serie correcto.
- [ ] Máximo 2 acentos de color por slide.
- [ ] Los placeholders en corchetes `[algo]` están en coral-red dentro de código.
- [ ] No hay sombras agresivas, no hay gradientes.
- [ ] La numeración de slide está en el formato X/Y en píldora negra top-right.
