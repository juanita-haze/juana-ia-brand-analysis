# VOICE.md — Tono, léxico y reglas de escritura

> Si tu marca visual es la "casa", este archivo es el acento con el que hablas dentro de ella. El estilo visual atrae, pero la voz es lo que hace que la gente te siga y vuelva.

---

## 1. Cómo suena tu voz (extraído de tus propios slides)

He recopilado frases literales de tus carruseles para triangular el tono:

| Frase | Observación |
|---|---|
| *"Mi setup de IA reemplazó a un equipo de 5 personas"* | Titular chulo, claim fuerte, implícitamente provocador. |
| *"Así hackearon Vercel en 48h"* | Síntesis + cifra. Cero adjetivos. |
| *"El auditor **brutal** de tus gastos"* | Una palabra emocional dentro de un título técnico. Contraste. |
| *"Sé honesto — no me trates como si fuera de cristal."* | Humanidad máxima. Una frase así desarma al lector. |
| *"4 pasos · cero excusas · antes de que sea tarde"* | Ritmo. Separa con `·`. Compresión. |
| *"Rota TODO lo no-sensitive"* | Imperativo técnico. Mayúsculas selectivas para énfasis. |
| *"[env vars leaked] ← game over"* | Humor techy, referencia gamer, ironía. |
| *"Corrígeme sin piedad si me equivoco en tus preguntas."* | Vulnerabilidad + agencia. Pides ser desafiada. |

**Síntesis del tono:** técnica + humana + irónica + directa. Sin exceso de emoción, sin corporativismo. Escribes como alguien que trabaja de esto y se toma el tiempo de traducirlo.

---

## 2. Los 6 principios de voz de Juana.ia

### 1. Compresión > explicación
Prefieres decir mucho en poco. "48h" vs "en menos de dos días". "48h" gana siempre.

```
✅ "Así hackearon Vercel en 48h"
❌ "Un análisis detallado de cómo un grupo de atacantes logró..."
```

### 2. Lo humano siempre gana al final
El contenido es técnico, pero el remate siempre aterriza en algo humano. El prompt de auditar gastos acaba en *"Sé honesto — no me trates como si fuera de cristal"*. Esa frase es lo que hace que el guardado ocurra.

```
✅ "Responde como respondería esa persona real — con sus defensas, sus interrupciones, sus frases típicas."
❌ "El modelo simulará la interacción según los parámetros dados."
```

### 3. Hablas de "tú" (y con imperativos)
No hay "nosotros hacemos", no hay pasiva. Todo es segunda persona, activa:

```
✅ "Pega tu extracto del último mes."
✅ "Actúa como mi jefe."
✅ "Dime 3 cosas que me ahorraría."
❌ "Se recomienda pegar el extracto..."
```

### 4. Mayúsculas selectivas para énfasis (no negrita)
En lugar de abusar de **negrita**, usas MAYÚSCULAS aisladas. Es más crudo, más terminal.

```
✅ "Rota TODO lo no-sensitive"
✅ "si tienes un deploy en Vercel, haz esto AHORA"
```
Regla: máximo 2-3 palabras en mayúscula por slide.

### 5. Palabras técnicas sin pedir perdón
Dices `deploy`, `env vars`, `OAuth`, `commit`, `MCP` sin traducir. Tu público o lo sabe, o quiere aprenderlo. Traducirlo sería condescendiente.

Pero cuando **el concepto importa**, lo aterrizas con una metáfora humana (*"un token expuesto hace 6 meses hoy vale oro"*).

### 6. Nunca vendes IA como magia
Nunca dices "con IA harás X en minutos". Hablas de **procesos reales**:
- El auditor brutal → "clasifícalos en: necesarios, cómodos, por aburrimiento y por ego".
- El profesor particular → "explícalo como a un niño de 10 años, luego súbelo a nivel adulto...".

Tu IA es una herramienta específica y opinada, no una caja mágica.

---

## 3. Léxico propio (glosario on-brand)

Palabras y giros que usas o puedes usar sin que chirríe:

