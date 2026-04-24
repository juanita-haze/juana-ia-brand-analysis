# PLAYBOOK.md — Cómo producir un carrusel nuevo

> Esta es la checklist que sigues cada vez que vas a publicar. Si la sigues entera, el carrusel sale on-brand sin tener que pensar. Tiempo estimado por carrusel: 90-120 minutos de ideación + escritura. El diseño debería ser ejecución mecánica si usas las plantillas.

---

## Fase 1 — Decisión (5 min)

Antes de tocar nada, responde estas 3 preguntas:

### 1. ¿Qué serie es este carrusel?
- `.workspace` → sobre tu setup, tu forma de trabajar, tus rutinas con IA
- `.hackroom` → sobre un incidente, una vulnerabilidad, un fallo técnico real
- `.promptroom` → sobre UN prompt concreto que regalas a tu audiencia

→ Si no encaja en ninguna, pregúntate si merece una serie nueva, o si es un post de feed y no un carrusel.

### 2. ¿Qué acción quieres que haga el que lo ve?
Elige UNA:
- Guardarlo (prompts, guías paso a paso)
- Compartirlo (análisis que hace que parezcan inteligentes quien lo comparte)
- Contactarte (casos prácticos que llevan a "yo necesito esto")
- Descargar Astrya (demos de features, comparativas)

→ Todo el carrusel se diseña hacia esa acción. No mezcles objetivos.

### 3. ¿Cuál es tu "frase dolor" o "frase trofeo"?
Una frase de una línea que vende el carrusel. Ejemplos:

- **Dolor:** "Gastas 400€/mes en suscripciones que nadie usa."
- **Trofeo:** "Automaticé mi onboarding y ahora atiendo el triple de clientes."
- **Curiosidad:** "Le robaron OAuth a Vercel en 48 horas."

→ Esa frase es el germen de tu portada.

---

## Fase 2 — Estructura (15 min)

Elige una de las 4 estructuras probadas:

### Estructura A — Setup Tour (para .workspace)
```
Slide 1:  Portada — "Mi [setup/stack] para [resultado]"
Slide 2:  Overview — qué incluye todo el sistema
Slide 3-7: Una herramienta/proceso por slide
Slide 8:  Resultado medible ("ahorro X horas/semana")
Slide 9:  CTA — cómo replicarlo o contactarte
```

### Estructura B — Incident Timeline (para .hackroom)
```
Slide 1:  Portada — "Así [pasó X] en [cifra]"
Slide 2:  Timeline — la cadena de eventos
Slide 3-5: Vectores del ataque, uno por slide
Slide 6:  Lección técnica
Slide 7:  Qué hacer TÚ (los 4 pasos)
Slide 8:  Cierre/CTA
```

### Estructura C — Prompt Drop (para .promptroom)
```
Slide 1:  Portada — "El prompt que [hace X]"
Slide 2-6: Un prompt completo por slide, con categoría
Slide 7:  Tips de uso o variaciones
Slide 8:  CTA — "guarda el carrusel"
```

### Estructura D — Comparativa / Teardown
```
Slide 1:  Portada — "[A] vs [B]: la diferencia real"
Slide 2:  Contexto/por qué comparar
Slide 3-4: A y B lado a lado
Slide 5-7: Criterios de elección (uno por slide)
Slide 8:  Tu recomendación + CTA
```

---

## Fase 3 — Escritura (45 min)

### Checklist por slide

#### Portada (slide 1)
- [ ] Título sans-bold, máx. 10 palabras.
- [ ] **Una palabra en itálica serif** (el highlight).
- [ ] Cifra visible (48h, 10 min, 5 personas, 4 pasos...).
- [ ] Subtítulo en una línea (opcional, gris, metadata).
- [ ] Cabecera macOS con nombre de la serie (`juaniaia_.hackroom`).
- [ ] Imagen pixel-art o folder como protagonista (opcional pero fuerte).
- [ ] Paginador space invaders abajo (el primero encendido).

