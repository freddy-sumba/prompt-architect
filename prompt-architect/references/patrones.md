# Patrones de prompt por tipo de tarea

## 1. Zero-shot
Tareas simples y bien definidas. Rol + tarea + formato + restricciones.

## 2. Few-shot
Cuando el formato o estilo es difícil de describir.
- 3–5 ejemplos representativos, al menos un caso límite.
- Separa cada uno con `<ejemplo>`.

## 3. Extracción estructurada (JSON)
Convertir texto libre en JSON, tabla o esquema.
- Define el esquema exacto.
- Indica qué hacer si falta un campo: `null`, `"desconocido"` o error.
- Prohíbe inventar valores.
- Fuerza el formato: "Devuelve solo el JSON" + esquema; prefill con `{` o salida estructurada si el modelo lo soporta.

## 4. Clasificación
- Lista cerrada de categorías con definición breve.
- Regla para ambiguos ("si dudas entre A y B, elige A").
- Salida en formato fijo.

## 5. Generación con criterios
Contenido abierto con estándares.
- Audiencia, tono, longitud, estructura.
- Criterios de calidad explícitos.
- Qué evitar (formulado en positivo).

## 6. Agente con herramientas
- Lista de herramientas y cuándo usar cada una.
- Cuándo NO usarlas.
- Qué hacer si fallan.
- Formato de llamada y límite de iteraciones.

## 7. Auditoría de prompts
- Revisar con `checklist.md`.
- Señalar problemas concretos.
- Proponer versión mejorada + changelog.

## 8. Cadena de verificación
Tareas críticas: generar → verificar contra criterios → corregir si falla → entregar solo la versión final.
