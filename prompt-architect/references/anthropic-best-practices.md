# Buenas prácticas de Anthropic (resumen)

## Principios base
1. **Claridad y detalle.** Trata a Claude como un genio nuevo en el puesto: no adivina lo que no le dices. Explica el motivo de las reglas.
2. **Rol explícito.** Define quién es Claude en la tarea (system prompt).
3. **XML tags.** Separa instrucciones de datos con `<contexto>`, `<entrada>`, `<ejemplo>`.
4. **Formato de salida explícito.** Si quieres JSON, dilo y da el esquema.
5. **Few-shot.** 3–5 ejemplos bien elegidos superan párrafos de descripción.
6. **Razonar antes de responder.** En tareas complejas, pide análisis y respuesta final por separado.

## Específico de Claude
- XML suele funcionar mejor que markdown para separar bloques.
- **Prefill** (iniciar la respuesta del asistente, p. ej. con `{`) fuerza formato en modelos que lo soportan; en los que no, usa instrucciones claras, esquema y salida estructurada.
- **System prompt = rol + contexto + reglas**, conciso pero explícito.
- Prefiere extended/adaptive thinking o razonamiento estructurado a un "piensa paso a paso" genérico.
- Reformula en positivo: "haz Y" en lugar de "no hagas X".

## Anti-patrones
- Instrucciones contradictorias ("sé detallado pero breve").
- Ejemplos sesgados o poco representativos.
- Pedir "no alucines" sin criterios de verificación (mejor: "si no hay datos, dilo").
- Mezclar datos del usuario con instrucciones en el mismo bloque.
- Suponer que Claude "entiende la intención" sin decírsela.

## Ciclo recomendado
1. Empezar simple.
2. Probar con casos reales.
3. Iterar sobre lo que falla.
4. Evaluar con un set pequeño de pruebas antes de darlo por bueno.

## Recursos oficiales
- https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview
- https://docs.claude.com/en/resources/prompt-library/library
- https://www.anthropic.com/learn
