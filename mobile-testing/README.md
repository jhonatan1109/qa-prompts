# 📱 Mobile Testing

Prompts para diseñar y ejecutar pruebas en aplicaciones móviles (iOS y Android).

---

## Prompt 1 — Casos de prueba para app móvil

**Cuándo usarlo:** Tienes una funcionalidad nueva en la app y necesitas casos de prueba considerando el contexto móvil.

```
Actúa como QA especializado en mobile. Para esta funcionalidad:
[DESCRIBE LA FUNCIONALIDAD DE LA APP]

Plataformas: [iOS / Android / ambas]

Genera casos de prueba cubriendo:
- Flujo principal en pantalla táctil
- Gestos específicos (swipe, pinch, tap, long press)
- Comportamiento en diferentes tamaños de pantalla
- Orientación portrait y landscape
- Interrupciones (llamada entrante, notificación, cambio de app)
- Comportamiento sin conexión / conexión lenta
- Permisos del sistema (cámara, ubicación, notificaciones)
```

---

## Prompt 2 — Pruebas de compatibilidad de dispositivos

**Cuándo usarlo:** Necesitas decidir en qué dispositivos y versiones de OS probar sin revisar todos.

```
Tengo esta app móvil:
Plataforma: [iOS / Android / ambas]
Funcionalidad a probar: [DESCRIBE]
Estadísticas de usuarios (si las tienes): [VERSIONES DE OS MÁS USADAS]

Recomienda:
1. Matriz de dispositivos y versiones de OS prioritarios para probar
2. Justificación de cada combinación elegida
3. Casos donde el comportamiento podría diferir entre versiones
4. Herramientas sugeridas para pruebas en dispositivos reales o emuladores
```

---

## Prompt 3 — Pruebas de usabilidad móvil

**Cuándo usarlo:** Quieres evaluar si una pantalla o flujo es usable en móvil antes de lanzar.

```
Revisa este flujo de una app móvil desde la perspectiva de usabilidad:
[DESCRIBE EL FLUJO O PEGA EL DISEÑO / PROTOTIPO]

Evalúa:
- Tamaño de elementos táctiles (mínimo recomendado 44x44 pts)
- Legibilidad de textos en pantallas pequeñas
- Flujo de navegación (¿es intuitivo?)
- Posición de elementos clave (¿alcanzables con el pulgar?)
- Feedback visual al usuario (loaders, errores, confirmaciones)
- Posibles fricciones o pasos innecesarios

Entrega un listado de observaciones con nivel de impacto (Alto / Medio / Bajo).
```

---

## Prompt 4 — Pruebas de rendimiento móvil

**Cuándo usarlo:** La app se siente lenta o quieres establecer criterios de performance antes del lanzamiento.

```
Para esta app móvil:
[DESCRIBE LA APP Y LA FUNCIONALIDAD A EVALUAR]

Genera un plan de pruebas de rendimiento que incluya:
- Métricas clave a medir (tiempo de carga, uso de CPU, memoria, batería)
- Escenarios de prueba (primer arranque, navegación, carga de datos)
- Condiciones de red a simular (4G, 3G, WiFi, offline)
- Herramientas recomendadas (Android Profiler, Xcode Instruments, etc.)
- Umbrales de aceptación sugeridos para cada métrica
```

---

## Prompt 5 — Script de prueba automatizado con Appium

**Cuándo usarlo:** Quieres automatizar un flujo de la app móvil con Appium.

```
Crea un script de prueba automatizado con Appium en [Python / JavaScript / Java]
para este flujo:
[DESCRIBE EL FLUJO A AUTOMATIZAR]

App: [iOS / Android]
Versión de OS: [VERSIÓN]

Requisitos:
- Usa Page Object Model (POM)
- Selectores robustos (accessibility id, resource-id o xpath como último recurso)
- Manejo de waits explícitos
- Manejo de permisos del sistema si aplica
- Comentarios explicativos en el código
```

---

## 💡 Tips

- Para el Prompt 1, menciona si la app usa gestos personalizados o tiene modo oscuro — son áreas frecuentes de bugs.
- Para el Prompt 2, Google Analytics o Firebase te dan las versiones de OS reales de tus usuarios — úsalas como input.
- Para el Prompt 5, incluir el `appium-inspector` screenshot del elemento mejora mucho la calidad de los selectores generados.
