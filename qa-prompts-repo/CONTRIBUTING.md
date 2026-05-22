# 🤝 Cómo contribuir

¡Gracias por querer aportar a esta biblioteca! Sigue estos pasos para agregar un prompt nuevo.

---

## Pasos para contribuir

### 1. Haz un fork del repositorio

En GitHub, haz clic en el botón **Fork** (arriba a la derecha).

### 2. Clona tu fork

```bash
git clone https://github.com/TU-USUARIO/qa-prompts.git
cd qa-prompts
```

### 3. Crea una rama con un nombre descriptivo

```bash
git checkout -b agregar-prompt-performance-testing
```

### 4. Agrega tu prompt

- Si encaja en una categoría existente: edita el `README.md` de esa carpeta.
- Si es una categoría nueva: crea una carpeta nueva y su `README.md` siguiendo el formato existente.

### 5. Formato del prompt

Usa esta estructura:

```markdown
## Prompt N — [Título del prompt]

**Cuándo usarlo:** [Descripción de 1-2 líneas del caso de uso]

```
[TEXTO DEL PROMPT CON PLACEHOLDERS EN MAYÚSCULAS]
```

```

### 6. Haz commit y push

```bash
git add .
git commit -m "feat: agrega prompt para pruebas de performance"
git push origin agregar-prompt-performance-testing
```

### 7. Abre un Pull Request

En GitHub, abre un PR desde tu rama hacia `main` con:
- Título claro
- Descripción de qué prompt agregaste y por qué es útil

---

## Criterios para que un prompt sea aceptado

- ✅ Tiene un caso de uso claro (no duplica uno existente)
- ✅ Usa placeholders en `[CORCHETES]` para las partes variables
- ✅ Incluye la sección "Cuándo usarlo"
- ✅ Ha sido probado al menos una vez con una IA (ChatGPT, Claude, etc.)

---

## ¿Dudas?

Abre un [Issue](../../issues) con tu pregunta.
