# series/03-promptroom.md — `juanaia_.promptroom`

> **Regalas prompts listos para copiar-pegar, con instrucciones claras y un giro humano.** Esta es tu serie más guardable y la que más tráfico nuevo te trae. Quien guarda un prompt vuelve a tu perfil.

---

## Código visual

- **Color de acento dominante:** 🟣 Morado (`#6B4FE3`) + categorías con color propio.
- **Metáfora:** archivo `.md` abierto en un editor, "prompt log" como diario.
- **Cabecera:** `juanaia_.promptroom` + subtítulo `prompt log · 2026`
- **Estructura fija por slide:** cabecera + search bar + pill de categoría + título + caja negra con el prompt.

---

## Slides analizados de esta serie

### Slide 3/9 — "El que convierte a Claude en tu profesor particular"
- **Categoría:** APRENDER (pill verde).
- **Search query:** *"Enséñame cualquier cosa en 20 minutos"*.
- **Highlight itálico:** "profesor particular" en morado.
- **Prompt completo:**
  ```
  # funciona con cualquier tema: finanzas, código, filosofía

  "Quiero entender [tema]. Mi nivel real es [cero / básico / intermedio].
  Enséñamelo en 4 pasos: 1) explícalo como se lo contarías a un niño de
  10 años con un ejemplo cotidiano, 2) súbelo a nivel adulto con los 3
  conceptos clave, 3) hazme 5 preguntas que pondrían a prueba si lo he
  entendido, 4) dime qué aprendería alguien que lleva 10 años en esto
  y que yo aún no sé. Corrígeme sin piedad si me equivoco en tus preguntas."
  ```

**Por qué funciona:**
- La estructura "4 pasos con progresión de dificultad" es un framework replicable → la gente lo guarda como plantilla mental.
- **"Corrígeme sin piedad"** es el remate emocional. Sin esa frase, es un prompt más.
- "[tema]" en rojo coral como placeholder — la gente ve EXACTAMENTE qué cambiar.

---

### Slide 4/9 — "El roleplay para llegar preparada a lo importante"
- **Categoría:** COMUNICACIÓN (pill amarilla).
- **Search query:** *"Entrena conmigo para una conversación difícil"*.
- **Highlight itálico:** "roleplay" en rojo coral.
- **Prompt completo:**
  ```
  # pedir aumento, cortar a alguien, poner un límite...

  "Actúa como [mi jefe / mi madre / mi ex / ese cliente]. Voy a tener
  una conversación sobre [tema] y me da miedo bloquearme. Responde como
  respondería esa persona real — con sus defensas, sus interrupciones,
  sus frases típicas. Cuando yo te diga 'pausa', salte del personaje y
  dime qué estoy haciendo bien, qué argumento está flojo, y cómo responder
  mejor. Empieza tú."
  ```

**Por qué funciona:**
- **El dolor es altísimo.** Todo el mundo tiene una conversación pendiente. El titular toca hueso.
- "[mi jefe / mi madre / mi ex / ese cliente]" — 4 ejemplos entre corchetes dan 4 escenarios de uso sin escribir 4 prompts.
- El **meta-comando "pausa"** es una técnica de prompt engineering avanzada envuelta en lenguaje cotidiano. Suena simple, es brillante.
- *"me da miedo bloquearme"* — vulnerabilidad en medio de un prompt técnico. Es lo que genera el guardado masivo.

---

### Slide 5/9 — "El auditor brutal de tus gastos"
- **Categoría:** FINANZAS (pill verde menta).
- **Search query:** *"Analiza mi dinero como lo haría un asesor"*.
- **Highlight itálico:** "brutal" en rojo coral.
- **Prompt completo:**
  ```
  # pega tu extracto del último mes

  "Te paso mis gastos de [mes]. Ingresos: [X €], gastos: [Y €].
  Clasifícalos en: necesarios, cómodos, por aburrimiento y por ego.
  Dime 1) en qué categoría gasto más de lo que yo creo, 2) qué 3
  suscripciones o hábitos cortaría sin que mi vida empeore, 3) cuánto
  me ahorraría al año y qué podría hacer con ese dinero. Sé honesto —
  no me trates como si fuera de cristal."
  ```

**Por qué funciona:**
- **"Necesarios, cómodos, por aburrimiento y por ego"** — una taxonomía propia que es oro. Esa frase sola va a ser citada en mil posts.
- Las 3 preguntas numeradas son el framework completo de una auditoría financiera condensado.
- El remate *"no me trates como si fuera de cristal"* — tu firma.

---

## Patrón profundo: la anatomía del prompt Juana-style

