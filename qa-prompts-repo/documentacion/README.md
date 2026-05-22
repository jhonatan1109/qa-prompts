# 📄 Documentación

Prompts para generar planes de prueba, criterios de aceptación y reportes ejecutivos.

---

## Prompt 1 — Plan de pruebas completo

**Cuándo usarlo:** Inicio de sprint, proyecto nuevo o release importante que requiere documentación formal.

```
Crea un plan de pruebas para este proyecto / sprint:
[DESCRIBE EL PROYECTO, ALCANCE DEL SPRINT Y CONTEXTO]

Incluye:
- Alcance (qué se prueba y qué no)
- Estrategia de prueba (tipos: funcional, regresión, integración, etc.)
- Criterios de entrada (cuándo empezar a probar)
- Criterios de salida (cuándo se considera listo para producción)
- Riesgos identificados y mitigación
- Recursos y responsables
- Cronograma estimado
```

---

## Prompt 2 — Criterios de aceptación en Gherkin

**Cuándo usarlo:** Refinamiento de backlog. Conviertes historias de usuario en escenarios concretos y ejecutables.

```
Para esta historia de usuario:
[PEGA LA USER STORY]

Escribe criterios de aceptación en formato Gherkin (Given / When / Then) cubriendo:
- Flujo principal (happy path)
- Flujos alternos
- Escenarios de error
- Casos límite relevantes

Usa Scenario Outline con Examples cuando haya variaciones de datos.
```

---

## Prompt 3 — Reporte ejecutivo de resultados

**Cuándo usarlo:** Al cierre de un ciclo de pruebas, para comunicar resultados a stakeholders no técnicos.

```
Dado este resumen de ejecución:
- Total de casos: [N]
- Pasados: [N]
- Fallidos: [N]
- Bloqueados: [N]
- Bugs críticos encontrados: [LISTA BREVE]
- Ambiente probado: [NOMBRE]
- Fecha / período: [FECHA]

Redacta un reporte ejecutivo de testing que sea:
- Claro para stakeholders no técnicos
- Incluya semáforo de calidad (Verde / Amarillo / Rojo) con justificación
- Recomendación de go / no-go para producción
- Próximos pasos sugeridos
```

---

## 💡 Tips

- Para el Prompt 2, pide la salida en formato compatible con tu herramienta (Cucumber, SpecFlow, Behave).
- Para el Prompt 3, incluir la lista de bugs con severidad mejora la recomendación de go/no-go.
