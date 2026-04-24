# templates/slide-structures.md — Layouts reutilizables

> 7 layouts de slide que ya usas y que puedes combinar para producir carruseles nuevos en minutos. Cada uno tiene su estética y su momento de uso.

---

## Layout 01 — "Desktop"
Cuando quieres: portada inmersiva, mostrar un "sistema".

```
┌─────────────────────────────────────────┐
│ 🔴🟡🟢 juana_ia.workspace          1/8 │
│        juana.ia 2026                    │
├─────────────────────────────────────────┤
│                                         │
│   📁             📁                     │
│  Contenido/    Clientes/                │
│                                         │
│   📁     🐙     📁                      │
│  [tachado]     Research/                │
│                                         │
│                                         │
│                ↓                        │
│        Mi setup de IA                   │
│        reemplazó a un                   │
│        equipo de 5 personas             │
│                                         │
│                                         │
│   📁             📁                     │
│  Diseño/       Automatiza/              │
│                                         │
├─────────────────────────────────────────┤
│         👾 👾 👾 👾 👾 👾 👾            │
└─────────────────────────────────────────┘
```

**Úsalo para:** portadas de la serie `.workspace`.
**No lo uses para:** slides interiores (demasiado vacío, no aporta info).

---

## Layout 02 — "Search + Grid 2×2"
Cuando quieres: mostrar 4 elementos/features/pasos a la vez.

```
┌─────────────────────────────────────────┐
│ 🔴🟡🟢 juana_ia.workspace          4/8 │
├─────────────────────────────────────────┤
│  🟢           Search: Deploy...         │
│                                         │
│  ┌──────────────┐   ┌──────────────┐   │
│  │ Card 1       │   │ Card 2       │   │
│  │ (terminal o  │   │ (terminal o  │   │
│  │  lista)      │   │  lista)      │   │
│  └──────────────┘   └──────────────┘   │
│    Título Card 1       Título Card 2    │
│                                         │
│  ┌──────────────┐   ┌──────────────┐   │
│  │ Card 3       │   │ Card 4       │   │
│  └──────────────┘   └──────────────┘   │
│    Título Card 3       Título Card 4    │
│                                         │
├─────────────────────────────────────────┤
│         👾 👾 👾 👾 👾 👾 👾            │
└─────────────────────────────────────────┘
```

**Úsalo para:** resumen de features, comparativas, "4 pasos", "4 errores".
**Tip:** los títulos SIEMPRE fuera de la card, debajo. Es más limpio.

---

## Layout 03 — "Prompt Card"
Cuando quieres: regalar un prompt listo para copiar.

```
┌─────────────────────────────────────────┐
│ 🔴🟡🟢 juanaia_.promptroom         3/9 │
│        prompt log · 2026                │
├─────────────────────────────────────────┤
│  🔍 Enséñame cualquier cosa en 20 min 📁│
│                                         │
│  / 02   APRENDER                        │
│                                         │
│  El que convierte a Claude en tu        │
│  profesor particular                    │
│                                         │
│  ┌─────────────────────────────────┐   │
│  │ 🔴🟡🟢  ~ learn-fast.md         │   │
│  │                                 │   │
│  │ # funciona con cualquier tema   │   │
│  │                                 │   │
│  │ "Quiero entender [tema].        │   │
│  │  Mi nivel real es [cero /       │   │
│  │  básico / intermedio].          │   │
│  │  Enséñamelo en 4 pasos..."      │   │
│  │                                 │   │
│  └─────────────────────────────────┘   │
│                                         │
├─────────────────────────────────────────┤
│  @juanaia_ · prompt log      👾 👾 👾  │
└─────────────────────────────────────────┘
```

**Úsalo para:** cada slide de `.promptroom`.
**Tip:** la caja negra debe tener el header `~ filename.md` y comentario de uso en cursiva gris. Los placeholders `[entre corchetes]` SIEMPRE en rojo coral.

---

## Layout 04 — "Timeline Terminal"
Cuando quieres: contar una cronología o cadena de eventos.

```
┌─────────────────────────────────────────┐
│ 🔴🟡🟢 juaniaia_.hackroom          2/8 │
│        incident log · 2026              │
├─────────────────────────────────────────┤
│  🔍 Qué pasó con Vercel el 19 abril 📁 │
│                                         │
│  🔴 BREACH · acceso no autorizado...  ↓ │
│                                         │
│  ┌─────────────────────────────────┐   │
│  │ ● Timeline · la cadena          │   │
│  │                                 │   │
│  │ feb 2026   Empleado baja...     │   │
│  │ →          Malware extrae...    │   │
│  │ →          Atacante entra...    │   │
│  │ 19 abr     OAuth tomado...      │   │
│  │ 21 abr     Vercel confirma...   │   │
│  └─────────────────────────────────┘   │
│                                         │
│  ┌─────────────────────────────────┐   │
│  │ 🔴🟡🟢  Terminal — attack.log   │   │
│  │                                 │   │
│  │ $ cat attack.log | head -20     │   │
│  │ → vector: OAuth hijack...       │   │
│  │ → origin: Roblox auto-farm...   │   │
│  │ [ASCII diagram aquí]            │   │
│  │ $ █                             │   │
│  └─────────────────────────────────┘   │
│                                         │
├─────────────────────────────────────────┤
│         👾 👾 👾 👾 👾 👾 👾            │
└─────────────────────────────────────────┘
```

