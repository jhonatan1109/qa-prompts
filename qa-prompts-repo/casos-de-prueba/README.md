# 🗂 Casos de Prueba

Prompts para generar, diseñar y optimizar casos de prueba a partir de requisitos.

---

## Prompt 1 — Generar casos de prueba desde un requisito

**Cuándo usarlo:** Tienes un requisito o historia de usuario y necesitas casos de prueba completos rápidamente.

```
Actúa como QA senior. Dado este requisito:
[PEGA EL REQUISITO]

Genera casos de prueba completos incluyendo:
- ID
- Descripción
- Precondiciones
- Pasos detallados
- Datos de entrada
- Resultado esperado
- Prioridad (Alta / Media / Baja)
```

---

## Prompt 2 — Casos límite y valores extremos

**Cuándo usarlo:** Quieres asegurarte de cubrir los bordes y casos que suelen escaparse.

```
Para esta funcionalidad:
[DESCRIBE LA FUNCIONALIDAD]

Genera casos de prueba de:
- Valores límite (boundary values)
- Partición de equivalencias
- Casos negativos importantes

Que un QA experimentado no pasaría por alto.
```

---

## Prompt 3 — Matriz de prueba para combinaciones (Pairwise)

**Cuándo usarlo:** Tienes múltiples parámetros con varios valores y necesitas reducir combinaciones sin perder cobertura.

```
Tengo estos parámetros con sus valores posibles:
[LISTA PARÁMETROS Y VALORES]

Crea una matriz de prueba usando la técnica de pairwise testing
para reducir el número de combinaciones manteniendo cobertura efectiva.
Explica qué combinaciones cubre cada caso.
```

---

## 💡 Tips

- Sé específico al describir el requisito: incluye reglas de negocio, restricciones y flujos alternos.
- Pide la salida en formato tabla si la vas a pegar en Jira, Excel o Confluence.
- Agrega al prompt: *"Formato: tabla Markdown"* o *"Formato: JSON"* según tu necesidad.
