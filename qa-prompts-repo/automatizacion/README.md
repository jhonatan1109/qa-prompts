# ⚙️ Automatización

Prompts para generar, convertir y mejorar scripts de prueba automatizados.

---

## Prompt 1 — Generar script automatizado desde cero

**Cuándo usarlo:** Necesitas automatizar un flujo y quieres un punto de partida sólido.

```
Crea un script de prueba automatizado con [Cypress / Playwright / Selenium]
para este escenario:
[DESCRIBE EL FLUJO A AUTOMATIZAR]

Requisitos:
- Usa Page Object Model (POM)
- Manejo correcto de waits (no hardcodees tiempos)
- Aserciones claras y descriptivas
- Comentarios explicativos en el código
- Manejo básico de errores
```

---

## Prompt 2 — Convertir caso manual a script automatizado

**Cuándo usarlo:** Ya tienes un caso de prueba manual documentado y quieres pasarlo a código.

```
Tengo este caso de prueba manual:
[PEGA EL CASO MANUAL]

Conviértelo a un script automatizado en [FRAMEWORK].

Además:
- Optimiza los selectores para que sean robustos y mantenibles
  (preferir data-testid, aria-label o roles sobre clases CSS)
- Separa los datos de prueba del código
- Estructura el código para que sea fácil de mantener
```

---

## Prompt 3 — Revisar y mejorar script existente

**Cuándo usarlo:** Tienes un script que falla intermitentemente o que un compañero escribió y quieres mejorarlo.

```
Revisa este script de prueba e identifica problemas:
[PEGA EL CÓDIGO]

Busca específicamente:
- Flakiness potencial (causas de fallos intermitentes)
- Malas prácticas de automatización
- Waits hardcodeados (sleep / wait fijo)
- Aserciones débiles o incorrectas
- Selectores frágiles

Devuelve: lista de problemas encontrados + versión mejorada del código.
```

---

## 💡 Tips

- Especifica la versión del framework si es relevante (ej: Cypress 13, Playwright 1.40).
- Indica si el proyecto ya tiene una estructura definida para que el código encaje.
- Para el Prompt 3, incluir el mensaje de error que arroja el script mejora mucho el diagnóstico.