**Úsalo para:** slide 2 de los carruseles de `.hackroom`, case studies con cronología.
**Tip:** deja una línea antes de cada evento del timeline para que respire. El ASCII diagram del final siempre remata con `[algo] ← game over` o similar.

---

## Layout 05 — "Hero Pixel + Título"
Cuando quieres: máximo impacto visual en portada.

```
┌─────────────────────────────────────────┐
│ 🔴🟡🟢 juaniaia_.hackroom          1/8 │
│        incident log · 2026              │
├─────────────────────────────────────────┤
│  ┌─────────────────────────────────┐   │
│  │ 🔴 BREACH · 19 ABR 2026         │   │
│  │  [binary text background]       │   │
│  │                                 │   │
│  │        🎭  ← hero pixel art     │   │
│  │      (hacker, folder, etc.)     │   │
│  │                                 │   │
│  │        [etiqueta anon@0xff]     │   │
│  │                                 │   │
│  └─────────────────────────────────┘   │
│                                         │
│         · CIBERSEGURIDAD ·              │
│                                         │
│         Así hackearon                   │
│         Vercel en 48h                   │
│   el ataque que forzó a medio internet  │
│         a rotar sus API keys            │
│                                         │
├─────────────────────────────────────────┤
│         👾 👾 👾 👾 👾 👾 👾            │
└─────────────────────────────────────────┘
```

**Úsalo para:** portadas impactantes, especialmente en `.hackroom`.
**Tip:** el texto binario detrás del hero no tiene que leerse — es textura. Usa `#2A2D2F` sobre negro para que quede leíble pero secundario.

---

## Layout 06 — "Banner + Grid Numerado"
Cuando quieres: dar una guía accionable con pasos.

```
┌─────────────────────────────────────────┐
│ 🔴🟡🟢 juaniaia_.hackroom          7/8 │
├─────────────────────────────────────────┤
│  🟢 ♡ GUÍA si tienes un deploy en Vercel│
│     haz esto AHORA                      │
│                                         │
│  Asegura tu proyecto en 10 min          │
│  4 pasos · cero excusas · antes de que  │
│  sea tarde                              │
│                                         │
│  ┌──────────────┐   ┌──────────────┐   │
│  │ 01           │   │ 02           │   │
│  │ Rota TODO    │   │ Activa       │   │
│  │ lo no-sensi- │   │ sensitive    │   │
│  │ tive         │   │ en todo      │   │
│  │              │   │              │   │
│  │[$ vercel env]│   │[settings→env]│   │
│  └──────────────┘   └──────────────┘   │
│                                         │
│  ┌──────────────┐   ┌──────────────┐   │
│  │ 03           │   │ 04           │   │
│  │ Auditoría    │   │ Escanea      │   │
│  │ OAuth        │   │ tu repo      │   │
│  │              │   │              │   │
│  │[admin.google]│   │[gitguardian] │   │
│  └──────────────┘   └──────────────┘   │
│                                         │
├─────────────────────────────────────────┤
│         👾 👾 👾 👾 👾 👾 👾            │
└─────────────────────────────────────────┘
```

**Úsalo para:** slide de "acción práctica" (suele ser la penúltima del carrusel).
**Tip:** los números 01-04 en itálica serif morada GRANDES. Cada card termina con una píldora con el comando/path específico abajo.

---

## Layout 07 — "Cierre / CTA"
Cuando quieres: cerrar el carrusel con una acción.

```
┌─────────────────────────────────────────┐
│ 🔴🟡🟢 juana_ia.workspace          8/8 │
├─────────────────────────────────────────┤
│                                         │
│  ┌─────────────────────────────────┐   │
│  │ 🔴🟡🟢  Terminal — zsh          │   │
│  │                                 │   │
│  │ juana@mac ~$ bye                │   │
│  │ → connecting with @juanaia_...  │   │
│  │ → 42,317 subscribers online     │   │
│  │ → dm: open                      │   │
│  │ → astrya.ai: live               │   │
│  │                                 │   │
│  │ $ follow (y/n) █                │   │
│  └─────────────────────────────────┘   │
│                                         │
│  Si esto te fue útil                    │
│  → comparte el post                     │
│  → sígueme para más IA aplicada         │
│  → prueba Astrya: astrya.ai             │
│                                         │
├─────────────────────────────────────────┤
│  @juanaia_ · 2026         👾 👾 👾 👾  │
└─────────────────────────────────────────┘
```

**Úsalo para:** slide final. Evita el "gracias por leer" genérico.
**Tip:** usa el lenguaje de terminal para la CTA. Es on-brand y menos agresivo que el típico "¡Sígueme!".

---

## Matriz de uso

| Tipo de slide | Layouts recomendados |
|---|---|
| Portada impacto visual | 01 (Desktop), 05 (Hero Pixel) |
| Portada prompt/guía | 03 (Prompt Card) |
| Desarrollo con múltiples puntos | 02 (Grid 2×2) |
| Timeline / cronología | 04 (Timeline Terminal) |
| Acción práctica / checklist | 06 (Banner + Grid numerado) |
| Cierre / CTA | 07 (Cierre terminal) |

---

## Regla de ritmo

Un carrusel de 8 slides nunca debe usar 8 layouts distintos. Idealmente:

```
Slide 1:   Layout 01 o 05   (portada impacto)
Slide 2:   Layout 04 o 03   (introducción estructurada)
Slide 3-6: Layout 02 repetido, o variaciones  (desarrollo)
Slide 7:   Layout 06         (acción)
Slide 8:   Layout 07         (cierre)
```

**La repetición de layout crea ritmo.** La variación excesiva rompe la lectura.