Todos tus prompts siguen exactamente la misma estructura. Documentarla es oro:

```
┌────────────────────────────────────────────────┐
│ 1. COMENTARIO DE USO     → "# pega tu extracto"│
│                                                │
│ 2. ROL ASIGNADO          → "Actúa como [X]"    │
│                            o contexto directo  │
│                                                │
│ 3. DATOS DE ENTRADA      → "[tema]" "[X €]"    │
│                            (placeholders en    │
│                             rojo coral)        │
│                                                │
│ 4. TAREAS NUMERADAS      → "1) X, 2) Y, 3) Z"  │
│                                                │
│ 5. CONDICIÓN DE TONO     → "Sé honesto"        │
│    (la firma)              "Corrígeme"         │
│                            "No me trates como  │
│                            si fuera de cristal"│
└────────────────────────────────────────────────┘
```

**Observación clave:** si analizas los prompts sin el paso 5, son prompts técnicos normales. El paso 5 (la condición humana) es lo que convierte un prompt genérico en un "prompt de Juana".

---

## Paleta de categorías detectada (por color de pill)

| Pill | Color | Tipo de prompt |
|---|---|---|
| APRENDER | Verde menta | Aprendizaje, tutoriales, explicaciones |
| COMUNICACIÓN | Amarillo mostaza | Conversaciones, relaciones, social |
| FINANZAS | Verde menta (también) | Dinero, presupuestos, decisiones |
| *(futuras)* | | |
| TRABAJO | Morado sugerido | Productividad, gestión, equipos |
| SALUD | Rojo coral sugerido | Rutinas, hábitos, mental |
| NEGOCIO | Turquesa sugerido | Founders, estrategia, lanzamientos |
| CREATIVIDAD | Naranja sugerido | Escritura, ideas, marca personal |

---

## Fórmulas de portada para la serie `.promptroom`

```
1. "El que [logra X] en [tiempo]"
2. "El [tipo de experto] para cuando [situación]"
3. "Enséñame [cosa]" / "Analiza [cosa]" / "Entrena conmigo..."
4. "El prompt que reemplaza a [persona/profesional]"
5. "Cómo [verbo difícil] sin [fricción clásica]"
```

---

## Ideas de carruseles futuros en esta serie

Cada idea tiene potencial de ser el siguiente slide de tu `.promptroom`. Todos los prompts deben seguir la anatomía descrita arriba.

### TRABAJO
1. **"El que revisa tu CV como si fuera head of hiring"** — roast útil.
2. **"El que escribe emails de cobro sin culpa"** — para freelancers.
3. **"El planificador de semana que no te deja procrastinar"**.
4. **"El revisor de propuestas antes de enviarlas al cliente"**.

### SALUD / VIDA
5. **"El coach que te monta la rutina que SÍ vas a seguir"**.
6. **"El que te ayuda a cortar con algo (o alguien)"**.
7. **"El diario de ansiedad que no te juzga"**.

### NEGOCIO / FOUNDERS
8. **"El que critica tu pitch sin piedad"**.
9. **"El que detecta el agujero en tu modelo de negocio"**.
10. **"El que escribe 5 variantes de tu landing en 2 minutos"**.

### CREATIVIDAD
11. **"El que convierte tus notas de voz en un artículo"**.
12. **"El que detecta tu voz y la imita para escribir en ti"**.
13. **"El que te obliga a publicar (con deadline y todo)"**.

### DÍA A DÍA
14. **"El que decide por ti cuando estás saturada"**.
15. **"El que te prepara las conversaciones del día"**.

---

## Tips específicos de esta serie

- **Cada prompt debe caber en la caja negra sin overflow.** Prueba en el maquetado antes de darle al OK.
- **Los placeholders `[entre corchetes]` siempre en rojo coral.** Esto es ley en tu marca.
- **El hashtag `#` de comentario de uso siempre en cursiva gris.** Es un metadata, no parte del prompt.
- **La última frase (la condición humana) debe ser tuya, no genérica.** Evita "responde de forma detallada"; prefiere "no me trates como si fuera de cristal".

---

## Oportunidad: empaquetar la serie como producto

Con 30-50 prompts siguiendo esta estructura, tienes un **mini-producto vendible**:
- Notion template con todos los prompts categorizados.
- PDF descargable con tu branding.
- Add-on para Astrya: "librería de prompts de Juana".
- Curso corto: "Cómo escribir prompts que funcionan" (usando tu anatomía como framework).

La serie `.promptroom` es la más fácil de monetizar porque **cada slide ya es, por sí sola, un producto en miniatura**.