| Recomendado ✅ | Evitar ❌ |
|---|---|
| Setup, stack | "mi configuración", "mis herramientas" |
| Rotar (keys) | "cambiar las contraseñas" |
| Brecha, breach | "ataque informático" |
| Deploy, desplegar | "poner en producción" |
| Prompt | "instrucción" (excepto para explicar) |
| Env vars | "variables de entorno" (está bien, pero env vars es más tuyo) |
| Build, commit | "construir", "guardar" |
| Workspace | "espacio de trabajo" |
| Roleplay | "simulación de conversación" |
| Brutal, honesto | "útil", "eficiente" |
| Agente | "bot", "asistente" |

**Castellanismos que te sientan bien:** "me da miedo bloquearme", "sin piedad", "no me trates como si fuera de cristal", "cero excusas", "a lo importante".

**Giros que NO encajan en tu marca:**
- "Delve" / "profundizar en" / "adentrarnos"
- "Aprovechar el potencial" / "potenciar"
- "Revolucionario" / "disruptivo" / "game-changer"
- "En este post te cuento..." / "Hoy vengo a hablarte de..."
- "¿Te ha gustado? Dale guardar" (demasiado influencer)
- "Mucho texto, ya te lo resumo" (quiebra la estética)

---

## 4. Reglas duras de escritura

### Reglas de portada (slide 1)
- **Máximo 10 palabras.**
- **Debe contener una cifra o una promesa medible.** (48h, 20 min, 5 personas, 10 pasos).
- **Debe tener una palabra en itálica serif** (IA, roleplay, brutal, 10 min...).
- **No debe explicar el contenido — debe intrigar.**

### Reglas de slide interior
- **Una idea por slide.** Si necesitas dos, son dos slides.
- **Título del slide ≤ 12 palabras**, puede ocupar 2 líneas.
- **El cuerpo monospace** (dentro de una caja `~ filename.md` o terminal) nunca pasa de 8 líneas. Si pasa, parte el slide.
- **Si hay lista, máximo 4 items.** Más de 4 ya no cabe mentalmente.

### Reglas de prompts (serie .promptroom)
Tus prompts siguen una estructura que es ORO y deberías documentarla:

```
"Actúa como [rol específico].

Contexto: [qué pasa en tu vida].

Tarea 1: [acción concreta].
Tarea 2: [otra acción].
Tarea 3: [otra].

Condición final: [cómo quieres que te hable el modelo].
  → Ej: 'Sé honesto', 'Corrígeme sin piedad', 'No me trates como si fuera de cristal'."
```

Cada prompt SIEMPRE termina con una condición de tono/vulnerabilidad. Es tu firma y lo que lo hace guardable.

### Reglas de CTA
Nunca escribas "sígueme para más contenido". En su lugar, adapta al lenguaje de la serie:

```
Workspace:  $ sigue-juana
Hackroom:   → antes de que te hackeen, guarda esto
Promptroom: /copy → /paste → /aplicar
```

---

## 5. Plantilla mental para escribir cualquier carrusel

Antes de dar a publicar, pasa el texto por este filtro de 5 preguntas:

- [ ] ¿El título tiene **una cifra o promesa medible**?
- [ ] ¿Hay **al menos una palabra humana** en un carrusel técnico (o una palabra técnica en uno humano)?
- [ ] ¿La última slide **pide algo** (DM, guardar, probar), y lo pide en el lenguaje de la marca?
- [ ] ¿Hay **algún giro irónico o vulnerable** en algún slide? (sin esto, suena a tutorial plano).
- [ ] ¿Podría este carrusel **confundirse con el de otra cuenta**? Si sí, falta marca.

---

## 6. Tu "voz de Juana" en 3 frases

Si alguien más tuviera que escribir en tu nombre, bastaría con darle esto:

> Escribe como alguien que lleva 5 años automatizando con IA, que odia el bombo, y que tiene un blog de dev pero con un diario personal escondido dentro. Técnica sin ser pedante, emocional sin ser cursi. Si dudas entre una palabra bonita y una palabra exacta, elige la exacta.
