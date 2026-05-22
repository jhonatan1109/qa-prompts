# 🐛 Bugs & Reportes

Prompts para redactar bug reports claros y analizar causas raíz.

---

## Prompt 1 — Redactar bug report profesional

**Cuándo usarlo:** Encontraste un bug y necesitas documentarlo de forma clara para el equipo de desarrollo.

```
Necesito redactar un bug report claro y completo. Tengo esta información:
[DESCRIBE EL BUG BREVEMENTE]

Genera un reporte con:
- Título descriptivo (máx. 10 palabras)
- Ambiente donde ocurre (prod / staging / local)
- Pasos para reproducir (numerados)
- Resultado actual
- Resultado esperado
- Severidad (Crítica / Alta / Media / Baja)
- Prioridad (P1 / P2 / P3)
- Evidencia sugerida (qué capturas o logs adjuntar)
```

---

## Prompt 2 — Análisis de causa raíz con 5 Whys

**Cuándo usarlo:** Un bug fue corregido pero quieres entender la causa raíz y evitar que vuelva a ocurrir.

```
Este bug fue reportado y corregido:
[DESCRIPCIÓN DEL BUG]

Ayúdame a:
1. Formular hipótesis de causa raíz usando el método 5 Whys
2. Sugerir qué áreas del sistema revisar para evitar recurrencia
3. Proponer casos de prueba de regresión específicos para este escenario
```

---

## 💡 Tips

- Agrega contexto técnico si lo tienes: versión del sistema, browser, OS, logs de error.
- Para el prompt 2, incluir el stack trace o mensaje de error mejora mucho la calidad del análisis.
