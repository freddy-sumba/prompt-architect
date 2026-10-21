# Plantilla base del prompt

Adapta según la tarea; **elimina las secciones que no aporten**.

```text
# ROL
Eres {{rol_experto}} con experiencia en {{dominio}}.

# OBJETIVO
{{resultado_concreto_que_debe_lograr}}

# CONTEXTO
<contexto>
{{contexto_relevante}}
Audiencia: {{audiencia}}
Tono: {{tono}}
Idioma: {{idioma}}
</contexto>

# TAREA
{{instruccion_principal_en_verbo_imperativo}}

# ENTRADAS
<entrada>
- {{variable_1}}: {{descripcion}}
- {{variable_2}}: {{descripcion}}
</entrada>

# PROCESO
1. {{paso_1}}
2. {{paso_2}}
3. {{paso_3}}

# RESTRICCIONES
- Responde en {{idioma}}.
- Si falta un dato, indícalo explícitamente en lugar de inventarlo.
- Longitud máxima: {{longitud}}.
- Prioriza {{prioridad}}.
- Evita {{cosas_a_evitar}}.

# FORMATO DE SALIDA
Devuelve exactamente:
1. {{seccion_1}}
2. {{seccion_2}}
3. {{seccion_3}}

# CRITERIOS DE CALIDAD
- {{criterio_1}}
- {{criterio_2}}
- {{criterio_3}}

# EJEMPLOS (opcional)
<ejemplo>
Entrada: {{ejemplo_entrada}}
Salida esperada: {{ejemplo_salida}}
</ejemplo>
```
