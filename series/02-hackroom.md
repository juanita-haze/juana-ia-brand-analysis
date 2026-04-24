# series/02-hackroom.md — `juaniaia_.hackroom`

> **Analizas incidentes reales y los explicas mejor que la prensa tech.** Esta serie te da autoridad técnica y genera urgencia accionable. Quien lo lee, revisa sus propios deploys después.

---

## Código visual

- **Color de acento dominante:** 🔴 Rojo coral (`#FF6B5E`) + complementario morado.
- **Metáfora:** sala de control de incidentes, logs, timelines de ataque.
- **Cabecera:** `juaniaia_.hackroom` + subtítulo `incident log · 2026`
- **Detalle sutil:** aquí el handle tiene **doble `i` en `juaniaia_`** — una variación micro que diferencia la serie. Es casi imperceptible pero da sensación de sistema.

---

## Slides analizados de esta serie (carrusel Vercel, 8 slides)

### Slide 1/8 — Portada "Así hackearon Vercel en 48h"

**Lo que veo:**
- Caja negra gigante ocupando el 70% superior.
- Dentro: **texto binario difuminado** (1010100, API_KEY, LEAKED, ROOT_IN, PWNED...) en los laterales, dando sensación de logs.
- Badge rojo coral arriba a la izquierda: `⚠ BREACH · 19 ABR 2026`.
- En el centro, **icono pixel-art de un hacker encapuchado** con ojos rojos brillantes y barra verde debajo (tipo terminal blink).
- Etiqueta roja abajo: `anon@0xff`.
- Fuera de la caja, ya en crema:
  - Subtítulo pequeño: `· CIBERSEGURIDAD ·`
  - Título GIGANTE: **"Así hackearon *Vercel* en *48h*"** (Vercel en itálica roja, 48h en itálica morada — **dos highlights en una sola portada**, excepción a la regla normal).
  - Subtítulo: *"el ataque que forzó a medio internet a rotar sus API keys"*
- Paginador space invaders (primer invasor morado encendido).

**Por qué funciona (brutal análisis):**
- **Es el mejor slide 1 de toda tu serie.** Equivale a una portada de NYT: imagen potente + título + bajada.
- El fondo con texto binario no tiene que leerse — **comunica atmósfera**. Es tipografía como textura.
- El contraste entre la caja negra superior y el título en fondo crema crea una tensión visual que el ojo no puede ignorar.
- Doble highlight (Vercel + 48h) funciona aquí porque uno es el sujeto y el otro es el número. Cada uno en un color diferente (coral / morado) para que no compitan.

### Slide 2/8 — Timeline "Qué pasó con Vercel el 19 abril"

**Lo que veo:**
- Search bar con query: *"Qué pasó con Vercel el 19 abril"* (placeholder con bold en "Vercel" y "19 abril").
- Folder rojo coral a la derecha.
- **Banner de alerta**: `BREACH · acceso no autorizado · Vercel · 19 abr 2026 ↓`.
- **Caja negra con timeline**:
  ```
  feb 2026  →  Empleado de Context.ai baja exploits de Roblox → infección Lumma stealer
  →           Malware extrae Google Workspace, Supabase, Datadog, Authkit
  →           Atacante entra en la app de Context.ai instalada por empleado de Vercel
  19 abr    →  OAuth tomado · acceso a Google Workspace de Vercel → adentro
  21 abr    →  Vercel confirma brecha y notifica a clientes afectados
  ```
- **Caja negra de terminal** con `cat attack.log | head -20` mostrando:
  - vector, origin, impact
  - Una diagrama ASCII de la cadena: `[Roblox] → [Lumma] → [Context.ai employee creds stolen] → [OAuth token] → [Vercel Workspace] → [env vars leaked] ← game over`

**Por qué funciona:**
- **"Game over" al final de la cadena** es pura poesía. Mezcla humor gamer con gravedad técnica. Una frase así hace que quien lo vea piense "esta persona sabe cómo comunicar".
- El timeline dentro de la caja negra es fácil de escanear: fechas a la izquierda, acción a la derecha. No necesitas leer todo para entender.
- El ASCII diagram es **oro de guardado**. Gente que ni va a leer el detalle captura esa caja para su notion.

