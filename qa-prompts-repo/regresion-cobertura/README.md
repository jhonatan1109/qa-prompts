# 🔁 Regresión & Cobertura

Prompts para definir suites de regresión e identificar gaps en la cobertura de pruebas.

---

## Prompt 1 — Suite de regresión para nueva feature

**Cuándo usarlo:** Se va a lanzar un cambio y necesitas saber qué probar más allá de lo nuevo.

```
Se va a lanzar esta nueva funcionalidad:
[DESCRIBE LA FEATURE Y LOS CAMBIOS TÉCNICOS]

1. Identifica qué módulos o flujos existentes podrían verse afectados
2. Para cada área de riesgo, explica por qué podría tener impacto
3. Prioriza la lista de mayor a menor riesgo
4. Sugiere qué casos de regresión son candidatos para automatizar
```

---

## Prompt 2 — Identificar gaps de cobertura

**Cuándo usarlo:** Quieres saber qué escenarios importantes te están faltando en tu suite actual.

```
Tengo estos casos de prueba existentes:
[LISTA O DESCRIBE LOS CASOS ACTUALES]

Para esta funcionalidad:
[DESCRIBE LA FUNCIONALIDAD COMPLETA]

Identifica:
- Escenarios importantes no cubiertos
- Flujos alternos ignorados
- Casos de error no probados
- Combinaciones de datos no consideradas

Devuelve la lista priorizada con justificación de por qué cada gap es relevante.
```

---

## 💡 Tips

- Para el Prompt 1, menciona si hay cambios en base de datos, integraciones o servicios externos.
- Para el Prompt 2, mientras más detallada sea la descripción de la funcionalidad, más precisos serán los gaps identificados.
