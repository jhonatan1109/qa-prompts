# 🔌 APIs & Servicios

Prompts para diseñar pruebas de APIs REST y generar colecciones de Postman.

---

## Prompt 1 — Casos de prueba para endpoint REST

**Cuándo usarlo:** Recibes un endpoint nuevo y necesitas cubrir todos los escenarios relevantes.

```
Para este endpoint:
Método: [GET / POST / PUT / DELETE / PATCH]
URL: [URL del endpoint]
Headers requeridos: [LISTA DE HEADERS]
Body / Params: [ESTRUCTURA DEL REQUEST]
Auth: [Tipo de autenticación]

Genera casos de prueba cubriendo:
- Respuestas exitosas (2xx) con distintos escenarios
- Errores de cliente (400, 401, 403, 404, 422)
- Errores de servidor (500, 503)
- Validaciones de campos obligatorios y formatos
- Casos límite en los valores de los parámetros
- Pruebas de autorización (con y sin permisos)
```

---

## Prompt 2 — Colección Postman desde contrato de API

**Cuándo usarlo:** Tienes un contrato OpenAPI (Swagger) o un ejemplo de JSON y quieres automatizarlo en Postman.

```
Dado este contrato de API:
[PEGA EL CONTRATO OPENAPI / JSON DE EJEMPLO]

Genera una colección de Postman con:
- Requests organizados por carpeta según recurso
- Tests en JavaScript para cada response (status code, schema, tiempos)
- Variables de entorno necesarias ({{base_url}}, {{token}}, etc.)
- Pre-request scripts si son necesarios para autenticación
```

---

## 💡 Tips

- Incluye ejemplos de request y response si los tienes: mejora mucho la calidad de los casos generados.
- Para el Prompt 2, el JSON de Swagger completo da mejores resultados que fragmentos.
- Pide que los tests de Postman usen `pm.test()` con mensajes descriptivos.