**Nota crítica:**
- Slide muy denso. Si alguien entra por aquí sin contexto, puede saturarse. Compensado por el slide 1 (que pasa 70% del ojo antes).

---

### Slide 7/8 — Guía "Asegura tu proyecto en 10 min"

**Lo que veo:**
- Banner verde (cambio de color — pasa del rojo "alerta" al verde "acción").
- Texto: `♡ GUÍA si tienes un deploy en Vercel, haz esto AHORA`.
- Título GIGANTE: "Asegura tu proyecto en *10 min*".
- Subtítulo: *"4 pasos · cero excusas · antes de que sea tarde"*.
- **Grid 2×2** de cards negras, numeradas 01-02-03-04 en itálica serif morada:
  1. **Rota TODO lo no-sensitive** → `$ vercel env ls`
  2. **Activa "sensitive" en todo** → `settings → env → sensitive`
  3. **Auditoría OAuth Workspace** → `admin.google · security`
  4. **Escanea tu repo** → `gitguardian · scan`

**Por qué funciona:**
- **Transición emocional perfecta**: toda la serie te mete miedo (rojo, BREACH, game over) y entonces llega ESTE slide verde con la solución. El alivio hace que sea el slide más compartido.
- Cada card tiene **la acción + el comando o path** para ejecutarla. Eliminaste cualquier fricción entre leer y actuar.
- Los números 01-04 en itálica serif morada + el título en sans bold + el footer mono → usas las 3 tipografías en una sola slide sin que chirríe. Masterclass.

---

## Fórmulas de portada para la serie `.hackroom`

```
1. "Así hackearon [empresa conocida] en [tiempo corto]"
2. "El bug de [herramienta] que pocos conocen (y tú usas a diario)"
3. "[Cifra] de empresas afectadas por [incidente]. La cadena real."
4. "[Empresa] filtró [cosa]. Cómo saber si te afecta."
5. "El vector que casi nadie audita: [cosa técnica específica]"
```

## Ideas de carruseles futuros en esta serie

1. **"OAuth: el eslabón más roto de 2026"** — no un incidente, sino una serie de mini-incidentes enlazados.
2. **"Tu prompt a ChatGPT también es un vector"** — incidentes de prompt injection.
3. **"5 APIs que filtran datos que ni sabías que expones"**.
4. **"Lumma Stealer: qué es, cómo se propaga, cómo detectarlo"**.
5. **"El mail de phishing que nadie detectó en mi empresa"** (case study personal).
6. **"Así analicé un incidente en 3 horas con IA"** — cruce con `.workspace`.
7. **"Tu repo de Github filtra secretos. Este prompt los encuentra todos"** — cruce con `.promptroom`.
8. **"Los 4 errores de seguridad que todos los founders cometen al lanzar"**.
9. **"Por qué los MCP servers son el próximo gran agujero"** (tema emergente).
10. **"Pentesting con IA: lo que un atacante ya está haciendo con tu dominio"**.

---

## Tips específicos de esta serie

- **Siempre estructura = alerta + timeline + lección + acción.** Es la arquitectura emocional del carrusel que convierte.
- **Los terminales con logs falsos pero plausibles son tu ventaja.** Inviertes 30 minutos más en el diseño, pero la gente los captura como si fueran reales.
- **El humor es tu secreto.** "game over", "adentro", "pwned", "0xff" — todos los guiños gamer/hacker son lo que te separan de un análisis aburrido de Xataka.
- **Siempre cierra con ACCIÓN.** La gente no comparte miedo, comparte soluciones.
- **Cuida las fechas.** Esta serie envejece. Un carrusel sobre un incidente de hace 2 años se ve desactualizado. Publica dentro de los 7-14 días del incidente para captar la ola.

---

## Riesgo a vigilar

- **No te conviertas en "la cuenta de tragedias".** Si todas tus slides son negras con BREACH, la gente asocia tu marca con ansiedad. Mantén la proporción: máximo 1 carrusel `.hackroom` cada 2 de `.workspace` o `.promptroom`.
- **Verifica siempre la información.** Esta serie te da autoridad, pero un error factual te la quita más rápido de lo que la ganaste. Referencia fuentes en el caption.
- **No hagas clickbait con empresas.** El titular "Así hackearon Vercel en 48h" funciona porque es verdad; si lo inventas o exageras, pierdes la confianza de la comunidad tech.