#### Slides interiores
- [ ] Cada slide responde UNA pregunta de la cabeza del lector.
- [ ] Título del slide de 1 línea ideal, 2 líneas máximo.
- [ ] Si va contenido dentro de una ventana negra, tiene header `~ nombre-del-archivo.md`.
- [ ] Si es una lista, numerada 01, 02, 03, 04 (itálica morada, como en el slide de Vercel).
- [ ] Badge de categoría arriba a la izquierda (`/ 02 APRENDER`).
- [ ] Al menos un detalle "de marca": icono pixel, terminal, placeholder en rojo coral `[tema]`.

#### Cierre (último slide)
- [ ] CTA en lenguaje de la marca (ej: `$ dm → @juanaia_`).
- [ ] Si el carrusel genera leads, mención sutil a servicio o a Astrya.
- [ ] El paginador muestra el último invasor encendido.

---

## Fase 4 — Caption del post (20 min)

El caption de Instagram/TikTok es tu **segunda portada**. La estructura que funciona:

### Plantilla de caption
```
[Línea 1: HOOK — la frase más fuerte del carrusel, sin contexto]

[Línea 2-3: el problema real que resuelve]

[Línea 4-8: qué van a encontrar en el carrusel, en bullets cortos]
→ ...
→ ...
→ ...

[Línea 9: CTA suave]
Guarda esto para cuando lo necesites.
O pásalo a ese amigo que [contexto].

[Línea 10: tag/firma]
—
🟣 @juanaia_ | IA aplicada para gente que sí trabaja
```

### Reglas del caption
- **Primera línea sin puntos finales**, es un titular.
- **No más de 4 bullets** con `→` delante.
- **Hashtags al final**, máximo 5 (agrupados en una línea sin espacios entre `#`).
- **Ningún emoji en las primeras 3 líneas** (comen protagonismo al texto).
- **1 emoji máximo en la firma** (el círculo morado 🟣 o el rayo ⚡).

---

## Fase 5 — Checklist final antes de publicar

Pasa este filtro de 8 puntos. Si alguno falla, no publicas:

- [ ] **¿La portada para el scroll?** Lee solo el título: ¿intriga o vende?
- [ ] **¿Se entiende el slide 2 sin haber visto el slide 1?** (los algoritmos te pueden servir cualquier slide primero).
- [ ] **¿Hay una cifra concreta en el carrusel?** Sin cifras, falta autoridad.
- [ ] **¿Hay una palabra humana en un contenido técnico?** (brutal, miedo, honesto, cristal, vida).
- [ ] **¿El último slide pide algo?** Guardar / compartir / DM / probar. No puede ser "gracias".
- [ ] **¿El paginador avanza correctamente (un invasor encendido por slide)?**
- [ ] **¿Todos los slides usan el mismo color de acento?** (no mezclar .workspace verde con .hackroom rojo).
- [ ] **Lee el carrusel en voz alta.** ¿Suena a ti, o a ChatGPT copiado?

---

## Fase 6 — Post-publicación

### Primeros 30 minutos
- Responde TODOS los comentarios. El algoritmo escucha muy fuerte esta ventana.
- Dale like a cada comentario que recibas (acción barata, señal fuerte).

### Primeras 24 horas
- Si el carrusel vuela: prepara un hilo de X/Twitter reciclando los slides como tuits.
- Si el carrusel no vuela: no lo fuerces, pasa al siguiente. 1 de cada 5 sale fuerte, es lo normal.
- Contesta a al menos 10 comentarios en cuentas similares (no spam — aporta).

### Semana siguiente
- Si algún slide del carrusel fue especialmente citado, hazlo un tweet solo.
- Si una frase tuya fue captura de pantalla por alguien, esa frase va a la próxima portada.

---

## Ritmo de publicación sugerido (si preguntas)

```
Lunes     →  .workspace     (setup, cómo trabajas)
Miércoles →  .promptroom    (un prompt)
Viernes   →  .hackroom      (seguridad, análisis, opinión)
```

Tres series × un post semanal = 12 carruseles al mes, 144 al año. Con tu nivel de sistema, es sostenible.

---

## Regla de oro del playbook

> Si algo no cabe en una plantilla — o lo fuerzas a caber, o te das cuenta de que es otro formato (reel, hilo de X, post de texto en LinkedIn). El carrusel no es el único formato. No metas en carrusel algo que es un tuit.
