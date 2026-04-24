# assets/color-palette.md — Paleta exacta

> HEX extraídos visualmente de los 8 slides analizados. Úsalos tal cual en Figma, Canva o el diseñador que uses. Son aproximaciones cuidadosas; si tienes acceso al archivo original de diseño, confirma y actualiza.

---

## Paleta primaria (el alma de la marca)

### BG-CREAM `#F2ECD9`
```
██████████████████  #F2ECD9
```
- **Uso:** fondo de TODOS los slides. No hay excepciones.
- **Por qué:** cálido, diferente, reduce fatiga visual, hace brillar los negros.
- **Alternativa si necesitas más claro:** `#F5F0E3` (muy pocas veces).
- **Alternativa si necesitas más oscuro:** `#E8E0C8` (para variación sutil, ej: banners internos).

### BG-TERMINAL `#0F0F10`
```
██████████████████  #0F0F10
```
- **Uso:** fondo de todas las cajas de código, terminales y ventanas negras.
- **Por qué:** no es negro puro, tiene una pizca de azul. Más cálido que `#000000`, más sofisticado.
- **NO uses:** `#000000` puro. Canta "default".

### TEXT-PRIMARY `#0F0F10`
Mismo HEX que el terminal, usado sobre el fondo crema. Esto genera coherencia: tus textos sobre crema usan el mismo negro que los fondos de tus terminales. Sutil pero importante.

### TEXT-MUTED `#8C8A80`
```
██████████████████  #8C8A80
```
- **Uso:** metadata, subtítulos gris, captions.
- **Por qué:** es un gris topo ligeramente verdoso que armoniza con el crema.
- **NO uses:** grises fríos tipo `#666666`. Chocan con el crema.

### TEXT-ON-DARK `#EDEAE0`
- **Uso:** texto sobre las cajas negras de terminal (cuando no es código coloreado).
- **Por qué:** no es blanco puro, tiene la misma calidez del crema. Así nada "desentona".

---

## Paleta de acentos (los 6 colores de folder)

### PURPLE-HERO `#6B4FE3`
```
██████████████████  #6B4FE3
```
- **Uso principal:** color signature, highlights tipográficos (IA, 10 min), número de slide activo en space invaders, número de lista (01-04 en itálica serif).
- **Folder asociado:** Contenido/ (morado).
- **Emoción:** autoridad, tech, premium.

### GREEN-MINT `#4FD696`
```
██████████████████  #4FD696
```
- **Uso principal:** CTAs positivos, estados "Ready", "Success", banners de guía, comandos en terminal.
- **Folder asociado:** Astrya / Workspace (verde del rayo ⚡).
- **Emoción:** acción, crecimiento, todo-bien.

### CORAL-RED `#FF6B5E`
```
██████████████████  #FF6B5E
```
- **Uso principal:** alertas, BREACH, placeholders `[entre corchetes]`, highlights de títulos en `.hackroom`.
- **Folder asociado:** Research/ (rojo).
- **Emoción:** urgencia, atención, peligro controlado.

### YELLOW-MUSTARD `#F4C135`
```
██████████████████  #F4C135
```
- **Uso principal:** folder Clientes/, pill de categoría COMUNICACIÓN, resaltados de comillas en prompts ("pausa").
- **Emoción:** atención, calidez, destacado.

### ORANGE `#F08A3B`
```
██████████████████  #F08A3B
```
- **Uso principal:** folder Diseño/, strings/valores en código.
- **Emoción:** creatividad, energía.

### TEAL `#2DC4B5`
```
██████████████████  #2DC4B5
```
- **Uso principal:** folder Automatiza/, cosas sistémicas.
- **Emoción:** fluidez, sistema, técnica.

---

## Colores secundarios / de soporte

### SYSTEM-RED `#FF5F57`
Color EXACTO del círculo rojo de macOS. No lo modifiques.

### SYSTEM-YELLOW `#FEBC2E`
Círculo amarillo de macOS.

### SYSTEM-GREEN `#28C840`
Círculo verde de macOS.

### LINK-BLUE `#8EA3FF`
- **Uso:** URLs dentro de código (ej: `https://astrya.ai`).
- Una de las pocas veces que usas azul. Solo para links.

### CODE-GRAY `#6B6A64`
- **Uso:** comentarios dentro de terminal (`# pega tu extracto`).
- Siempre en itálica.

---

## Cómo usar los acentos correctamente

### Regla 1 — Un color dominante por carrusel
- Carruseles `.workspace` → verde menta dominante
- Carruseles `.hackroom` → rojo coral dominante
- Carruseles `.promptroom` → morado dominante

### Regla 2 — Máximo 2 acentos en un solo slide
Si ya usas morado para el título, el CTA puede ser verde, pero nunca amarillo + naranja + rojo a la vez.

### Regla 3 — Los highlights en título siempre compiten o complementan
- Coral + morado = tensión (funciona en `.hackroom`: Vercel en coral, 48h en morado).
- Dos tonos verdes = armonía.
- Coral + amarillo = ruido (no usar).

### Regla 4 — Los folders tienen identidad fija
Una vez asocies Clientes/ con amarillo, mantenlo SIEMPRE amarillo. No cambies colores por slide.

---

## Conversión a otros formatos (para tu diseñador)

| Nombre | HEX | RGB | HSL |
|---|---|---|---|
| bg-cream | #F2ECD9 | rgb(242,236,217) | hsl(46,52%,90%) |
| bg-terminal | #0F0F10 | rgb(15,15,16) | hsl(240,3%,6%) |
| text-primary | #0F0F10 | rgb(15,15,16) | hsl(240,3%,6%) |
| text-muted | #8C8A80 | rgb(140,138,128) | hsl(50,5%,53%) |
| text-on-dark | #EDEAE0 | rgb(237,234,224) | hsl(46,24%,90%) |
| purple-hero | #6B4FE3 | rgb(107,79,227) | hsl(251,72%,60%) |
| green-mint | #4FD696 | rgb(79,214,150) | hsl(150,61%,57%) |
| coral-red | #FF6B5E | rgb(255,107,94) | hsl(5,100%,68%) |
| yellow-mustard | #F4C135 | rgb(244,193,53) | hsl(45,89%,58%) |
| orange | #F08A3B | rgb(240,138,59) | hsl(26,86%,59%) |
| teal | #2DC4B5 | rgb(45,196,181) | hsl(174,63%,47%) |

---

## Test de contraste (accesibilidad)

Para que tu marca sea legible y accesible:

| Combinación | Ratio | ¿Pasa WCAG AA? |
|---|---|---|
| text-primary (#0F0F10) sobre bg-cream (#F2ECD9) | 16.1 : 1 | ✅ AAA |
| text-muted (#8C8A80) sobre bg-cream (#F2ECD9) | 3.1 : 1 | ⚠ solo texto grande |
| text-on-dark (#EDEAE0) sobre bg-terminal (#0F0F10) | 15.3 : 1 | ✅ AAA |
| purple-hero (#6B4FE3) sobre bg-cream (#F2ECD9) | 5.2 : 1 | ✅ AA |
| coral-red (#FF6B5E) sobre bg-cream (#F2ECD9) | 3.1 : 1 | ⚠ solo texto grande |

**Nota:** el coral y el gris muted pasan solo para textos grandes. No los uses para body text pequeño sobre crema.
