# 📊 Análisis & Estrategia

Prompts para análisis de riesgo de releases y revisión de historias de usuario desde la perspectiva QA.

---

## Prompt 1 — Análisis de riesgo de la release

**Cuándo usarlo:** Antes de una release para priorizar esfuerzo de pruebas donde más importa.

```
Se lanzará esta versión con los siguientes cambios:
[LISTA DE CAMBIOS / FEATURES / FIXES]

Realiza un análisis de riesgo que incluya:
1. Áreas de mayor riesgo y por qué
2. Probabilidad de fallo estimada (Alta / Media / Baja) por área
3. Impacto en el usuario final si falla
4. Estrategia de prueba basada en riesgo (qué probar primero)
5. Sugerencia de criterios mínimos para aprobar la release
```

---

## Prompt 2 — Revisión de historia de usuario como QA

**Cuándo usarlo:** Refinamiento de backlog, antes de que el sprint comience, para detectar ambigüedades temprano.

```
Como QA, revisa esta historia de usuario antes del sprint:
[PEGA LA USER STORY COMPLETA]

Identifica:
1. Ambigüedades o términos que pueden interpretarse de formas distintas
2. Criterios de aceptación faltantes o incompletos
3. Flujos alternos y de error no mencionados
4. Dependencias técnicas o de negocio no mencionadas
5. Preguntas concretas para hacer al Product Owner o equipo

Formato de salida: tabla con columna "Observación" y "Pregunta sugerida".
```

---

## 💡 Tips

- Para el Prompt 1, menciona si hay cambios en integraciones externas, migraciones de datos o cambios de infraestructura.
- Para el Prompt 2, incluir el contexto del producto (qué hace la app, a qué usuarios sirve) mejora la calidad de las preguntas generadas.
