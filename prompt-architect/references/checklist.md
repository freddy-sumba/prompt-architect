# Checklist de calidad

Marca cada punto antes de entregar un prompt.

## Claridad
- [ ] El rol está definido y aporta valor.
- [ ] El objetivo es concreto y medible.
- [ ] La tarea usa verbos de acción claros.
- [ ] Las instrucciones están en positivo (no solo "no hagas X").

## Estructura
- [ ] El contexto es suficiente pero no excesivo.
- [ ] Instrucciones y datos están separados con XML tags.
- [ ] Las variables están declaradas y descritas.
- [ ] El prompt empieza simple y no acumula reglas innecesarias.

## Restricciones
- [ ] Las restricciones no se contradicen.
- [ ] Se contemplan casos límite o falta de información.
- [ ] Se indica qué hacer ante ambigüedad.

## Salida
- [ ] El formato de salida es explícito.
- [ ] Hay criterios de éxito verificables.
- [ ] Se especifica longitud o estructura esperada.
- [ ] Si el formato es estricto, se define esquema (y prefill/salida estructurada si el modelo lo soporta).

## Calidad
- [ ] Los ejemplos (si hay) son representativos y no sesgados.
- [ ] El prompt es testeable con un caso real.
- [ ] No hay fugas de datos sensibles.

## Seguridad
- [ ] Se contemplan instrucciones maliciosas o inyecciones en los datos de entrada.
- [ ] Se indica manejo de información privada.
- [ ] Se evita pedir contenido dañino o ilegal.

## Reutilización
- [ ] Se usan variables si el prompt debe reutilizarse.
- [ ] El prompt es independiente del modelo (salvo que se pida lo contrario).

## Entrada por audio
- [ ] Se eliminaron muletillas y frases cortadas.
- [ ] Se reconstruyó la intención real.
- [ ] Los supuestos están declarados.
